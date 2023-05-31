# Comparing `tmp/baklabel-1.2.0.tar.gz` & `tmp/baklabel-1.2.1.tar.gz`

## Comparing `baklabel-1.2.0.tar` & `baklabel-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 baklabel-1.2.0/doc/about.txt
--rw-r--r--   0        0        0    21203 2020-02-02 00:00:00.000000 baklabel-1.2.0/doc/backup_howto.txt
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 baklabel-1.2.0/doc/instructions.txt
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 baklabel-1.2.0/doc/release_note.txt
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 baklabel-1.2.0/doc/synopsis.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.0/src/baklabel/__init__.py
--rw-r--r--   0        0        0    24128 2020-02-02 00:00:00.000000 baklabel-1.2.0/src/baklabel/baklabel.py
--rw-r--r--   0        0        0    22619 2020-02-02 00:00:00.000000 baklabel-1.2.0/src/baklabel/test_baklabel.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 baklabel-1.2.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 baklabel-1.2.0/LICENSE
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 baklabel-1.2.0/README.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 baklabel-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 baklabel-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.1/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 baklabel-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 baklabel-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 baklabel-1.2.1/doc/about.txt
+-rw-r--r--   0        0        0    20706 2020-02-02 00:00:00.000000 baklabel-1.2.1/doc/backup_howto.txt
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 baklabel-1.2.1/doc/examples.txt
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 baklabel-1.2.1/doc/release_note.txt
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 baklabel-1.2.1/doc/synopsis.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.1/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.1/src/baklabel/__init__.py
+-rw-r--r--   0        0        0    24161 2020-02-02 00:00:00.000000 baklabel-1.2.1/src/baklabel/baklabel.py
+-rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 baklabel-1.2.1/src/baklabel/test_baklabel.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 baklabel-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 baklabel-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 baklabel-1.2.1/README.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 baklabel-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 baklabel-1.2.1/PKG-INFO
```

### Comparing `baklabel-1.2.0/doc/backup_howto.txt` & `baklabel-1.2.1/doc/backup_howto.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Target Audience - baklabel
 ==========================
 
-The 'baklabel' utility is intended for a system administrator to install and set up to suit the system owner. It is meant for small office or home networks which prefer to use high capacity portable disk drives rather than tapes.
-
-The instructions are intended to be more or less understandable by most users but the detailed sections will require some experience or at least moderate confidence.
+The 'baklabel' utility is intended for a system administrator to install and set up to suit the system owner. The instructions are intended to be more or less understandable by most users but the detailed sections will require some experience or at least moderate confidence.
 
 This document describes grandfathered backups. It then explains in overview how to install the necessary components to make a grandfathered backup system actually work. Finally, it contains the exact (five line) Python script needed to use baklabel and two example Windows batch files which employ xcopy in one and robocopy in the other to perform the backups.
 
 All Windows systems have xcopy and some also have robocopy. Robocopy is more reliable for larger backups.
 
 Linux or Mac based systems will require a bash script similar to the batch file. Also, the examples are based on Windows so drive letters will need to be replaced by network paths on non-Windows machines.
 
@@ -17,17 +15,17 @@
 
 In a small office or home office environment it is often quite economical to use a high capacity USB connected portable drive as backup media. They are large in the multiple terabyte range and inexpensive costing less than $500.
 
 With more than one portable drive, off-site backup is feasible.
 
 Grandfathered backups mean users can go back to almost any earlier time and retrieve information as it was then. Essentially it means that today's backup will never overwrite yesterday's backup.
 
-The secret of success is automatic creation and selection of the correct destination folder for the overnight backup. The Python program which nominates the folder name for the date of the backup is called baklabel.
+The secret of success is _automatic_ creation and selection of the correct destination folder for the overnight backup. The Python program which nominates the folder name for the date of the backup is called baklabel.
 
-This program has a number of sensible defaults so it doesn't need tweaking. However tweaking is easy if necessary eg., without tweaking, if the backup kicks off between midnight and 4am it defaults to yesterday's backup label.
+baklabel has a number of sensible defaults so it doesn't need tweaking. Eg., if the backup kicks off between midnight and 4am it defaults to yesterday's backup label.
 
 This "how to" assumes you have a very large USB drive F: and a typical backup load of less than a 24th (4 percent) the size of the drive. Your media should be big enough to permit expected growth in the load over time. There will be up to 24 copies of the backup for all the grandfathering including one manual backup and one saved annual backup.
 
 The following pattern of 23 automatic grandfather folders and one manual folder would normally be entirely adequate because backups only get overwritten periodically rather than frequently.
 
 F:\backups\manual   (most recent manually initiated backup)
 F:\backups\mon      (most recent Monday backup)
@@ -48,15 +46,15 @@
 F:\backups\may      (most recent 31 May backup)
 F:\backups\jun      (most recent 30 June backup)
 F:\backups\jul      (most recent 31 July backup)
 F:\backups\aug      (most recent 31 August backup)
 F:\backups\sep      (most recent 30 September backup)
 F:\backups\oct      (most recent 31 October backup)
 F:\backups\nov      (most recent 30 October backup)
-F:\backups\dec_2010 (31 December 2010 backup)
+F:\backups\dec_2023 (31 December 2023 backup)
 
 
 How to set up Grandfathered backups
 ===================================
 
 - Install Python (see below) and baklabel
 
@@ -76,15 +74,15 @@
 
 Put scripts into the admin folder
 ---------------------------------
 This admin folder will contain backup.py, backup.bat and eventually all the log files written during both scheduled and manual backups. Log files will be named after the above directory names eg., log-wed.txt, log-manual.txt etc.
 
 Install Python
 --------------
-If you don't already have Python 2.x or 3.x on your machine, download and install Python 2.7 from http://www.python.org  It should all work fine with versions earlier than 2.7 and also Python 3.x but that hasn't been tested. There is a vast amount of software available for Python 2.x but not yet a lot for 3.x. Version 2.7 has been officially flagged as being the last 2.x and will be supported for a very long time.
+If you don't already have Python on your machine, download and install it from http://www.python.org.
 
 pip install baklabel
 
 Install a large portable disk drive
 -----------------------------------
 Install a very large removable USB connected drive (eg drive F:) and, staying with the example above, create a root folder for the backups eg., F:\backups
 
@@ -104,15 +102,15 @@
 
 Create a new C:\admin\backup.py file using Notepad (not Word) then copy
 and paste the following few lines (with or without the # lines):
 
 #########################################################
 import baklabel                                         # 1
 baklab = baklabel.Grandad()                             # 2
-baklabcmd = '{backup.bat} {baklab.label()}'             # 3
+baklabcmd = f'{backup.bat} {baklab.label()}'            # 3
 import os                                               # 4
 os.system(baklabcmd)                                    # 5
 #########################################################
 
 Here are some numbered notes on backup.py. Skip them if you have no interest.
 
 1. import baklabel imports the baklabel module installed in the first preparation step and gives this backup.py script direct access to the python code which calculates the correct backup label.
```

### Comparing `baklabel-1.2.0/doc/instructions.txt` & `baklabel-1.2.1/doc/examples.txt`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.0/doc/release_note.txt` & `baklabel-1.2.1/doc/release_note.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 baklabel - see Description below
 ========
 
-Version  Build Who  When/What
-==============================
+Version    Who  When/What
+=========================
 
-ver 1.1.0 2729  md  23 May 2023 - Change from GPL3 to MIT license, change
-                    to pyproject.toml and clean up strings using f-strings
+ver 1.2.1   md  30 May 2023 - Clean up documentation
 
+ver 1.2.0   md  29 May 2023 - Improve guessdate() to resolve ambiguous dates
 
-ver 1.0.3 2729  md  24 Aug 2012 - Code review and tweaks to test importing
-                    to cater for in-house python path adjustments
+ver 1.1.0   md  23 May 2023 - Change from GPL3 to MIT license, change to pyproject.toml
+                and clean up strings using f-strings
 
-ver 1.0.2 2685  md  8 Mar 2011 - Refactored guessdate() out of __main__
-                    to permit string dates as a calling convenience
 
-ver 1.0.1 2671  md  4 Nov 2010 - Minor refactoring and tidying comments
+ver 1.0.3   md  24 Aug 2012 - Code review and tweaks to test importing to cater for
+                in-house python path adjustments
 
-ver 1.0.0 2670  md  3 Nov 2010 - New option to append current year to
-                    any month-end label, not just end-of-year.
+ver 1.0.2   md  8 Mar 2011 - Refactored guessdate() out of __main__ to permit string
+                dates as a calling convenience
 
-ver 0.2.0 2664  md  27 oct 2010 - Help now respects defaults which have
-                    been adjusted in the source code. A new default now
-                    permits adjustment of new_year_month which sets the
-                    end-of-year label to any desired month.
+ver 1.0.1   md  4 Nov 2010 - Minor refactoring and tidying comments
 
-ver 0.1.0b 2646  md 8 oct 2010 - Added -d numeric option for setting
-                    the label to x days ago. Eg., -1 = yesterday. Also
-                    added a time trigger option in the -d switch such
-                    that, for example, -d 3am will produce yesterday's
-                    label if baklabel is called prior to 3am
+ver 1.0.0   md  3 Nov 2010 - New option to append current year to any month-end label,
+                not just end-of-year.
 
-ver 0.0.0a 2640  md 1 jul 2010 - first written
+ver 0.2.0   md  27 oct 2010 - Help now respects defaults which have been adjusted in
+                the source code. A new default now permits adjustment of new_year_month
+                which sets the end-of-year label to any desired month.
+
+ver 0.1.0b   md 8 oct 2010 - Added -d numeric option for setting the label to x days
+                ago. Eg., -1 = yesterday. Also added a time trigger option in the -d
+                switch such that, for example, -d 3am will produce yesterday's label
+                if baklabel is called prior to 3am
+
+ver 0.0.0a   md 1 jul 2010 - first written
 
 
 Description
 ===========
-Baklabel is intended for use in automated scripts to deliver a sensible
-directory path fragment (or label) each day to construct a grandfathered
-local backup destination. It can also be run as a stand-alone utility to
-find the backup label produced for any given date and set of options.
+Baklabel is intended for use in automated scripts to deliver a sensible directory path
+fragment (or label) each day to construct a grandfathered local backup.
+
+Import baklabel.Grandad to produce today's label fragment.
 
-Run  baklabel.py -h  to see command line usage options.
+See test_baklabel.py for examples of how to call Grandad
 
-Call baklabel directly or import it and produce labels from your code.
+It is also a stand-alone utility to find the backup label produced for any given date
+and set of options.
 
-Python 2.7 and 3.x
+python3 baklabel.py -h  to see command line usage and options.
 
-In the docs directory after installing, see release_note.txt for more
-detail on the package, instructions.txt for baklabel output examples and
-backup_howto.txt for a complete example backup script for Windows.
+Python 3.x (Python 2.7 should also work but is no longer tested)
+
+In the doc directory after installing, see release_note.txt for more detail on the
+package, examples.txt for baklabel output examples and backup_howto.txt for a sample
+backup script for Windows.
 
 
 Grandfathered Backups
 =====================
-Properly grandfathered, there needs to be a daily backup to one of 23
-separate tapes, sets of media or local directories on a storage device.
-This complement is made up of 6 weekday backups, 5 week backups and 12
-month backups. 23 backups is quite economical for 12 months coverage.
-
-This provides a stream of untouched backups for at least seven days plus
-the ability to go back four or five Fridays plus having monthly snapshots
-going back for twelve months. This represents real comfort when retrieving
-data which has been compromised at some unknown point in the past.
-
-Each of the regular weekday Sat to Thu backups will be overwritten seven
-days later. However, if an end-of-month occurs on that weekday the month-
-end backup will happen instead and the weekday backup will survive for an
-extra seven days.
-
-Four of the weekly backups get overwritten four weeks later. The fifth
-Friday tape gets overwritten once in a blue moon! Whenever there are five
-Fridays in a month. If end-of-month occurs on a Friday then the month-end
-backup occurs and that Friday backup survives for an extra month or so
-before being overwritten again.
+Properly grandfathered, there needs to be a daily backup to one of 23 separate tapes,
+sets of media or local directories on a storage device. This complement is made up of
+6 weekday backups, 5 week-end backups, 11 month-end backups plus one for year-end.
+
+23 backups is quite economical for 12 months coverage.
 
-Each month-end backup gets overwritten a year later.
+This represents real comfort when retrieving data which has been compromised at some
+unknown point in the past.
 
-Media taken off-site will not be overwritten in future so they should be
-manually labeled with the actual date of the backup carried.
+Each of the regular weekday Sat to Thu backups will be overwritten seven days later.
+However, if an end-of-month occurs on that weekday the month-end backup will happen
+instead and that weekday backup will survive for an extra seven days.
 
-Here are the default labels produced by baklabel for on-site backups:
+Four of the week-end (default is Friday) backups get overwritten four weeks later. The
+fifth Friday backup gets overwritten whenever there are five Fridays in a month.
 
-dec_2010  = 31 Dec 2010
+If end-of-month occurs on a Friday then the month-end backup occurs and that Friday
+backup survives for an extra month or so before being overwritten again.
+
+Each month-end backup gets overwritten in the following year unless archived.
+
+Here are all the default labels produced by baklabel for on-site backups:
+
+dec_2023  = 31 Dec 2023
 nov       = 30 Nov
 oct       = 31 Oct
 sep       = 30 Sep
 aug       = 31 Aug
 jul       = 31 Jul
 jun       = 30 Jun
 may       = 31 May
@@ -101,45 +101,44 @@
  fri_2,   = day 4 of the week
   fri_3,  = day 4 of the week
    fri_4, = day 4 of the week
     fri_5 = day 4 of the week
 sat       = day 5 of the week
 sun       = day 6 of the week
 
-If a backup name is higher in this list than another then it will be
-produced instead of the one below it.
+If a backup name is higher in this list than another then it will be produced instead
+of the one below it.
 
-End-of-year is usually special for archiving reasons. Otherwise it is just
-another month-end. baklabel defaults to appending the year to the December
-backup label. This can be undone with the '-y False' option.
+End-of-year is usually special for archiving reasons. Otherwise it is just another
+month-end. baklabel defaults to appending the year to the December backup label. This
+can be defeated with the '-y False' option.
 
-Also, if the new year begins in July rather than January, for example,
-use the '-n 7' option. This makes June 30 the end-of-year backup rather
-than 31 December. The June label would then be 'jun_2010'.
+If the new year begins in July rather than January, for example, use the '-n 7' option.
+This makes June 30 the end-of-year backup rather than December 31. The June label would
+then be 'jun_2023'.
 
-If you prefer a different day than friday for these week-at-a-time backups
-then edit the WEEKLY_DAY value to represent a different day of the week.
+If you prefer a different day than Friday for these week-end backups there is no
+command line option. You need to edit the baklabel code and change WEEKLY_DAY to
+represent a different day of the week. Use the Python number of the day-of-week.
 
-If you want to live dangerously you could make WEEKLY_DAY greater than or
-equal to 7 and skip saving week-at-a-time backups. Not recommended.
+To defeat week-end backups altogether and make Friday just another day, make WEEKLY_DAY
+greater than or equal to 7. Skipping week-end backups would not be recommended by most
+grandfathers!
 
 
-Source:  Userid is 'public' with no password.
-https://svn.climate.com.au/repos/pysrc/foss/baklabel/distrib/
-
-(That may change to github shortly)
+Source:  https://github.com/mdewhirst/baklabel
 
 Mike Dewhirst
 miked@dewhirst.com.au
 
 
 
-License
-=======
-Copyright (c) 2023 Climate Pty Ltd
+MIT License
+===========
+Copyright (c) 2010-2023 Climate Pty Ltd
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `baklabel-1.2.0/doc/synopsis.txt` & `baklabel-1.2.1/doc/synopsis.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,130 +1,134 @@
 00000000: 0d0a 5379 6e6f 7073 6973 0d0a 3d3d 3d3d  ..Synopsis..====
 00000010: 3d3d 3d3d 0d0a 4261 6b6c 6162 656c 2069  ====..Baklabel i
 00000020: 7320 696e 7465 6e64 6564 2066 6f72 2075  s intended for u
 00000030: 7365 2069 6e20 6175 746f 6d61 7465 6420  se in automated 
 00000040: 7363 7269 7074 7320 746f 2064 656c 6976  scripts to deliv
-00000050: 6572 2061 2073 656e 7369 626c 650d 0a64  er a sensible..d
-00000060: 6972 6563 746f 7279 2070 6174 6820 6672  irectory path fr
+00000050: 6572 2061 2073 656e 7369 626c 6520 6469  er a sensible di
+00000060: 7265 6374 6f72 7920 7061 7468 0d0a 6672  rectory path..fr
 00000070: 6167 6d65 6e74 2028 6f72 206c 6162 656c  agment (or label
 00000080: 2920 6561 6368 2064 6179 2074 6f20 636f  ) each day to co
 00000090: 6e73 7472 7563 7420 6120 6772 616e 6466  nstruct a grandf
-000000a0: 6174 6865 7265 640d 0a6c 6f63 616c 2062  athered..local b
-000000b0: 6163 6b75 7020 6465 7374 696e 6174 696f  ackup destinatio
-000000c0: 6e2e 2049 7420 6361 6e20 616c 736f 2062  n. It can also b
-000000d0: 6520 7275 6e20 6173 2061 2073 7461 6e64  e run as a stand
-000000e0: 2d61 6c6f 6e65 2075 7469 6c69 7479 2074  -alone utility t
-000000f0: 6f0d 0a66 696e 6420 7468 6520 6261 636b  o..find the back
-00000100: 7570 206c 6162 656c 2070 726f 6475 6365  up label produce
-00000110: 6420 666f 7220 616e 7920 6769 7665 6e20  d for any given 
-00000120: 6461 7465 2061 6e64 2073 6574 206f 6620  date and set of 
-00000130: 6f70 7469 6f6e 732e 0d0a 0d0a 5275 6e20  options.....Run 
-00000140: 2062 616b 6c61 6265 6c2e 7079 202d 6820   baklabel.py -h 
-00000150: 2074 6f20 7365 6520 636f 6d6d 616e 6420   to see command 
-00000160: 6c69 6e65 2075 7361 6765 206f 7074 696f  line usage optio
-00000170: 6e73 2e0d 0a0d 0a43 616c 6c20 6261 6b6c  ns.....Call bakl
-00000180: 6162 656c 2064 6972 6563 746c 7920 6f72  abel directly or
-00000190: 2069 6d70 6f72 7420 6974 2061 6e64 2070   import it and p
-000001a0: 726f 6475 6365 206c 6162 656c 7320 6672  roduce labels fr
-000001b0: 6f6d 2079 6f75 7220 636f 6465 2e0d 0a0d  om your code....
-000001c0: 0a50 7974 686f 6e20 322e 3720 616e 6420  .Python 2.7 and 
-000001d0: 332e 780d 0a0d 0a49 6e20 7468 6520 646f  3.x....In the do
-000001e0: 6373 2064 6972 6563 746f 7279 2061 6674  cs directory aft
-000001f0: 6572 2069 6e73 7461 6c6c 696e 672c 2073  er installing, s
-00000200: 6565 2072 656c 6561 7365 5f6e 6f74 652e  ee release_note.
-00000210: 7478 7420 666f 7220 6d6f 7265 0d0a 6465  txt for more..de
-00000220: 7461 696c 206f 6e20 7468 6520 7061 636b  tail on the pack
-00000230: 6167 652c 2069 6e73 7472 7563 7469 6f6e  age, instruction
-00000240: 732e 7478 7420 666f 7220 6261 6b6c 6162  s.txt for baklab
-00000250: 656c 206f 7574 7075 7420 6578 616d 706c  el output exampl
-00000260: 6573 2061 6e64 0d0a 6261 636b 7570 5f68  es and..backup_h
-00000270: 6f77 746f 2e74 7874 2066 6f72 2061 2063  owto.txt for a c
-00000280: 6f6d 706c 6574 6520 6578 616d 706c 6520  omplete example 
-00000290: 6261 636b 7570 2073 6372 6970 7420 666f  backup script fo
-000002a0: 7220 5769 6e64 6f77 732e 0d0a 0d0a 5573  r Windows.....Us
-000002b0: 6167 653a 0d0a 2020 2020 6261 6b6c 6162  age:..    baklab
-000002c0: 656c 2e70 7920 5b4f 7074 696f 6e73 5d0d  el.py [Options].
-000002d0: 0a0d 0a4f 7074 696f 6e73 3a0d 0a20 2020  ...Options:..   
-000002e0: 2057 6974 686f 7574 206f 7074 696f 6e73   Without options
-000002f0: 2c20 7072 6f64 7563 6520 746f 6461 7927  , produce today'
-00000300: 7320 6465 6661 756c 7420 6c61 6265 6c2e  s default label.
-00000310: 2049 6620 7468 6520 6375 7272 656e 7420   If the current 
-00000320: 7469 6d65 2069 730d 0a20 2020 2070 7269  time is..    pri
-00000330: 6f72 2074 6f20 3461 6d20 2873 7769 7463  or to 4am (switc
-00000340: 686f 7665 7220 7469 6d65 2920 7468 656e  hover time) then
-00000350: 2070 726f 6475 6365 2079 6573 7465 7264   produce yesterd
-00000360: 6179 2773 206c 6162 656c 2e0d 0a0d 0a20  ay's label..... 
-00000370: 2020 202d 6420 2864 6566 6175 6c74 2064     -d (default d
-00000380: 6174 6520 6973 2074 6f64 6179 2920 4f72  ate is today) Or
-00000390: 2075 7365 2065 672e 2c20 272d 6420 3230   use eg., '-d 20
-000003a0: 3130 2f33 2f33 3027 206f 7220 272d 6420  10/3/30' or '-d 
-000003b0: 3330 2d33 2d32 3031 3027 0d0a 2020 2020  30-3-2010'..    
-000003c0: 2020 2055 7365 202f 206f 7220 2d20 6173     Use / or - as
-000003d0: 2064 6174 6520 7365 7061 7261 746f 7273   date separators
-000003e0: 2e20 4461 7465 2066 6f72 6d61 7420 6973  . Date format is
-000003f0: 2067 7565 7373 6564 2e20 4d74 682d 6461   guessed. Mth-da
-00000400: 792d 7965 6172 0d0a 2020 2020 2020 206f  y-year..       o
-00000410: 6e6c 7920 776f 726b 7320 6966 2064 6179  nly works if day
-00000420: 203e 2031 322e 0d0a 0d0a 2020 2020 2020   > 12.....      
-00000430: 2055 7365 202d 3120 666f 7220 7965 7374   Use -1 for yest
-00000440: 6572 6461 7927 7320 6c61 6265 6c20 6f72  erday's label or
-00000450: 202d 3720 666f 7220 6c61 7374 2077 6565   -7 for last wee
-00000460: 6b27 7320 6c61 6265 6c2e 2055 7365 202b  k's label. Use +
-00000470: 3220 666f 720d 0a20 2020 2020 2020 6120  2 for..       a 
-00000480: 6c61 6265 6c20 666f 7220 7468 6520 6461  label for the da
-00000490: 7920 6166 7465 7220 746f 6d6f 7272 6f77  y after tomorrow
-000004a0: 2e20 416e 7920 6e75 6d62 6572 2077 696c  . Any number wil
-000004b0: 6c20 6265 2063 6f6d 7075 7465 642e 0d0a  l be computed...
-000004c0: 0d0a 2020 2020 2020 2054 6f20 6164 6a75  ..       To adju
-000004d0: 7374 2074 6865 2073 7769 7463 686f 7665  st the switchove
-000004e0: 7220 7469 6d65 2075 7365 2065 672e 2c27  r time use eg.,'
-000004f0: 2d64 2036 616d 2720 6f72 2027 2d64 2036  -d 6am' or '-d 6
-00000500: 706d 2720 6574 632e 0d0a 0d0a 2020 2020  pm' etc.....    
-00000510: 2d73 2028 6465 6661 756c 7420 6973 2062  -s (default is b
-00000520: 6c61 6e6b 2920 7365 7276 6572 206e 616d  lank) server nam
-00000530: 6520 7573 6564 2074 6f20 7072 6566 6978  e used to prefix
-00000540: 2074 6865 2062 6163 6b75 7020 6c61 6265   the backup labe
-00000550: 6c0d 0a0d 0a20 2020 202d 7920 2864 6566  l....    -y (def
-00000560: 6175 6c74 2069 7320 5472 7565 2920 4170  ault is True) Ap
-00000570: 7065 6e64 2079 6561 7220 746f 2065 6e64  pend year to end
-00000580: 2d6f 662d 7965 6172 206c 6162 656c 2e20  -of-year label. 
-00000590: 4f72 2075 7365 2027 2d79 2046 616c 7365  Or use '-y False
-000005a0: 270d 0a20 2020 2020 2020 6f72 2027 2d79  '..       or '-y
-000005b0: 204e 6f27 2e20 416e 7974 6869 6e67 2065   No'. Anything e
-000005c0: 6c73 6520 6d65 616e 7320 5472 7565 2e0d  lse means True..
-000005d0: 0a0d 0a20 2020 202d 6d20 2864 6566 6175  ...    -m (defau
-000005e0: 6c74 2069 7320 4661 6c73 6529 2041 7070  lt is False) App
-000005f0: 656e 6420 7965 6172 2074 6f20 656e 642d  end year to end-
-00000600: 6f66 2d6d 6f6e 7468 206c 6162 656c 2e20  of-month label. 
-00000610: 4f72 2075 7365 2027 2d6d 2054 7275 6527  Or use '-m True'
-00000620: 0d0a 2020 2020 2020 206f 7220 272d 6d20  ..       or '-m 
-00000630: 5965 7327 2e20 416e 7974 6869 6e67 2065  Yes'. Anything e
-00000640: 6c73 6520 6d65 616e 7320 4661 6c73 652e  lse means False.
-00000650: 0d0a 0d0a 2020 2020 2d6e 2028 6465 6661  ....    -n (defa
-00000660: 756c 7420 6973 2031 2920 4d6f 6e74 6820  ult is 1) Month 
-00000670: 6e75 6d62 6572 2063 6f6d 6d65 6e63 696e  number commencin
-00000680: 6720 7468 6520 6e65 7720 7965 6172 2e20  g the new year. 
-00000690: 4a61 6e75 6172 7920 6973 2031 2e0d 0a0d  January is 1....
-000006a0: 0a20 2020 202d 6520 2864 6566 6175 6c74  .    -e (default
-000006b0: 2069 7320 2762 6c61 6e6b 2729 2065 6e64   is 'blank') end
-000006c0: 2d6f 662d 7965 6172 206c 6162 656c 206f  -of-year label o
-000006d0: 6e6c 7920 6861 7320 616e 2065 6666 6563  nly has an effec
-000006e0: 7420 6f6e 206e 6577 2079 6561 7227 730d  t on new year's.
-000006f0: 0a20 2020 2020 2020 6576 6520 696e 2061  .       eve in a
-00000700: 6e79 2079 6561 722e 2059 6f75 206d 6179  ny year. You may
-00000710: 2070 7265 6665 7220 272d 6520 656f 7927   prefer '-e eoy'
-00000720: 206f 7220 272d 6520 656e 642d 6f66 2d79   or '-e end-of-y
-00000730: 6561 7227 2069 6620 796f 750d 0a20 2020  ear' if you..   
-00000740: 2020 2020 646f 6e27 7420 7761 6e74 2061      don't want a
-00000750: 206c 6162 656c 206c 696b 6520 2764 6563   label like 'dec
-00000760: 5f32 3031 3027 206f 7220 2764 6563 272e  _2010' or 'dec'.
-00000770: 0d0a 0d0a 2020 2020 2d77 2028 6465 6661  ....    -w (defa
-00000780: 756c 7420 6973 2034 2920 4461 7920 6e75  ult is 4) Day nu
-00000790: 6d62 6572 206f 6620 7765 656b 6c79 2062  mber of weekly b
-000007a0: 6163 6b75 7073 2e20 4d6f 6e64 6179 2069  ackups. Monday i
-000007b0: 7320 302c 2053 756e 6461 7920 6973 2036  s 0, Sunday is 6
-000007c0: 0d0a 0d0a 2020 2020 2d68 2028 6f72 202d  ....    -h (or -
-000007d0: 3f29 2073 686f 7773 2074 6869 7320 6865  ?) shows this he
-000007e0: 6c70 2074 6578 7420 616e 6420 7468 6520  lp text and the 
-000007f0: 6465 6661 756c 7420 6c61 6265 6c20 666f  default label fo
-00000800: 7220 746f 6461 7920 2e2e 2e0d 0a20 2020  r today .....   
-00000810: 20                                        
+000000a0: 6174 6865 7265 6420 6c6f 6361 6c20 6261  athered local ba
+000000b0: 636b 7570 2e0d 0a0d 0a49 6d70 6f72 7420  ckup.....Import 
+000000c0: 6261 6b6c 6162 656c 2e47 7261 6e64 6164  baklabel.Grandad
+000000d0: 2074 6f20 7072 6f64 7563 6520 746f 6461   to produce toda
+000000e0: 7927 7320 6c61 6265 6c20 6672 6167 6d65  y's label fragme
+000000f0: 6e74 2e0d 0a0d 0a53 6565 2074 6573 745f  nt.....See test_
+00000100: 6261 6b6c 6162 656c 2e70 7920 666f 7220  baklabel.py for 
+00000110: 6578 616d 706c 6573 206f 6620 686f 7720  examples of how 
+00000120: 746f 2063 616c 6c20 4772 616e 6461 640d  to call Grandad.
+00000130: 0a0d 0a49 7420 6973 2061 6c73 6f20 6120  ...It is also a 
+00000140: 7374 616e 642d 616c 6f6e 6520 7574 696c  stand-alone util
+00000150: 6974 7920 746f 2066 696e 6420 7468 6520  ity to find the 
+00000160: 6261 636b 7570 206c 6162 656c 2070 726f  backup label pro
+00000170: 6475 6365 6420 666f 7220 616e 7920 6769  duced for any gi
+00000180: 7665 6e20 6461 7465 0d0a 616e 6420 7365  ven date..and se
+00000190: 7420 6f66 206f 7074 696f 6e73 2e0d 0a0d  t of options....
+000001a0: 0a70 7974 686f 6e33 2062 616b 6c61 6265  .python3 baklabe
+000001b0: 6c2e 7079 202d 6820 2074 6f20 7365 6520  l.py -h  to see 
+000001c0: 636f 6d6d 616e 6420 6c69 6e65 2075 7361  command line usa
+000001d0: 6765 2061 6e64 206f 7074 696f 6e73 2e0d  ge and options..
+000001e0: 0a0d 0a50 7974 686f 6e20 332e 7820 2850  ...Python 3.x (P
+000001f0: 7974 686f 6e20 322e 3720 7368 6f75 6c64  ython 2.7 should
+00000200: 2061 6c73 6f20 776f 726b 2062 7574 2069   also work but i
+00000210: 7320 6e6f 206c 6f6e 6765 7220 7465 7374  s no longer test
+00000220: 6564 290d 0a0d 0a49 6e20 7468 6520 646f  ed)....In the do
+00000230: 6320 6469 7265 6374 6f72 7920 6166 7465  c directory afte
+00000240: 7220 696e 7374 616c 6c69 6e67 2c20 7365  r installing, se
+00000250: 6520 7265 6c65 6173 655f 6e6f 7465 2e74  e release_note.t
+00000260: 7874 2066 6f72 206d 6f72 6520 6465 7461  xt for more deta
+00000270: 696c 206f 6e20 7468 650d 0a70 6163 6b61  il on the..packa
+00000280: 6765 2c20 6578 616d 706c 6573 2e74 7874  ge, examples.txt
+00000290: 2066 6f72 2062 616b 6c61 6265 6c20 6f75   for baklabel ou
+000002a0: 7470 7574 2065 7861 6d70 6c65 7320 616e  tput examples an
+000002b0: 6420 6261 636b 7570 5f68 6f77 746f 2e74  d backup_howto.t
+000002c0: 7874 2066 6f72 2061 2073 616d 706c 650d  xt for a sample.
+000002d0: 0a62 6163 6b75 7020 7363 7269 7074 2066  .backup script f
+000002e0: 6f72 2057 696e 646f 7773 2e0d 0a0d 0a55  or Windows.....U
+000002f0: 7361 6765 3a0d 0a20 2020 2062 616b 6c61  sage:..    bakla
+00000300: 6265 6c2e 7079 205b 4f70 7469 6f6e 735d  bel.py [Options]
+00000310: 0d0a 0d0a 4f70 7469 6f6e 733a 0d0a 2020  ....Options:..  
+00000320: 2020 5769 7468 6f75 7420 6f70 7469 6f6e    Without option
+00000330: 732c 2070 726f 6475 6365 2074 6f64 6179  s, produce today
+00000340: 2773 2064 6566 6175 6c74 206c 6162 656c  's default label
+00000350: 2e20 4966 2074 6865 2063 7572 7265 6e74  . If the current
+00000360: 2074 696d 6520 6973 0d0a 2020 2020 7072   time is..    pr
+00000370: 696f 7220 746f 2034 616d 2028 7377 6974  ior to 4am (swit
+00000380: 6368 6f76 6572 2074 696d 6529 2074 6865  chover time) the
+00000390: 6e20 7072 6f64 7563 6520 7965 7374 6572  n produce yester
+000003a0: 6461 7927 7320 6c61 6265 6c2e 0d0a 0d0a  day's label.....
+000003b0: 2020 2020 2d64 2028 6465 6661 756c 7420      -d (default 
+000003c0: 6461 7465 2069 7320 746f 6461 7929 204f  date is today) O
+000003d0: 7220 7573 6520 6567 2e2c 2027 2d64 2032  r use eg., '-d 2
+000003e0: 3031 302f 332f 3330 2720 6f72 2027 2d64  010/3/30' or '-d
+000003f0: 2033 302d 332d 3230 3130 270d 0a20 2020   30-3-2010'..   
+00000400: 2020 2020 5573 6520 2f20 6f72 202d 2061      Use / or - a
+00000410: 7320 6461 7465 2073 6570 6172 6174 6f72  s date separator
+00000420: 732e 2044 6174 6520 666f 726d 6174 2069  s. Date format i
+00000430: 7320 6775 6573 7365 642e 204d 7468 2d64  s guessed. Mth-d
+00000440: 6179 2d79 6561 720d 0a20 2020 2020 2020  ay-year..       
+00000450: 6f6e 6c79 2077 6f72 6b73 2069 6620 6461  only works if da
+00000460: 7920 3e20 3132 2e0d 0a0d 0a20 2020 2020  y > 12.....     
+00000470: 2020 5573 6520 2d31 2066 6f72 2079 6573    Use -1 for yes
+00000480: 7465 7264 6179 2773 206c 6162 656c 206f  terday's label o
+00000490: 7220 2d37 2066 6f72 206c 6173 7420 7765  r -7 for last we
+000004a0: 656b 2773 206c 6162 656c 2e20 5573 6520  ek's label. Use 
+000004b0: 2b32 2066 6f72 0d0a 2020 2020 2020 2061  +2 for..       a
+000004c0: 206c 6162 656c 2066 6f72 2074 6865 2064   label for the d
+000004d0: 6179 2061 6674 6572 2074 6f6d 6f72 726f  ay after tomorro
+000004e0: 772e 2041 6e79 206e 756d 6265 7220 7769  w. Any number wi
+000004f0: 6c6c 2062 6520 636f 6d70 7574 6564 2e0d  ll be computed..
+00000500: 0a0d 0a20 2020 2020 2020 546f 2061 646a  ...       To adj
+00000510: 7573 7420 7468 6520 7377 6974 6368 6f76  ust the switchov
+00000520: 6572 2074 696d 6520 7573 6520 6567 2e2c  er time use eg.,
+00000530: 272d 6420 3661 6d27 206f 7220 272d 6420  '-d 6am' or '-d 
+00000540: 3670 6d27 2065 7463 2e0d 0a0d 0a20 2020  6pm' etc.....   
+00000550: 202d 7320 2864 6566 6175 6c74 2069 7320   -s (default is 
+00000560: 626c 616e 6b29 2073 6572 7665 7220 6e61  blank) server na
+00000570: 6d65 2075 7365 6420 746f 2070 7265 6669  me used to prefi
+00000580: 7820 7468 6520 6261 636b 7570 206c 6162  x the backup lab
+00000590: 656c 0d0a 0d0a 2020 2020 2d79 2028 6465  el....    -y (de
+000005a0: 6661 756c 7420 6973 2054 7275 6529 2041  fault is True) A
+000005b0: 7070 656e 6420 7965 6172 2074 6f20 656e  ppend year to en
+000005c0: 642d 6f66 2d79 6561 7220 6c61 6265 6c2e  d-of-year label.
+000005d0: 204f 7220 7573 6520 272d 7920 4661 6c73   Or use '-y Fals
+000005e0: 6527 0d0a 2020 2020 2020 206f 7220 272d  e'..       or '-
+000005f0: 7920 4e6f 272e 2041 6e79 7468 696e 6720  y No'. Anything 
+00000600: 656c 7365 206d 6561 6e73 2054 7275 652e  else means True.
+00000610: 0d0a 0d0a 2020 2020 2d6d 2028 6465 6661  ....    -m (defa
+00000620: 756c 7420 6973 2046 616c 7365 2920 4170  ult is False) Ap
+00000630: 7065 6e64 2079 6561 7220 746f 2065 6e64  pend year to end
+00000640: 2d6f 662d 6d6f 6e74 6820 6c61 6265 6c2e  -of-month label.
+00000650: 204f 7220 7573 6520 272d 6d20 5472 7565   Or use '-m True
+00000660: 270d 0a20 2020 2020 2020 6f72 2027 2d6d  '..       or '-m
+00000670: 2059 6573 272e 2041 6e79 7468 696e 6720   Yes'. Anything 
+00000680: 656c 7365 206d 6561 6e73 2046 616c 7365  else means False
+00000690: 2e0d 0a0d 0a20 2020 202d 6e20 2864 6566  .....    -n (def
+000006a0: 6175 6c74 2069 7320 3129 204d 6f6e 7468  ault is 1) Month
+000006b0: 206e 756d 6265 7220 636f 6d6d 656e 6369   number commenci
+000006c0: 6e67 2074 6865 206e 6577 2079 6561 722e  ng the new year.
+000006d0: 204a 616e 7561 7279 2069 7320 312e 0d0a   January is 1...
+000006e0: 0d0a 2020 2020 2d65 2028 6465 6661 756c  ..    -e (defaul
+000006f0: 7420 6973 2027 626c 616e 6b27 2920 656e  t is 'blank') en
+00000700: 642d 6f66 2d79 6561 7220 6c61 6265 6c20  d-of-year label 
+00000710: 6f6e 6c79 2068 6173 2061 6e20 6566 6665  only has an effe
+00000720: 6374 206f 6e20 6e65 7720 7965 6172 2773  ct on new year's
+00000730: 0d0a 2020 2020 2020 2065 7665 2069 6e20  ..       eve in 
+00000740: 616e 7920 7965 6172 2e20 596f 7520 6d61  any year. You ma
+00000750: 7920 7072 6566 6572 2027 2d65 2065 6f79  y prefer '-e eoy
+00000760: 2720 6f72 2027 2d65 2065 6e64 2d6f 662d  ' or '-e end-of-
+00000770: 7965 6172 2720 6966 2079 6f75 0d0a 2020  year' if you..  
+00000780: 2020 2020 2064 6f6e 2774 2077 616e 7420       don't want 
+00000790: 6120 6c61 6265 6c20 6c69 6b65 2027 6465  a label like 'de
+000007a0: 635f 3230 3130 2720 6f72 2027 6465 6327  c_2010' or 'dec'
+000007b0: 2e0d 0a0d 0a20 2020 202d 7720 2864 6566  .....    -w (def
+000007c0: 6175 6c74 2069 7320 3429 2044 6179 206e  ault is 4) Day n
+000007d0: 756d 6265 7220 6f66 2077 6565 6b6c 7920  umber of weekly 
+000007e0: 6261 636b 7570 732e 204d 6f6e 6461 7920  backups. Monday 
+000007f0: 6973 2030 2c20 5375 6e64 6179 2069 7320  is 0, Sunday is 
+00000800: 360d 0a0d 0a20 2020 202d 6820 286f 7220  6....    -h (or 
+00000810: 2d3f 2920 7368 6f77 7320 7468 6973 2068  -?) shows this h
+00000820: 656c 7020 7465 7874 2061 6e64 2074 6865  elp text and the
+00000830: 2064 6566 6175 6c74 206c 6162 656c 2066   default label f
+00000840: 6f72 2074 6f64 6179 202e 2e2e 0d0a 2020  or today .....  
+00000850: 2020
```

### Comparing `baklabel-1.2.0/src/baklabel/baklabel.py` & `baklabel-1.2.1/src/baklabel/baklabel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2011-2023 Climate Pty Ltd
 longdesc = """
-Baklabel is intended for use in automated scripts to deliver a sensible
-directory path fragment (or label) each day to construct a grandfathered
-local backup destination. It can also be run as a stand-alone utility to
-find the backup label produced for any given date and set of options.
+Baklabel is intended for use in automated scripts to deliver a sensible directory path
+fragment (or label) each day to construct a grandfathered local backup.
 
-Run  baklabel.py -h  to see command line usage options.
+Import baklabel.Grandad to produce today's label fragment.
 
-Call baklabel directly or import it and produce labels from your code.
+See test_baklabel.py for examples of how to call Grandad
 
-Python 2.7 and 3.x
+It is also a stand-alone utility to find the backup label produced for any given date
+and set of options.
 
-In the docs directory after installing, see release_note.txt for more
-detail on the package, instructions.txt for baklabel output examples and
-backup_howto.txt for a complete example backup script for Windows.
+python3 baklabel.py -h  to see command line usage and options.
+
+Python 3.x (Python 2.7 should also work but is no longer tested)
+
+In the doc directory after installing, see release_note.txt for more detail on the
+package, examples.txt for baklabel output examples and backup_howto.txt for a sample
+backup script for Windows.
 """
 
 longerdesc = """
-Properly grandfathered, there needs to be a daily backup to one of 23
-separate tapes, sets of media or local directories on a storage device.
-This complement is made up of 6 weekday backups, 5 week backups and 12
-month backups. 23 backups is quite economical for 12 months coverage.
-
-This provides a stream of untouched backups for at least seven days plus
-the ability to go back four or five Fridays plus having monthly snapshots
-going back for twelve months. This represents real comfort when retrieving
-data which has been compromised at some unknown point in the past.
-"""
+Properly grandfathered, there needs to be a daily backup to one of 23 separate tapes,
+sets of media or local directories on a storage device. This complement is made up of
+6 weekday backups, 5 week-end backups, 11 month-end backups plus one for year-end.
 
-source = """
-Source:  Userid is 'public' with no password.
-https://svn.climate.com.au/repos/pysrc/foss/baklabel/distrib/
+23 backups is quite economical for 12 months coverage.
 
-(That may change to github shortly)
+This represents real comfort when retrieving data which has been compromised at some
+unknown point in the past.
+"""
+
+repo = """
+Source:  https://github.com/mdewhirst/baklabel
 
 Mike Dewhirst
 miked@dewhirst.com.au
 """
 
 relnote = """baklabel - see Description below
 ========
 
-Version  Build Who  When/What
-==============================
+Version    Who  When/What
+=========================
+
+ver 1.2.1   md  30 May 2023 - Clean up documentation
 
 ver 1.2.0   md  29 May 2023 - Improve guessdate() to resolve ambiguous dates
 
 ver 1.1.0   md  23 May 2023 - Change from GPL3 to MIT license, change to pyproject.toml
                 and clean up strings using f-strings
 
 
@@ -75,33 +76,29 @@
 
 
 Description
 ==========={0}
 
 Grandfathered Backups
 ====================={1}
-Each of the regular weekday Sat to Thu backups will be overwritten seven
-days later. However, if an end-of-month occurs on that weekday the month-
-end backup will happen instead and the weekday backup will survive for an
-extra seven days.
+Each of the regular weekday Sat to Thu backups will be overwritten seven days later.
+However, if an end-of-month occurs on that weekday the month-end backup will happen
+instead and that weekday backup will survive for an extra seven days.
 
-Four of the weekly backups get overwritten four weeks later. The fifth
-Friday tape gets overwritten once in a blue moon! Whenever there are five
-Fridays in a month. If end-of-month occurs on a Friday then the month-end
-backup occurs and that Friday backup survives for an extra month or so
-before being overwritten again.
+Four of the week-end (default is Friday) backups get overwritten four weeks later. The
+fifth Friday backup gets overwritten whenever there are five Fridays in a month.
 
-Each month-end backup gets overwritten a year later.
+If end-of-month occurs on a Friday then the month-end backup occurs and that Friday
+backup survives for an extra month or so before being overwritten again.
 
-Media taken off-site will not be overwritten in future so they should be
-manually labeled with the actual date of the backup carried.
+Each month-end backup gets overwritten in the following year unless archived.
 
-Here are the default labels produced by baklabel for on-site backups:
+Here are all the default labels produced by baklabel for on-site backups:
 
-dec_2010  = 31 Dec 2010
+dec_2023  = 31 Dec 2023
 nov       = 30 Nov
 oct       = 31 Oct
 sep       = 30 Sep
 aug       = 31 Aug
 jul       = 31 Jul
 jun       = 30 Jun
 may       = 31 May
@@ -117,37 +114,39 @@
  fri_2,   = day 4 of the week
   fri_3,  = day 4 of the week
    fri_4, = day 4 of the week
     fri_5 = day 4 of the week
 sat       = day 5 of the week
 sun       = day 6 of the week
 
-If a backup name is higher in this list than another then it will be
-produced instead of the one below it.
-
-End-of-year is usually special for archiving reasons. Otherwise it is just
-another month-end. baklabel defaults to appending the year to the December
-backup label. This can be undone with the '-y False' option.
-
-Also, if the new year begins in July rather than January, for example,
-use the '-n 7' option. This makes June 30 the end-of-year backup rather
-than 31 December. The June label would then be 'jun_2010'.
+If a backup name is higher in this list than another then it will be produced instead
+of the one below it.
 
-If you prefer a different day than friday for these week-at-a-time backups
-then edit the WEEKLY_DAY value to represent a different day of the week.
-
-If you want to live dangerously you could make WEEKLY_DAY greater than or
-equal to 7 and skip saving week-at-a-time backups. Not recommended.
+End-of-year is usually special for archiving reasons. Otherwise it is just another
+month-end. baklabel defaults to appending the year to the December backup label. This
+can be defeated with the '-y False' option.
+
+If the new year begins in July rather than January, for example, use the '-n 7' option.
+This makes June 30 the end-of-year backup rather than December 31. The June label would
+then be 'jun_2023'.
+
+If you prefer a different day than Friday for these week-end backups there is no
+command line option. You need to edit the baklabel code and change WEEKLY_DAY to
+represent a different day of the week. Use the Python number of the day-of-week.
+
+To defeat week-end backups altogether and make Friday just another day, make WEEKLY_DAY
+greater than or equal to 7. Skipping week-end backups would not be recommended by most
+grandfathers!
 
 {2}
 
 
-License
-=======
-Copyright (c) 2023 Climate Pty Ltd
+MIT License
+===========
+Copyright (c) 2010-2023 Climate Pty Ltd
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -159,38 +158,37 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
-""".format(longdesc, longerdesc, source)
+""".format(longdesc, longerdesc, repo)
 
 __doc__ = relnote
 
 import argparse
 from datetime import date, datetime
 
 # All upper-case words below from SERVER_PREFIX to SMALLHOURS are intended as
-# program constants. They are actually default values and may be edited at
-# your convenience after a particular installation. Once edited they should
-# be regarded as constants where they appear in the ensuing code.
+# program constants. They are default values and may be edited at your peril
+# should you upgrade baklabel in future.
 
 # prefix all backup labels - perhaps the name of the server being backed up
 SERVER_PREFIX = ''
 
 # end-of-year is Dec 31, new year's eve: NEW_YEAR_MONTH == 1 == January
 NEW_YEAR_MONTH = 1
 
 # end-of-year backup base label could be 'dec' or 'end-of-year' or 'eoy'
 # blank defaults to the usual monthend label, dec if NEW_YEAR_Month == 1
 EOY_LABEL = ''
 
 # append the year to the end-of-year backup name?
-# True returns 'dec_2010' on 31/12/2010, False returns just 'dec'
+# True returns 'dec_2023' on 31/12/2023, False returns just 'dec'
 APPEND_YEAR_TO_EOY_LABEL = True
 
 # True saves end-of-month backups forever, False overwites them each year
 APPEND_YEAR_TO_EOM_LABEL = False
 
 # end of week backup
 # 4 is Friday for the weekly backup (Monday is day 0)
@@ -199,28 +197,34 @@
 
 SMALLHOURS = 4
 # if the backup starts before SMALLHOURS am then use yesterday's label
 # otherwise use today's label
 
 
 def detect_system_date_format():
+    """ Ambiguous dates entered on the command line need to be resolved """
+
     import locale
     system_locale = locale.getlocale()
     if system_locale[0]:
-        example_date = datetime(2023, 5, 29)  # Example date today will suffice
-        locale.setlocale(locale.LC_TIME, system_locale)  # Set the locale explicitly
-        formatted_date = example_date.strftime("%x")  # Get formatted date
-        system_date_format = formatted_date.replace(
+        # Eg., ('Australia', 'utf-8')
+        # Example date today will suffice
+        example_date = datetime(2023, 5, 29)
+        # Set the locale explicitly
+        locale.setlocale(locale.LC_TIME, system_locale)
+        # Get formatted date
+        formatted_date = example_date.strftime("%x")
+        # Replace the known example values so we can disambiguate
+        return formatted_date.replace(
             "2023", "YYYY"
         ).replace(
             "05", "MM"
         ).replace(
             "29", "DD"
         )
-        return system_date_format
     else:
         # Only if no locale is set - possibly needs "MM-DD-YY" but not tested
         return "YYYY-MM-DD"  # Default date format if detection fails
 
 
 def guessdate(dstr, line=None):
     # now conjure/guess a date from a ?-?-? or ?/?/? string
@@ -252,14 +256,19 @@
                     ye = int(bits[fbits.index("YYYY")])
                     mo = int(bits[fbits.index("MM")])
                     da = int(bits[fbits.index("DD")])
         return date(ye, mo, da)
     else:
         raise ValueError('Invalid date format')
 
+
+def readme():
+    return f"{longdesc}\n{longerdesc}\n{repo}\n"
+
+
 class Grandad:
 
     # See __doc__ = synopsis below
     # making -h help reflect the above defaults - only used in synopsis
     svrname = 'blank'
     if not SERVER_PREFIX == '':
         svrname = SERVER_PREFIX
@@ -316,15 +325,14 @@
         new_year_month=NEW_YEAR_MONTH,
         eoy_label=EOY_LABEL,
         append_eoy_year=APPEND_YEAR_TO_EOY_LABEL,
         append_eom_year=APPEND_YEAR_TO_EOM_LABEL,
         weekly_day=WEEKLY_DAY,
         smallhours=SMALLHOURS,
     ):
-
         # increment = -1 means yesterday so hard-code 0 to begin with
         self.increment = 0
         # smallhours = 3 means use yesterday only until 3am - don't care about DST
         self.smallhours = smallhours
         self.backupday = self._confirmday(backupday)
         self.tomorrow = date.fromordinal(self.backupday.toordinal() + 1)
         self.server_prefix = server_prefix
```

### Comparing `baklabel-1.2.0/src/baklabel/test_baklabel.py` & `baklabel-1.2.1/src/baklabel/test_baklabel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,88 +1,13 @@
 import unittest
 import os, sys
 from datetime import date
 from baklabel import Grandad, guessdate
 
 
-class TestGuessdate(unittest.TestCase):
-
-    def test_usa_date_slash(self):
-        dlst = 12, 31, 2023
-        dstr = "/".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
-
-
-    def test_eu_date_slash(self):
-        dlst = 2023, 12, 31
-        dstr = "/".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
-
-
-    def test_au_date_slash(self):
-        dlst = 31, 12, 2023
-        dstr = "/".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
-
-
-    def test_usa_date_ambig_slash(self):
-        dlst = 5, 6, 2023
-        dstr = "/".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr, line=None)), '2023-06-05')
-
-
-    def test_eu_date_ambig_slash(self):
-        dlst = 2023, 6, 5
-        dstr = "/".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
-
-
-    def test_au_date_ambig_slash(self):
-        dlst = 5, 6, 2023
-        dstr = "/".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
-
-
-    def test_usa_date_slash(self):
-        dlst = 12, 31, 2023
-        dstr = "-".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
-
-
-    def test_eu_date(self):
-        dlst = 2023, 12, 31
-        dstr = "-".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
-
-
-    def test_au_date(self):
-        dlst = 31, 12, 2023
-        dstr = "-".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
-
-
-    def test_usa_date_ambig(self):
-        dlst = 5, 6, 2023
-        dstr = "-".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr, line=None)), '2023-06-05')
-
-
-    def test_eu_date_ambig(self):
-        dlst = 2023, 6, 5
-        dstr = "-".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
-
-
-    def test_au_date_ambig(self):
-        dlst = 5, 6, 2023
-        dstr = "-".join(str(item) for item in dlst)
-        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
-
-
-
 class TestBaklabel(unittest.TestCase):
     """
     def __init__(self,
         backupday=date.today(),
         server_prefix=SERVER_PREFIX,
         new_year_month=NEW_YEAR_MONTH,
         eoy_label=EOY_LABEL,
@@ -92,142 +17,123 @@
         smallhours=SMALLHOURS):
     """
 
     def test_new_year_day_eom_year_bad_str(self):
         """ 69 """
         dday = '2040/1'
         try:
-            tsto = Grandad(dday,
-                                    append_eom_year=True)
+            tsto = Grandad(dday, append_eom_year=True)
         except ValueError:
             dday = '2040/1/1'
-            tsto = Grandad(dday,
-                                    append_eom_year=True)
+            tsto = Grandad(dday, append_eom_year=True)
             expected = 'sun'
             result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_monthend_feb_eom_year_str(self):
         """ 68 """
         dday = '2040/2/28'
         expected = 'tue'
-        tsto = Grandad(dday,
-                                append_eom_year=True)
+        tsto = Grandad(dday, append_eom_year=True)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_monthend_feb_leap_year_eom_year_str(self):
         """ 67 """
         dday = '2040/2/29'
         expected = 'feb_2040'
-        tsto = Grandad(dday,
-                                append_eom_year=True)
+        tsto = Grandad(dday, append_eom_year=True)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_eoy_true_eom_false_str(self):
         """ 66 """
         dday = '2040/12/31'
         expected = 'dec_2040'
-        tsto = Grandad(dday,
-                                append_eoy_year=True,
-                                append_eom_year=False)
+        tsto = Grandad(dday, append_eoy_year=True, append_eom_year=False)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_eoy_false_eom_true_str(self):
         """ 65 """
         dday = '2040/12/31'
         expected = 'dec_2040'
-        tsto = Grandad(dday,
-                                append_eoy_year=False,
-                                append_eom_year=True)
+        tsto = Grandad(dday, append_eoy_year=False, append_eom_year=True)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_default_eoy_eom_false_str(self):
         """ 64 """
         dday = '2040/12/31'
         expected = 'dec_2040'
-        tsto = Grandad(dday,
-                                append_eom_year=False)
+        tsto = Grandad(dday, append_eom_year=False)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_forced_eoy_eom_false_str(self):
         """ 63 """
         dday = '2040/12/31'
         expected = 'eoy_2040'
-        tsto = Grandad(dday, eoy_label='eoy',
-                                append_eom_year=False)
+        tsto = Grandad(dday, eoy_label='eoy', append_eom_year=False)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_new_year_day_eom_year(self):
         """ 62 """
         dday = date(2040, 1, 1)
         expected = 'sun'
-        tsto = Grandad(dday,
-                                append_eom_year=True)
+        tsto = Grandad(dday, append_eom_year=True)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_monthend_feb_eom_year(self):
         """ 61 """
         dday = date(2040, 2, 28)
         expected = 'tue'
-        tsto = Grandad(dday,
-                                append_eom_year=True)
+        tsto = Grandad(dday, append_eom_year=True)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_monthend_feb_leap_year_eom_year(self):
         """ 60 """
         dday = date(2040, 2, 29)
         expected = 'feb_2040'
-        tsto = Grandad(dday,
-                                append_eom_year=True)
+        tsto = Grandad(dday, append_eom_year=True)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_eoy_true_eom_false(self):
         """ 59 """
         dday = date(2040, 12, 31)
         expected = 'dec_2040'
-        tsto = Grandad(dday,
-                                append_eoy_year=True,
-                                append_eom_year=False)
+        tsto = Grandad(dday, append_eoy_year=True, append_eom_year=False)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_eoy_false_eom_true(self):
         """ 58 """
         dday = date(2040, 12, 31)
         expected = 'dec_2040'
-        tsto = Grandad(dday,
-                                append_eoy_year=False,
-                                append_eom_year=True)
+        tsto = Grandad(dday, append_eoy_year=False, append_eom_year=True)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_default_eoy_eom_false(self):
         """ 57 """
         dday = date(2040, 12, 31)
         expected = 'dec_2040'
-        tsto = Grandad(dday,
-                                append_eom_year=False)
+        tsto = Grandad(dday, append_eom_year=False)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_forced_eoy_eom_false(self):
         """ 56 """
         dday = date(2040, 12, 31)
         expected = 'eoy_2040'
-        tsto = Grandad(dday, eoy_label='eoy',
-                                append_eom_year=False)
+        tsto = Grandad(dday, eoy_label='eoy', append_eom_year=False)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_monthend_mar_year(self):
         """ 55 """
         dday = date(2040, 3, 31)
         expected = 'mar_2040'
@@ -315,124 +221,111 @@
         expected = expobj.label()
         self.assertEqual(result, expected)
 
     def test_force_no_weekly_day_next_thu_a(self):
         """ 48 """
         dday = date(2040, 3, 8)
         expected = 'a_thu'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=7)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=7)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_force_no_weekly_day_wed_a(self):
         """ 47 """
         dday = date(2040, 3, 7)
         expected = 'a_wed'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=7)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=7)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_force_no_weekly_day_tue_a(self):
         """ 46 """
         dday = date(2040, 3, 6)
         expected = 'a_tue'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=7)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=7)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_force_no_weekly_day_mon_a(self):
         """ 45 """
         dday = date(2040, 3, 5)
         expected = 'a_mon'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=7)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=7)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_force_no_weekly_day_sun_a(self):
         """ 44 """
         dday = date(2040, 3, 4)
         expected = 'a_sun'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=7)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=7)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_force_no_weekly_day_sat_a(self):
         """ 43 """
         dday = date(2040, 3, 3)
         expected = 'a_sat'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=7)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=7)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_force_no_weekly_day_fri_a(self):
         """ 42 """
         dday = date(2040, 3, 2)
         expected = 'a_fri'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=7)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=7)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_force_no_weekly_day_thu_a(self):
         """ 41 """
         dday = date(2040, 3, 1)
         expected = 'a_thu'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=7)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=7)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_force_1st_thu_weekly_day_a(self):
         """ 40 """
         dday = date(2040, 3, 1)
         expected = 'a_thu_1'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=3)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=3)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_force_sun_weekly_day_a(self):
         """ 39 """
         dday = date(2040, 3, 11)
         expected = 'a_sun_2'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=6)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=6)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_monthend_beats_5th_sat_a(self):
         """ 38 """
         dday = date(2040, 3, 31)
         expected = 'a_mar'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=5)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=5)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_force_sat_weekly_day_a(self):
         """ 37 """
         dday = date(2040, 3, 24)
         expected = 'a_sat_4'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=5)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=5)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_force_3rd_thu_weekly_day_a(self):
         """ 36 """
         dday = date(2010, 3, 18)
         expected = 'a_thu_3'
-        tsto = Grandad(dday, server_prefix='a',
-                                weekly_day=3)
+        tsto = Grandad(dday, server_prefix='a', weekly_day=3)
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_new_year_day_a(self):
         """ 35 """
         dday = date(2040, 1, 1)
         expected = 'a_sun'
@@ -464,16 +357,15 @@
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_forced_eoy_a(self):
         """ 31 """
         dday = date(2040, 12, 31)
         expected = 'a_eoy_2040'
-        tsto = Grandad(dday, server_prefix='a',
-                                eoy_label='eoy')
+        tsto = Grandad(dday, server_prefix='a', eoy_label='eoy')
         result = tsto.label()
         self.assertEqual(result, expected)
 
     def test_monthend_mar_a(self):
         """ 30 """
         dday = date(2040, 3, 31)
         expected = 'a_mar'
@@ -709,14 +601,89 @@
         """ 1 """
         dday = date(2040, 3, 30)
         expected = 'fri_5'
         tsto = Grandad(dday)
         result = tsto.label()
         self.assertEqual(result, expected)
 
+
+class TestGuessdate(unittest.TestCase):
+
+    def test_usa_date_slash(self):
+        dlst = 12, 31, 2023
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_eu_date_slash(self):
+        dlst = 2023, 12, 31
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_au_date_slash(self):
+        dlst = 31, 12, 2023
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_usa_date_ambig_slash(self):
+        dlst = 5, 6, 2023
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr, line=None)), '2023-06-05')
+
+
+    def test_eu_date_ambig_slash(self):
+        dlst = 2023, 6, 5
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
+
+
+    def test_au_date_ambig_slash(self):
+        dlst = 5, 6, 2023
+        dstr = "/".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
+
+
+    def test_usa_date_slash(self):
+        dlst = 12, 31, 2023
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_eu_date(self):
+        dlst = 2023, 12, 31
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_au_date(self):
+        dlst = 31, 12, 2023
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-12-31')
+
+
+    def test_usa_date_ambig(self):
+        dlst = 5, 6, 2023
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr, line=None)), '2023-06-05')
+
+
+    def test_eu_date_ambig(self):
+        dlst = 2023, 6, 5
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
+
+
+    def test_au_date_ambig(self):
+        dlst = 5, 6, 2023
+        dstr = "-".join(str(item) for item in dlst)
+        self.assertEqual(str(guessdate(dstr)), '2023-06-05')
+
+
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 
 if __name__ == "__main__":
 
     import sys
```

### Comparing `baklabel-1.2.0/LICENSE` & `baklabel-1.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2023 Climate Pty Ltd
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2023 Climate Pty Ltd
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `baklabel-1.2.0/pyproject.toml` & `baklabel-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baklabel"
-version       = '1.2.0'
+version               = '1.2.1'
 authors = [
   { name="Mike Dewhirst", email="miked@dewhirst.com.au" },
 ]
 description = "Baklabel delivers a daily label fragment for grandfathered backups"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

