# Comparing `tmp/gitautobackup-1.0.1.3.tar.gz` & `tmp/gitautobackup-1.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Soft(withgit)\~Legacy\gitautobackup\dist\.tmp-4ticew1n\gitautobackup-1.0.1.3.tar", last modified: Tue May 30 20:21:26 2023, max compression
+gzip compressed data, was "D:\Soft(withgit)\~Legacy\gitautobackup\dist\.tmp-sgfauh7m\gitautobackup-1.1.0.0.tar", last modified: Wed May 31 20:15:12 2023, max compression
```

## Comparing `gitautobackup-1.0.1.3.tar` & `gitautobackup-1.1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 20:21:26.000000 gitautobackup-1.0.1.3/
--rw-rw-rw-   0        0        0    17098 2023-05-30 17:53:38.000000 gitautobackup-1.0.1.3/LICENSE
--rw-rw-rw-   0        0        0    27921 2023-05-30 20:21:26.000000 gitautobackup-1.0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6268 2023-05-30 18:39:48.000000 gitautobackup-1.0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 20:21:26.000000 gitautobackup-1.0.1.3/gitautobackup.egg-info/
--rw-rw-rw-   0        0        0    27921 2023-05-30 20:21:26.000000 gitautobackup-1.0.1.3/gitautobackup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-30 20:21:26.000000 gitautobackup-1.0.1.3/gitautobackup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 20:21:26.000000 gitautobackup-1.0.1.3/gitautobackup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-30 20:21:26.000000 gitautobackup-1.0.1.3/gitautobackup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2023-05-30 20:21:26.000000 gitautobackup-1.0.1.3/gitautobackup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-30 20:21:26.000000 gitautobackup-1.0.1.3/gitautobackup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 20:19:52.000000 gitautobackup-1.0.1.3/gitautobackup.egg-info/zip-safe
--rw-rw-rw-   0        0        0    16115 2023-05-30 20:17:09.000000 gitautobackup-1.0.1.3/gitautobackup.py
--rw-rw-rw-   0        0        0     2558 2023-05-30 18:39:31.000000 gitautobackup-1.0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 20:21:26.000000 gitautobackup-1.0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 20:15:12.000000 gitautobackup-1.1.0.0/
+-rw-rw-rw-   0        0        0    17098 2023-05-30 17:53:38.000000 gitautobackup-1.1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    44908 2023-05-31 20:15:12.000000 gitautobackup-1.1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6929 2023-05-31 14:45:35.000000 gitautobackup-1.1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 20:15:12.000000 gitautobackup-1.1.0.0/gitautobackup.egg-info/
+-rw-rw-rw-   0        0        0    44908 2023-05-31 20:15:12.000000 gitautobackup-1.1.0.0/gitautobackup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-31 20:15:12.000000 gitautobackup-1.1.0.0/gitautobackup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 20:15:12.000000 gitautobackup-1.1.0.0/gitautobackup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-05-31 20:15:12.000000 gitautobackup-1.1.0.0/gitautobackup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2023-05-31 20:15:12.000000 gitautobackup-1.1.0.0/gitautobackup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 20:15:12.000000 gitautobackup-1.1.0.0/gitautobackup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-31 20:14:49.000000 gitautobackup-1.1.0.0/gitautobackup.egg-info/zip-safe
+-rw-rw-rw-   0        0        0    17024 2023-05-31 15:47:43.000000 gitautobackup-1.1.0.0/gitautobackup.py
+-rw-rw-rw-   0        0        0     2132 2023-05-31 20:12:43.000000 gitautobackup-1.1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 20:15:12.000000 gitautobackup-1.1.0.0/setup.cfg
```

### Comparing `gitautobackup-1.0.1.3/LICENSE` & `gitautobackup-1.1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitautobackup-1.0.1.3/PKG-INFO` & `gitautobackup-1.1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 1.0.1.3
+Version: 1.1.0.0
 Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -378,59 +378,48 @@
           defined by the Mozilla Public License, v. 2.0.
         
 Project-URL: Homepage, https://github.com/MarkusHammer/gitautobackup
 Project-URL: Github, https://github.com/MarkusHammer/gitautobackup
 Project-URL: Issues, https://github.com/MarkusHammer/gitautobackup/issues
 Project-URL: Pull Requests, https://github.com/MarkusHammer/gitautobackup/pulls
 Project-URL: Git, https://github.com/MarkusHammer/gitautobackup.git
-Keywords: backup,git,commit,managment,tool,devtool,small,simple,development,utility
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Typing :: Typed
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development :: Version Control
-Classifier: Topic :: Software Development :: Version Control :: Git
-Classifier: Topic :: System :: Archiving
-Classifier: Topic :: System :: Archiving :: Backup
-Classifier: Topic :: System :: Software Distribution
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: dev
 License-File: LICENSE
 
 # Git Auto Backup Tool
 
 A basic CLI program and python module that allows for quickly making and comming changes to a git repository, along with a few other tools. Use it from the command line or import it as a module, it works both ways!
 
 ## Setup
 
 First off, this script uses the ``GitPython`` module, so ensure that you have a compatable version of git installed on you system so that ``GitPython`` can interface with it properly. For more info look [here](https://github.com/gitpython-developers/GitPython).
 
-If not installed via pip, than the requirements for this script must be installed in the python environment. This script requires the ``git`` python module be available in you python environment in order to run. This can also use the ``argparse`` module optionally to help greatly increase the usability on the command line (and is highly suggested). These can be installed using:
+If not installed via pip, than the requirements for this script must be installed in the python environment. This script requires the ``git`` python module be available in you python environment in order to run. This can also use the ``argparse`` module optionally to help greatly increase the usability on the command line (and is highly suggested), as well as the ``pprint`` module for better formating of verbose outputs. These can be installed using:
 
 ``pip install gitautobackup[cli]``
 
-or if you just want the module without the extra cli overhead:
+or if you just want the module without the extra cli overhead (not suggested):
 
 ``pip install gitautobackup``
 
 If you prefer to have this as a standalone file and are **sure** that you have all dependences satisfied in some way you can also simply clone this repo into your project and import the ``gitautobackup.py`` file locally.
 
+> Please note that if this is the method you use to ensure that the path is specified as if not it will default to the current terminal working directory which if set to the location of the clone of this repository will result in making a commit to this project's clone. I only say this as this is a mistake I have made myself quite a few times.
+
 ## Command Line Interface
 
 Depending on how you set up this file on your system, you can run this module using ``python -m gitautobackup`` if you set it up using pip, or ``python ./gitautobackup.py`` or ``py ./gitautobackup.py`` if you have the gitautobackup file locally.
 
 While this module does not explicitly require the ``argparse`` module, it is **highly** suggested as it help greatly improve the usability and allows acess to more options. If in doubt just install ``argparse`` if you can.
 
+Unlike argparse, ``pprint`` is a purley aesthetic module which is not at all needed other than for more friendly formating of the output of large blocks of text (something only commonly seen when using verbose output).
+
 ### With ``argparse``
 
 This module does not have any required arguments, as everything does have a default behaviour. The most importnant thing to note is that when not supplied with the path of the git repository, it attempts to deduce the location of a git repository (by testing if the directory is able to be loaded as a git repository) from (in this specific order):
 
 1. The console's current working direcory
 2. The directory given in the 0th arg of the command line (aka ``sys.argv[0]``'s lowest directory)
 3. The location of this file itself
@@ -499,7 +488,381 @@
 ## Credits
 
 This project uses the ``pathlib``, ``GitPython`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
 
 While not required, feel free to credit "*Markus Hammer*" (or just "*Markus*") if you find this code or script usefull for whatever you may be doing with it.
 
 **Thanks!**
+
+Mozilla Public License Version 2.0
+==================================
+
+1. Definitions
+--------------
+
+1.1. "Contributor"
+    means each individual or legal entity that creates, contributes to
+    the creation of, or owns Covered Software.
+
+1.2. "Contributor Version"
+    means the combination of the Contributions of others (if any) used
+    by a Contributor and that particular Contributor's Contribution.
+
+1.3. "Contribution"
+    means Covered Software of a particular Contributor.
+
+1.4. "Covered Software"
+    means Source Code Form to which the initial Contributor has attached
+    the notice in Exhibit A, the Executable Form of such Source Code
+    Form, and Modifications of such Source Code Form, in each case
+    including portions thereof.
+
+1.5. "Incompatible With Secondary Licenses"
+    means
+
+    (a) that the initial Contributor has attached the notice described
+        in Exhibit B to the Covered Software; or
+
+    (b) that the Covered Software was made available under the terms of
+        version 1.1 or earlier of the License, but not also under the
+        terms of a Secondary License.
+
+1.6. "Executable Form"
+    means any form of the work other than Source Code Form.
+
+1.7. "Larger Work"
+    means a work that combines Covered Software with other material, in
+    a separate file or files, that is not Covered Software.
+
+1.8. "License"
+    means this document.
+
+1.9. "Licensable"
+    means having the right to grant, to the maximum extent possible,
+    whether at the time of the initial grant or subsequently, any and
+    all of the rights conveyed by this License.
+
+1.10. "Modifications"
+    means any of the following:
+
+    (a) any file in Source Code Form that results from an addition to,
+        deletion from, or modification of the contents of Covered
+        Software; or
+
+    (b) any new file in Source Code Form that contains any Covered
+        Software.
+
+1.11. "Patent Claims" of a Contributor
+    means any patent claim(s), including without limitation, method,
+    process, and apparatus claims, in any patent Licensable by such
+    Contributor that would be infringed, but for the grant of the
+    License, by the making, using, selling, offering for sale, having
+    made, import, or transfer of either its Contributions or its
+    Contributor Version.
+
+1.12. "Secondary License"
+    means either the GNU General Public License, Version 2.0, the GNU
+    Lesser General Public License, Version 2.1, the GNU Affero General
+    Public License, Version 3.0, or any later versions of those
+    licenses.
+
+1.13. "Source Code Form"
+    means the form of the work preferred for making modifications.
+
+1.14. "You" (or "Your")
+    means an individual or a legal entity exercising rights under this
+    License. For legal entities, "You" includes any entity that
+    controls, is controlled by, or is under common control with You. For
+    purposes of this definition, "control" means (a) the power, direct
+    or indirect, to cause the direction or management of such entity,
+    whether by contract or otherwise, or (b) ownership of more than
+    fifty percent (50%) of the outstanding shares or beneficial
+    ownership of such entity.
+
+2. License Grants and Conditions
+--------------------------------
+
+2.1. Grants
+
+Each Contributor hereby grants You a world-wide, royalty-free,
+non-exclusive license:
+
+(a) under intellectual property rights (other than patent or trademark)
+    Licensable by such Contributor to use, reproduce, make available,
+    modify, display, perform, distribute, and otherwise exploit its
+    Contributions, either on an unmodified basis, with Modifications, or
+    as part of a Larger Work; and
+
+(b) under Patent Claims of such Contributor to make, use, sell, offer
+    for sale, have made, import, and otherwise transfer either its
+    Contributions or its Contributor Version.
+
+2.2. Effective Date
+
+The licenses granted in Section 2.1 with respect to any Contribution
+become effective for each Contribution on the date the Contributor first
+distributes such Contribution.
+
+2.3. Limitations on Grant Scope
+
+The licenses granted in this Section 2 are the only rights granted under
+this License. No additional rights or licenses will be implied from the
+distribution or licensing of Covered Software under this License.
+Notwithstanding Section 2.1(b) above, no patent license is granted by a
+Contributor:
+
+(a) for any code that a Contributor has removed from Covered Software;
+    or
+
+(b) for infringements caused by: (i) Your and any other third party's
+    modifications of Covered Software, or (ii) the combination of its
+    Contributions with other software (except as part of its Contributor
+    Version); or
+
+(c) under Patent Claims infringed by Covered Software in the absence of
+    its Contributions.
+
+This License does not grant any rights in the trademarks, service marks,
+or logos of any Contributor (except as may be necessary to comply with
+the notice requirements in Section 3.4).
+
+2.4. Subsequent Licenses
+
+No Contributor makes additional grants as a result of Your choice to
+distribute the Covered Software under a subsequent version of this
+License (see Section 10.2) or under the terms of a Secondary License (if
+permitted under the terms of Section 3.3).
+
+2.5. Representation
+
+Each Contributor represents that the Contributor believes its
+Contributions are its original creation(s) or it has sufficient rights
+to grant the rights to its Contributions conveyed by this License.
+
+2.6. Fair Use
+
+This License is not intended to limit any rights You have under
+applicable copyright doctrines of fair use, fair dealing, or other
+equivalents.
+
+2.7. Conditions
+
+Sections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted
+in Section 2.1.
+
+3. Responsibilities
+-------------------
+
+3.1. Distribution of Source Form
+
+All distribution of Covered Software in Source Code Form, including any
+Modifications that You create or to which You contribute, must be under
+the terms of this License. You must inform recipients that the Source
+Code Form of the Covered Software is governed by the terms of this
+License, and how they can obtain a copy of this License. You may not
+attempt to alter or restrict the recipients' rights in the Source Code
+Form.
+
+3.2. Distribution of Executable Form
+
+If You distribute Covered Software in Executable Form then:
+
+(a) such Covered Software must also be made available in Source Code
+    Form, as described in Section 3.1, and You must inform recipients of
+    the Executable Form how they can obtain a copy of such Source Code
+    Form by reasonable means in a timely manner, at a charge no more
+    than the cost of distribution to the recipient; and
+
+(b) You may distribute such Executable Form under the terms of this
+    License, or sublicense it under different terms, provided that the
+    license for the Executable Form does not attempt to limit or alter
+    the recipients' rights in the Source Code Form under this License.
+
+3.3. Distribution of a Larger Work
+
+You may create and distribute a Larger Work under terms of Your choice,
+provided that You also comply with the requirements of this License for
+the Covered Software. If the Larger Work is a combination of Covered
+Software with a work governed by one or more Secondary Licenses, and the
+Covered Software is not Incompatible With Secondary Licenses, this
+License permits You to additionally distribute such Covered Software
+under the terms of such Secondary License(s), so that the recipient of
+the Larger Work may, at their option, further distribute the Covered
+Software under the terms of either this License or such Secondary
+License(s).
+
+3.4. Notices
+
+You may not remove or alter the substance of any license notices
+(including copyright notices, patent notices, disclaimers of warranty,
+or limitations of liability) contained within the Source Code Form of
+the Covered Software, except that You may alter any license notices to
+the extent required to remedy known factual inaccuracies.
+
+3.5. Application of Additional Terms
+
+You may choose to offer, and to charge a fee for, warranty, support,
+indemnity or liability obligations to one or more recipients of Covered
+Software. However, You may do so only on Your own behalf, and not on
+behalf of any Contributor. You must make it absolutely clear that any
+such warranty, support, indemnity, or liability obligation is offered by
+You alone, and You hereby agree to indemnify every Contributor for any
+liability incurred by such Contributor as a result of warranty, support,
+indemnity or liability terms You offer. You may include additional
+disclaimers of warranty and limitations of liability specific to any
+jurisdiction.
+
+4. Inability to Comply Due to Statute or Regulation
+---------------------------------------------------
+
+If it is impossible for You to comply with any of the terms of this
+License with respect to some or all of the Covered Software due to
+statute, judicial order, or regulation then You must: (a) comply with
+the terms of this License to the maximum extent possible; and (b)
+describe the limitations and the code they affect. Such description must
+be placed in a text file included with all distributions of the Covered
+Software under this License. Except to the extent prohibited by statute
+or regulation, such description must be sufficiently detailed for a
+recipient of ordinary skill to be able to understand it.
+
+5. Termination
+--------------
+
+5.1. The rights granted under this License will terminate automatically
+if You fail to comply with any of its terms. However, if You become
+compliant, then the rights granted under this License from a particular
+Contributor are reinstated (a) provisionally, unless and until such
+Contributor explicitly and finally terminates Your grants, and (b) on an
+ongoing basis, if such Contributor fails to notify You of the
+non-compliance by some reasonable means prior to 60 days after You have
+come back into compliance. Moreover, Your grants from a particular
+Contributor are reinstated on an ongoing basis if such Contributor
+notifies You of the non-compliance by some reasonable means, this is the
+first time You have received notice of non-compliance with this License
+from such Contributor, and You become compliant prior to 30 days after
+Your receipt of the notice.
+
+5.2. If You initiate litigation against any entity by asserting a patent
+infringement claim (excluding declaratory judgment actions,
+counter-claims, and cross-claims) alleging that a Contributor Version
+directly or indirectly infringes any patent, then the rights granted to
+You by any and all Contributors for the Covered Software under Section
+2.1 of this License shall terminate.
+
+5.3. In the event of termination under Sections 5.1 or 5.2 above, all
+end user license agreements (excluding distributors and resellers) which
+have been validly granted by You or Your distributors under this License
+prior to termination shall survive termination.
+
+************************************************************************
+*                                                                      *
+*  6. Disclaimer of Warranty                                           *
+*  -------------------------                                           *
+*                                                                      *
+*  Covered Software is provided under this License on an "as is"       *
+*  basis, without warranty of any kind, either expressed, implied, or  *
+*  statutory, including, without limitation, warranties that the       *
+*  Covered Software is free of defects, merchantable, fit for a        *
+*  particular purpose or non-infringing. The entire risk as to the     *
+*  quality and performance of the Covered Software is with You.        *
+*  Should any Covered Software prove defective in any respect, You     *
+*  (not any Contributor) assume the cost of any necessary servicing,   *
+*  repair, or correction. This disclaimer of warranty constitutes an   *
+*  essential part of this License. No use of any Covered Software is   *
+*  authorized under this License except under this disclaimer.         *
+*                                                                      *
+************************************************************************
+
+************************************************************************
+*                                                                      *
+*  7. Limitation of Liability                                          *
+*  --------------------------                                          *
+*                                                                      *
+*  Under no circumstances and under no legal theory, whether tort      *
+*  (including negligence), contract, or otherwise, shall any           *
+*  Contributor, or anyone who distributes Covered Software as          *
+*  permitted above, be liable to You for any direct, indirect,         *
+*  special, incidental, or consequential damages of any character      *
+*  including, without limitation, damages for lost profits, loss of    *
+*  goodwill, work stoppage, computer failure or malfunction, or any    *
+*  and all other commercial damages or losses, even if such party      *
+*  shall have been informed of the possibility of such damages. This   *
+*  limitation of liability shall not apply to liability for death or   *
+*  personal injury resulting from such party's negligence to the       *
+*  extent applicable law prohibits such limitation. Some               *
+*  jurisdictions do not allow the exclusion or limitation of           *
+*  incidental or consequential damages, so this exclusion and          *
+*  limitation may not apply to You.                                    *
+*                                                                      *
+************************************************************************
+
+8. Litigation
+-------------
+
+Any litigation relating to this License may be brought only in the
+courts of a jurisdiction where the defendant maintains its principal
+place of business and such litigation shall be governed by laws of that
+jurisdiction, without reference to its conflict-of-law provisions.
+Nothing in this Section shall prevent a party's ability to bring
+cross-claims or counter-claims.
+
+9. Miscellaneous
+----------------
+
+This License represents the complete agreement concerning the subject
+matter hereof. If any provision of this License is held to be
+unenforceable, such provision shall be reformed only to the extent
+necessary to make it enforceable. Any law or regulation which provides
+that the language of a contract shall be construed against the drafter
+shall not be used to construe this License against a Contributor.
+
+10. Versions of the License
+---------------------------
+
+10.1. New Versions
+
+Mozilla Foundation is the license steward. Except as provided in Section
+10.3, no one other than the license steward has the right to modify or
+publish new versions of this License. Each version will be given a
+distinguishing version number.
+
+10.2. Effect of New Versions
+
+You may distribute the Covered Software under the terms of the version
+of the License under which You originally received the Covered Software,
+or under the terms of any subsequent version published by the license
+steward.
+
+10.3. Modified Versions
+
+If you create software not governed by this License, and you want to
+create a new license for such software, you may create and use a
+modified version of this License if you rename the license and remove
+any references to the name of the license steward (except to note that
+such modified license differs from this License).
+
+10.4. Distributing Source Code Form that is Incompatible With Secondary
+Licenses
+
+If You choose to distribute Source Code Form that is Incompatible With
+Secondary Licenses under the terms of this version of the License, the
+notice described in Exhibit B of this License must be attached.
+
+Exhibit A - Source Code Form License Notice
+-------------------------------------------
+
+  This Source Code Form is subject to the terms of the Mozilla Public
+  License, v. 2.0. If a copy of the MPL was not distributed with this
+  file, You can obtain one at http://mozilla.org/MPL/2.0/.
+
+If it is not possible or desirable to put the notice in a particular
+file, then You may include the notice in a location (such as a LICENSE
+file in a relevant directory) where a recipient would be likely to look
+for such a notice.
+
+You may add additional accurate notices of copyright ownership.
+
+Exhibit B - "Incompatible With Secondary Licenses" Notice
+---------------------------------------------------------
+
+  This Source Code Form is "Incompatible With Secondary Licenses", as
+  defined by the Mozilla Public License, v. 2.0.
```

### Comparing `gitautobackup-1.0.1.3/README.md` & `gitautobackup-1.1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,34 @@
 
 A basic CLI program and python module that allows for quickly making and comming changes to a git repository, along with a few other tools. Use it from the command line or import it as a module, it works both ways!
 
 ## Setup
 
 First off, this script uses the ``GitPython`` module, so ensure that you have a compatable version of git installed on you system so that ``GitPython`` can interface with it properly. For more info look [here](https://github.com/gitpython-developers/GitPython).
 
-If not installed via pip, than the requirements for this script must be installed in the python environment. This script requires the ``git`` python module be available in you python environment in order to run. This can also use the ``argparse`` module optionally to help greatly increase the usability on the command line (and is highly suggested). These can be installed using:
+If not installed via pip, than the requirements for this script must be installed in the python environment. This script requires the ``git`` python module be available in you python environment in order to run. This can also use the ``argparse`` module optionally to help greatly increase the usability on the command line (and is highly suggested), as well as the ``pprint`` module for better formating of verbose outputs. These can be installed using:
 
 ``pip install gitautobackup[cli]``
 
-or if you just want the module without the extra cli overhead:
+or if you just want the module without the extra cli overhead (not suggested):
 
 ``pip install gitautobackup``
 
 If you prefer to have this as a standalone file and are **sure** that you have all dependences satisfied in some way you can also simply clone this repo into your project and import the ``gitautobackup.py`` file locally.
 
+> Please note that if this is the method you use to ensure that the path is specified as if not it will default to the current terminal working directory which if set to the location of the clone of this repository will result in making a commit to this project's clone. I only say this as this is a mistake I have made myself quite a few times.
+
 ## Command Line Interface
 
 Depending on how you set up this file on your system, you can run this module using ``python -m gitautobackup`` if you set it up using pip, or ``python ./gitautobackup.py`` or ``py ./gitautobackup.py`` if you have the gitautobackup file locally.
 
 While this module does not explicitly require the ``argparse`` module, it is **highly** suggested as it help greatly improve the usability and allows acess to more options. If in doubt just install ``argparse`` if you can.
 
+Unlike argparse, ``pprint`` is a purley aesthetic module which is not at all needed other than for more friendly formating of the output of large blocks of text (something only commonly seen when using verbose output).
+
 ### With ``argparse``
 
 This module does not have any required arguments, as everything does have a default behaviour. The most importnant thing to note is that when not supplied with the path of the git repository, it attempts to deduce the location of a git repository (by testing if the directory is able to be loaded as a git repository) from (in this specific order):
 
 1. The console's current working direcory
 2. The directory given in the 0th arg of the command line (aka ``sys.argv[0]``'s lowest directory)
 3. The location of this file itself
```

### Comparing `gitautobackup-1.0.1.3/gitautobackup.egg-info/PKG-INFO` & `gitautobackup-1.1.0.0/gitautobackup.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 1.0.1.3
+Version: 1.1.0.0
 Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -378,59 +378,48 @@
           defined by the Mozilla Public License, v. 2.0.
         
 Project-URL: Homepage, https://github.com/MarkusHammer/gitautobackup
 Project-URL: Github, https://github.com/MarkusHammer/gitautobackup
 Project-URL: Issues, https://github.com/MarkusHammer/gitautobackup/issues
 Project-URL: Pull Requests, https://github.com/MarkusHammer/gitautobackup/pulls
 Project-URL: Git, https://github.com/MarkusHammer/gitautobackup.git
-Keywords: backup,git,commit,managment,tool,devtool,small,simple,development,utility
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Typing :: Typed
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development :: Version Control
-Classifier: Topic :: Software Development :: Version Control :: Git
-Classifier: Topic :: System :: Archiving
-Classifier: Topic :: System :: Archiving :: Backup
-Classifier: Topic :: System :: Software Distribution
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: dev
 License-File: LICENSE
 
 # Git Auto Backup Tool
 
 A basic CLI program and python module that allows for quickly making and comming changes to a git repository, along with a few other tools. Use it from the command line or import it as a module, it works both ways!
 
 ## Setup
 
 First off, this script uses the ``GitPython`` module, so ensure that you have a compatable version of git installed on you system so that ``GitPython`` can interface with it properly. For more info look [here](https://github.com/gitpython-developers/GitPython).
 
-If not installed via pip, than the requirements for this script must be installed in the python environment. This script requires the ``git`` python module be available in you python environment in order to run. This can also use the ``argparse`` module optionally to help greatly increase the usability on the command line (and is highly suggested). These can be installed using:
+If not installed via pip, than the requirements for this script must be installed in the python environment. This script requires the ``git`` python module be available in you python environment in order to run. This can also use the ``argparse`` module optionally to help greatly increase the usability on the command line (and is highly suggested), as well as the ``pprint`` module for better formating of verbose outputs. These can be installed using:
 
 ``pip install gitautobackup[cli]``
 
-or if you just want the module without the extra cli overhead:
+or if you just want the module without the extra cli overhead (not suggested):
 
 ``pip install gitautobackup``
 
 If you prefer to have this as a standalone file and are **sure** that you have all dependences satisfied in some way you can also simply clone this repo into your project and import the ``gitautobackup.py`` file locally.
 
+> Please note that if this is the method you use to ensure that the path is specified as if not it will default to the current terminal working directory which if set to the location of the clone of this repository will result in making a commit to this project's clone. I only say this as this is a mistake I have made myself quite a few times.
+
 ## Command Line Interface
 
 Depending on how you set up this file on your system, you can run this module using ``python -m gitautobackup`` if you set it up using pip, or ``python ./gitautobackup.py`` or ``py ./gitautobackup.py`` if you have the gitautobackup file locally.
 
 While this module does not explicitly require the ``argparse`` module, it is **highly** suggested as it help greatly improve the usability and allows acess to more options. If in doubt just install ``argparse`` if you can.
 
+Unlike argparse, ``pprint`` is a purley aesthetic module which is not at all needed other than for more friendly formating of the output of large blocks of text (something only commonly seen when using verbose output).
+
 ### With ``argparse``
 
 This module does not have any required arguments, as everything does have a default behaviour. The most importnant thing to note is that when not supplied with the path of the git repository, it attempts to deduce the location of a git repository (by testing if the directory is able to be loaded as a git repository) from (in this specific order):
 
 1. The console's current working direcory
 2. The directory given in the 0th arg of the command line (aka ``sys.argv[0]``'s lowest directory)
 3. The location of this file itself
@@ -499,7 +488,381 @@
 ## Credits
 
 This project uses the ``pathlib``, ``GitPython`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
 
 While not required, feel free to credit "*Markus Hammer*" (or just "*Markus*") if you find this code or script usefull for whatever you may be doing with it.
 
 **Thanks!**
+
+Mozilla Public License Version 2.0
+==================================
+
+1. Definitions
+--------------
+
+1.1. "Contributor"
+    means each individual or legal entity that creates, contributes to
+    the creation of, or owns Covered Software.
+
+1.2. "Contributor Version"
+    means the combination of the Contributions of others (if any) used
+    by a Contributor and that particular Contributor's Contribution.
+
+1.3. "Contribution"
+    means Covered Software of a particular Contributor.
+
+1.4. "Covered Software"
+    means Source Code Form to which the initial Contributor has attached
+    the notice in Exhibit A, the Executable Form of such Source Code
+    Form, and Modifications of such Source Code Form, in each case
+    including portions thereof.
+
+1.5. "Incompatible With Secondary Licenses"
+    means
+
+    (a) that the initial Contributor has attached the notice described
+        in Exhibit B to the Covered Software; or
+
+    (b) that the Covered Software was made available under the terms of
+        version 1.1 or earlier of the License, but not also under the
+        terms of a Secondary License.
+
+1.6. "Executable Form"
+    means any form of the work other than Source Code Form.
+
+1.7. "Larger Work"
+    means a work that combines Covered Software with other material, in
+    a separate file or files, that is not Covered Software.
+
+1.8. "License"
+    means this document.
+
+1.9. "Licensable"
+    means having the right to grant, to the maximum extent possible,
+    whether at the time of the initial grant or subsequently, any and
+    all of the rights conveyed by this License.
+
+1.10. "Modifications"
+    means any of the following:
+
+    (a) any file in Source Code Form that results from an addition to,
+        deletion from, or modification of the contents of Covered
+        Software; or
+
+    (b) any new file in Source Code Form that contains any Covered
+        Software.
+
+1.11. "Patent Claims" of a Contributor
+    means any patent claim(s), including without limitation, method,
+    process, and apparatus claims, in any patent Licensable by such
+    Contributor that would be infringed, but for the grant of the
+    License, by the making, using, selling, offering for sale, having
+    made, import, or transfer of either its Contributions or its
+    Contributor Version.
+
+1.12. "Secondary License"
+    means either the GNU General Public License, Version 2.0, the GNU
+    Lesser General Public License, Version 2.1, the GNU Affero General
+    Public License, Version 3.0, or any later versions of those
+    licenses.
+
+1.13. "Source Code Form"
+    means the form of the work preferred for making modifications.
+
+1.14. "You" (or "Your")
+    means an individual or a legal entity exercising rights under this
+    License. For legal entities, "You" includes any entity that
+    controls, is controlled by, or is under common control with You. For
+    purposes of this definition, "control" means (a) the power, direct
+    or indirect, to cause the direction or management of such entity,
+    whether by contract or otherwise, or (b) ownership of more than
+    fifty percent (50%) of the outstanding shares or beneficial
+    ownership of such entity.
+
+2. License Grants and Conditions
+--------------------------------
+
+2.1. Grants
+
+Each Contributor hereby grants You a world-wide, royalty-free,
+non-exclusive license:
+
+(a) under intellectual property rights (other than patent or trademark)
+    Licensable by such Contributor to use, reproduce, make available,
+    modify, display, perform, distribute, and otherwise exploit its
+    Contributions, either on an unmodified basis, with Modifications, or
+    as part of a Larger Work; and
+
+(b) under Patent Claims of such Contributor to make, use, sell, offer
+    for sale, have made, import, and otherwise transfer either its
+    Contributions or its Contributor Version.
+
+2.2. Effective Date
+
+The licenses granted in Section 2.1 with respect to any Contribution
+become effective for each Contribution on the date the Contributor first
+distributes such Contribution.
+
+2.3. Limitations on Grant Scope
+
+The licenses granted in this Section 2 are the only rights granted under
+this License. No additional rights or licenses will be implied from the
+distribution or licensing of Covered Software under this License.
+Notwithstanding Section 2.1(b) above, no patent license is granted by a
+Contributor:
+
+(a) for any code that a Contributor has removed from Covered Software;
+    or
+
+(b) for infringements caused by: (i) Your and any other third party's
+    modifications of Covered Software, or (ii) the combination of its
+    Contributions with other software (except as part of its Contributor
+    Version); or
+
+(c) under Patent Claims infringed by Covered Software in the absence of
+    its Contributions.
+
+This License does not grant any rights in the trademarks, service marks,
+or logos of any Contributor (except as may be necessary to comply with
+the notice requirements in Section 3.4).
+
+2.4. Subsequent Licenses
+
+No Contributor makes additional grants as a result of Your choice to
+distribute the Covered Software under a subsequent version of this
+License (see Section 10.2) or under the terms of a Secondary License (if
+permitted under the terms of Section 3.3).
+
+2.5. Representation
+
+Each Contributor represents that the Contributor believes its
+Contributions are its original creation(s) or it has sufficient rights
+to grant the rights to its Contributions conveyed by this License.
+
+2.6. Fair Use
+
+This License is not intended to limit any rights You have under
+applicable copyright doctrines of fair use, fair dealing, or other
+equivalents.
+
+2.7. Conditions
+
+Sections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted
+in Section 2.1.
+
+3. Responsibilities
+-------------------
+
+3.1. Distribution of Source Form
+
+All distribution of Covered Software in Source Code Form, including any
+Modifications that You create or to which You contribute, must be under
+the terms of this License. You must inform recipients that the Source
+Code Form of the Covered Software is governed by the terms of this
+License, and how they can obtain a copy of this License. You may not
+attempt to alter or restrict the recipients' rights in the Source Code
+Form.
+
+3.2. Distribution of Executable Form
+
+If You distribute Covered Software in Executable Form then:
+
+(a) such Covered Software must also be made available in Source Code
+    Form, as described in Section 3.1, and You must inform recipients of
+    the Executable Form how they can obtain a copy of such Source Code
+    Form by reasonable means in a timely manner, at a charge no more
+    than the cost of distribution to the recipient; and
+
+(b) You may distribute such Executable Form under the terms of this
+    License, or sublicense it under different terms, provided that the
+    license for the Executable Form does not attempt to limit or alter
+    the recipients' rights in the Source Code Form under this License.
+
+3.3. Distribution of a Larger Work
+
+You may create and distribute a Larger Work under terms of Your choice,
+provided that You also comply with the requirements of this License for
+the Covered Software. If the Larger Work is a combination of Covered
+Software with a work governed by one or more Secondary Licenses, and the
+Covered Software is not Incompatible With Secondary Licenses, this
+License permits You to additionally distribute such Covered Software
+under the terms of such Secondary License(s), so that the recipient of
+the Larger Work may, at their option, further distribute the Covered
+Software under the terms of either this License or such Secondary
+License(s).
+
+3.4. Notices
+
+You may not remove or alter the substance of any license notices
+(including copyright notices, patent notices, disclaimers of warranty,
+or limitations of liability) contained within the Source Code Form of
+the Covered Software, except that You may alter any license notices to
+the extent required to remedy known factual inaccuracies.
+
+3.5. Application of Additional Terms
+
+You may choose to offer, and to charge a fee for, warranty, support,
+indemnity or liability obligations to one or more recipients of Covered
+Software. However, You may do so only on Your own behalf, and not on
+behalf of any Contributor. You must make it absolutely clear that any
+such warranty, support, indemnity, or liability obligation is offered by
+You alone, and You hereby agree to indemnify every Contributor for any
+liability incurred by such Contributor as a result of warranty, support,
+indemnity or liability terms You offer. You may include additional
+disclaimers of warranty and limitations of liability specific to any
+jurisdiction.
+
+4. Inability to Comply Due to Statute or Regulation
+---------------------------------------------------
+
+If it is impossible for You to comply with any of the terms of this
+License with respect to some or all of the Covered Software due to
+statute, judicial order, or regulation then You must: (a) comply with
+the terms of this License to the maximum extent possible; and (b)
+describe the limitations and the code they affect. Such description must
+be placed in a text file included with all distributions of the Covered
+Software under this License. Except to the extent prohibited by statute
+or regulation, such description must be sufficiently detailed for a
+recipient of ordinary skill to be able to understand it.
+
+5. Termination
+--------------
+
+5.1. The rights granted under this License will terminate automatically
+if You fail to comply with any of its terms. However, if You become
+compliant, then the rights granted under this License from a particular
+Contributor are reinstated (a) provisionally, unless and until such
+Contributor explicitly and finally terminates Your grants, and (b) on an
+ongoing basis, if such Contributor fails to notify You of the
+non-compliance by some reasonable means prior to 60 days after You have
+come back into compliance. Moreover, Your grants from a particular
+Contributor are reinstated on an ongoing basis if such Contributor
+notifies You of the non-compliance by some reasonable means, this is the
+first time You have received notice of non-compliance with this License
+from such Contributor, and You become compliant prior to 30 days after
+Your receipt of the notice.
+
+5.2. If You initiate litigation against any entity by asserting a patent
+infringement claim (excluding declaratory judgment actions,
+counter-claims, and cross-claims) alleging that a Contributor Version
+directly or indirectly infringes any patent, then the rights granted to
+You by any and all Contributors for the Covered Software under Section
+2.1 of this License shall terminate.
+
+5.3. In the event of termination under Sections 5.1 or 5.2 above, all
+end user license agreements (excluding distributors and resellers) which
+have been validly granted by You or Your distributors under this License
+prior to termination shall survive termination.
+
+************************************************************************
+*                                                                      *
+*  6. Disclaimer of Warranty                                           *
+*  -------------------------                                           *
+*                                                                      *
+*  Covered Software is provided under this License on an "as is"       *
+*  basis, without warranty of any kind, either expressed, implied, or  *
+*  statutory, including, without limitation, warranties that the       *
+*  Covered Software is free of defects, merchantable, fit for a        *
+*  particular purpose or non-infringing. The entire risk as to the     *
+*  quality and performance of the Covered Software is with You.        *
+*  Should any Covered Software prove defective in any respect, You     *
+*  (not any Contributor) assume the cost of any necessary servicing,   *
+*  repair, or correction. This disclaimer of warranty constitutes an   *
+*  essential part of this License. No use of any Covered Software is   *
+*  authorized under this License except under this disclaimer.         *
+*                                                                      *
+************************************************************************
+
+************************************************************************
+*                                                                      *
+*  7. Limitation of Liability                                          *
+*  --------------------------                                          *
+*                                                                      *
+*  Under no circumstances and under no legal theory, whether tort      *
+*  (including negligence), contract, or otherwise, shall any           *
+*  Contributor, or anyone who distributes Covered Software as          *
+*  permitted above, be liable to You for any direct, indirect,         *
+*  special, incidental, or consequential damages of any character      *
+*  including, without limitation, damages for lost profits, loss of    *
+*  goodwill, work stoppage, computer failure or malfunction, or any    *
+*  and all other commercial damages or losses, even if such party      *
+*  shall have been informed of the possibility of such damages. This   *
+*  limitation of liability shall not apply to liability for death or   *
+*  personal injury resulting from such party's negligence to the       *
+*  extent applicable law prohibits such limitation. Some               *
+*  jurisdictions do not allow the exclusion or limitation of           *
+*  incidental or consequential damages, so this exclusion and          *
+*  limitation may not apply to You.                                    *
+*                                                                      *
+************************************************************************
+
+8. Litigation
+-------------
+
+Any litigation relating to this License may be brought only in the
+courts of a jurisdiction where the defendant maintains its principal
+place of business and such litigation shall be governed by laws of that
+jurisdiction, without reference to its conflict-of-law provisions.
+Nothing in this Section shall prevent a party's ability to bring
+cross-claims or counter-claims.
+
+9. Miscellaneous
+----------------
+
+This License represents the complete agreement concerning the subject
+matter hereof. If any provision of this License is held to be
+unenforceable, such provision shall be reformed only to the extent
+necessary to make it enforceable. Any law or regulation which provides
+that the language of a contract shall be construed against the drafter
+shall not be used to construe this License against a Contributor.
+
+10. Versions of the License
+---------------------------
+
+10.1. New Versions
+
+Mozilla Foundation is the license steward. Except as provided in Section
+10.3, no one other than the license steward has the right to modify or
+publish new versions of this License. Each version will be given a
+distinguishing version number.
+
+10.2. Effect of New Versions
+
+You may distribute the Covered Software under the terms of the version
+of the License under which You originally received the Covered Software,
+or under the terms of any subsequent version published by the license
+steward.
+
+10.3. Modified Versions
+
+If you create software not governed by this License, and you want to
+create a new license for such software, you may create and use a
+modified version of this License if you rename the license and remove
+any references to the name of the license steward (except to note that
+such modified license differs from this License).
+
+10.4. Distributing Source Code Form that is Incompatible With Secondary
+Licenses
+
+If You choose to distribute Source Code Form that is Incompatible With
+Secondary Licenses under the terms of this version of the License, the
+notice described in Exhibit B of this License must be attached.
+
+Exhibit A - Source Code Form License Notice
+-------------------------------------------
+
+  This Source Code Form is subject to the terms of the Mozilla Public
+  License, v. 2.0. If a copy of the MPL was not distributed with this
+  file, You can obtain one at http://mozilla.org/MPL/2.0/.
+
+If it is not possible or desirable to put the notice in a particular
+file, then You may include the notice in a location (such as a LICENSE
+file in a relevant directory) where a recipient would be likely to look
+for such a notice.
+
+You may add additional accurate notices of copyright ownership.
+
+Exhibit B - "Incompatible With Secondary Licenses" Notice
+---------------------------------------------------------
+
+  This Source Code Form is "Incompatible With Secondary Licenses", as
+  defined by the Mozilla Public License, v. 2.0.
```

### Comparing `gitautobackup-1.0.1.3/gitautobackup.py` & `gitautobackup-1.1.0.0/gitautobackup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,34 +10,23 @@
 
     See the github repo for more info!
     
     This project is on github here:
     https://github.com/MarkusHammer/gitautobackup
 '''
 
-# I mean I know its good pratice but I do not care for reformating all
-#  my docstrings and making the file less readable just so it fits on smaller screens.
-# No its not a run on sentince problem I can stop anytime I want damn it!
-# pylint: disable=C0301
-
-#Disable the warnings for importing out of the top level,
-# as this is used to import modules only when needed by certian functions
-# pylint: disable=C0415
-
-
-
 from pathlib import Path
-from git import Repo, InvalidGitRepositoryError
+from git import Repo, InvalidGitRepositoryError, GitCommandNotFound, NoSuchPathError, RepositoryDirtyError
 
 try:
     from typing import Union
 except ImportError:
     from typing_extensions import Union
 
-__version__ = "1.0.1.3"
+__version__ = "1.1.0.0"
 
 def path_hunt_dir(path: Union[Path, str, None]) -> Union['Path', None]:
     """_summary_
 
     Args:
         path (Union[Path,str,None]): The path to search for the parent directory of. If this is set to None the return value will always also be None
 
@@ -65,31 +54,31 @@
         return path
 
 
 def assert_repo(path: Union[Path, str, None], allow_bare: bool = False):
     """Raises various exceptions to test if a path is or is not a git repo. This function does not return a value, use is_repo instead if you want that.
 
     Args:
-        path (Union[Path,str,None]): The path to assert is a repository. Always raises FileNotFoundError when set to None.
+        path (Union[Path,str,None]): The path to assert is a repository. Always raises NoSuchPathError when set to None.
         allow_bare (bool, optional): Don't raise InvalidGitRepositoryError if the repository is bare. Defaults to False.
 
     Raises:
         NOTE: This may not be a comprehensive list of all possible exceptions raised, as pathlib or git may raise various other exceptions as well, however what is stated below is the behaviour explicitly defined in raise statements.
         InvalidGitRepositoryError: Raised when the folder could not be opened as a git repo, if the path couldn't possibly be a git repo (if its not a directory and does not end with ".git"), or if it can be opened but it is a bare repo and allow_bare is False.
-        FileNotFoundError: Raised when the path is None or doesn't exist on the system.
+        NoSuchPathError: Raised when the path is None or doesn't exist on the system.
     """
 
     if path is None:
-        raise FileNotFoundError()
+        raise NoSuchPathError()
 
     if not isinstance(path, Path):
         path = Path(path)
 
     if not path.exists():
-        raise FileNotFoundError()
+        raise NoSuchPathError()
 
     if not (path.is_dir() or str(path).endswith(".git")):
         raise InvalidGitRepositoryError()
 
     with Repo(path) as repo:
         if (not allow_bare) and repo.bare:
             raise InvalidGitRepositoryError()
@@ -105,15 +94,15 @@
     Returns:
         bool: Weather or not the path given is a git repository.
     """
 
     retval = True
     try:
         assert_repo(path, allow_bare)
-    except (InvalidGitRepositoryError, FileNotFoundError, PermissionError):
+    except (InvalidGitRepositoryError, NoSuchPathError, PermissionError):
         retval = False
     return retval
 
 
 def default_commit_name(nodatetime: bool = False) -> str:
     """Returns the default commit name, generated based on if the system has the datetime module accessable and if its allowed.
 
@@ -167,29 +156,34 @@
             possiblepath = path_hunt_dir(__file__)
             if possiblepath is not None and possiblepath.exists():
                 return possiblepath
 
     return None
 
 
-def auto_git_backup(repo_path: Union[Path, None] = None, commit_message: Union[str, None] = None, further_guess_paths: bool = False, verbose: bool = True, force_commit: bool = False, force_compress: Union[bool, None] = None) -> bool:
+def auto_git_backup(repo_path: Union[Path, None] = None,
+                    commit_message: Union[str, None] = None,
+                    further_guess_paths: bool = False, verbose: bool = True,
+                    force_commit: bool = False,
+                    force_compress: Union[bool, None] = None
+                    ) -> bool:
     """_summary_
 
     Args:
         repo_path (Union[Path,None], optional): The path of the target git repository. If set to None and further_guess_paths is set there will be an attempts to determine this using ```get_default_file_location()```. Defaults to None.
         commit_message (Union[str,None], optional): The message of the commit being made. If None this will be automatically generated using ```default_commit_name()```. Defaults to None.
         further_guess_paths (bool, optional): If the path is set to none, should there be attempt to automatically guess the relevant path using ```get_default_file_location()```. Defaults to False.
         verbose (bool, optional): SHould this function print out non error related messages? Defaults to True.
         force_commit (bool, optional): Should a commit be made even if there is nothing to be committed? Defaults to False.
         force_compress (Union[bool, None], optional): Should (or shouldn't) the database be compressed despite it possibly being beneficial. True forces the database to be compressed, False forces the databest to not be compressed, and None allows for this to be automatically determined by git instead. Defaults to None.
 
     Raises:
         NOTE: This may not be a comprehensive list of all possible exceptions raised, as pathlib or git may raise various other exceptions as well, however what is stated below is the behaviour explicitly defined in raise statements.
         InvalidGitRepositoryError: Raised when the folder could not be opened as a git repo, if the path couldn't possibly be a git repo (if its not a directory and does not end with ".git"), or if it can be opened but it is a bare repo and allow_bare is False.
-        FileNotFoundError: Raised when the path doesn't exist on the system.
+        NoSuchPathError: Raised when the path doesn't exist on the system.
 
     Returns:
         bool: Weather or not a commit was made.
     """
 
     made_a_backup: bool = False
 
@@ -206,15 +200,15 @@
         repo_path = get_default_file_location()
 
     if repo_path is None:
         raise InvalidGitRepositoryError()
 
     repo_path = Path(repo_path)
     if not repo_path.exists():
-        raise FileNotFoundError()
+        raise NoSuchPathError()
     while not is_repo(repo_path) and len(repo_path.parents) > 0:
         repo_path = repo_path.parent
     assert_repo(repo_path)
 
     if verbose:
         print(f"Opening path as repo: {repo_path} {'and forcing a commit' if force_commit else ''}...")
     with Repo(repo_path) as repo:
@@ -228,33 +222,35 @@
 
             if verbose:
                 pprint(repo.git.status("-s"))
 
             cmd_args = []
             if force_commit:
                 cmd_args.append("--allow-empty")
+            if verbose:
+                cmd_args.append("--verbose")
             msg = repo.git.commit(cmd_args, m=commit_message)
             if verbose and msg != "":
                 pprint(msg)
 
         if force_compress is None or force_compress is True:
             cmd_args = []
             if force_compress is None:
                 cmd_args.append("--auto")
             msg = repo.git.gc(cmd_args)
             if verbose and msg != "":
                 pprint(msg)
 
-    # TODO LONGTERM git reflog expire can it also be a feature?
-
     return made_a_backup
 
 
 def main(*args, prog_arg: Union[str, None] = None) -> bool:
-    """A function that run the main entry point for the cli interface of the program. This allows for you to use this as you would normally via the cli but still import this as a module. Please not however that argv is only intended for the cli arguments and not for the name of the script running this, thats what the optional prog_arg argument is intended for.
+    """A function that when used as a module acts as the main entry point of the program. This allows for you to use this as you would normally via the cli but still import this as a module.
+    Please note however that argv is only intended for the cli arguments and not for the name of the script running this, thats what the optional prog_arg argument is intended for.
+    Also note that this function does not handle exceptions unlike how the cli turns these into user friendly messages. This is intended as the user of a module will most likely find these exceptions usefull.
 
     Args:
         *args (Tuple[None]): The arguments form the command line, sans the one with the name of this program (what the sys module's argv puts in the [0]th spot), thats what prog_arg is for.
         prog_arg (Union[str, None], optional): This is used for what is traditionally used as the [0]th member if argv, the name of this program as it was called in the command line. THis is however, completely optional. Defaults to None.
 
     Returns:
         bool: weather or not a backup was made by ```auto_git_backup```
@@ -357,12 +353,33 @@
     if args.verbose:
         print("Making auto backup")
 
     return auto_git_backup(path, commit_message=message, further_guess_paths=further_guess_paths, verbose=verbose, force_commit=force_commit, force_compress=force_compress)
 
 
 def __main__():
+    if __name__ != "__main__":
+        raise RuntimeError("This module's __main__() function is not to be run outside of the module itself. Please use main() for this purpose")
+
     from sys import (exit as end, argv)
-    end(main(argv[1:], prog_arg=argv[0]))
+
+    scode = -1
+
+    try:
+        scode = 0 if main(argv[1:], prog_arg=argv[0]) else 1
+    except GitCommandNotFound:
+        print("Your system is not set up properly for use with the GitPython module. Please refer to it's documentation for setting it up before running this script.")
+    except (NoSuchPathError, FileNotFoundError, PermissionError):
+        print("The given path does not exist on this system or could not be accessed by this user.")
+        scode = -2
+    except InvalidGitRepositoryError:
+        print("The folder given is not a git repo, or is bare.")
+        scode = -3
+    except RepositoryDirtyError:
+        print("The repository already has some changes that could end up being overwritten. Please Handle these first before running this.")
+        scode = -4
+
+    end(scode)
+
 
 if __name__ == "__main__":
     __main__()
```

### Comparing `gitautobackup-1.0.1.3/pyproject.toml` & `gitautobackup-1.1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,45 @@
-#python -m pip install pip-tools validate-pyproject[all] build twine
-#validate-pyproject pyproject.toml
-#pip-compile pyproject.toml
-#python -m build
-#twine upload dist/* -u USERNAME -p PASSWORD --verbose # add -r gitautobackup when updating
-
 #pyproject.toml for gitautobackup python module
 #THX https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#entry-points
 #THX https://pypi.org/project/validate-pyproject/
 
-[build-system]
-requires = ["setuptools>=61.0.0"]
-build-backend = "setuptools.build_meta"
-
 [project]
-name = "gitautobackup"
-dependencies = ["pathlib", "GitPython", "typing-extensions;python_version<'3.8'"]
-requires-python = ">=3.0"
-
-#fullname = "Git Auto Backup Tool"
-dynamic = ["version", "readme"]
-description = "A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools"
-authors = [{ name = "Markus Hammer", email = "107761433+MarkusHammer@users.noreply.github.com" }]
-license = { file = "LICENSE" }
-classifiers = [
-    "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
-    "Development Status :: 5 - Production/Stable",
-    "Environment :: Console",
-    "Intended Audience :: Developers",
-    "Typing :: Typed",
-    "Natural Language :: English",
-    "Topic :: Software Development :: Version Control",
-    "Topic :: Software Development :: Version Control :: Git",
-    "Topic :: System :: Archiving",
-    "Topic :: System :: Archiving :: Backup",
-    "Topic :: System :: Software Distribution",
-    "Topic :: Utilities",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3"
-]
-keywords = [
-    "backup",
-    "git", 
-    "commit",
-    "managment",
-    "tool",
-    "devtool",
-    "small",
-    "simple",
-    "development",
-    "utility"
-]
+    dynamic = ["version", "readme"]
+    name = "gitautobackup"
+    #fullname = "Git Auto Backup Tool"
+    description = "A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools"
+    authors = [{ name = "Markus Hammer", email = "107761433+MarkusHammer@users.noreply.github.com" }]
+    license = { file = "LICENSE" }
+    dependencies = ["pathlib", "GitPython", "typing-extensions;python_version<'3.8'"]
+    requires-python = ">=3.0"
+    [project.optional-dependencies]
+        cli = ["argparse", "pprint"]
+        dev = ["setuptools>=64.0.0", "pip-tools", "validate-pyproject[all]", "build", "twine",]
+    [project.scripts] 
+        gitautobackup = "gitautobackup:__main__"
+        gitbackup = "gitautobackup:__main__"
+    [project.urls]
+        Homepage = "https://github.com/MarkusHammer/gitautobackup"
+        Github  = "https://github.com/MarkusHammer/gitautobackup"
+        Issues = "https://github.com/MarkusHammer/gitautobackup/issues"
+        "Pull Requests" = "https://github.com/MarkusHammer/gitautobackup/pulls"
+        Git = "https://github.com/MarkusHammer/gitautobackup.git"
 
-[tool.setuptools.dynamic]
-version = {attr = "gitautobackup.__version__"}
-readme = {file = ["README.md"], content-type = "text/markdown"}
-
-[project.optional-dependencies]
-cli = ["argparse"]
-dev = ["setuptools>=61.0.0"]
-
-[project.urls]
-Homepage = "https://github.com/MarkusHammer/gitautobackup"
-Github  = "https://github.com/MarkusHammer/gitautobackup"
-Issues = "https://github.com/MarkusHammer/gitautobackup/issues"
-"Pull Requests" = "https://github.com/MarkusHammer/gitautobackup/pulls"
-Git = "https://github.com/MarkusHammer/gitautobackup.git"
-
-[project.scripts]
-gitautobackup = "gitautobackup:__main__"
-#autobackup = "gitautobackup:__main__"
+[build-system]
+    requires = ["setuptools>=64.0.0"]
+    build-backend = "setuptools.build_meta"
+    
+    ### python -m pip install pip-tools validate-pyproject[all] build twine setuptools>=64.0.0
+    ### validate-pyproject pyproject.toml
+    ### pip-compile pyproject.toml
+    ### python -m build
+    ### twine upload dist/* -u USERNAME -p PASSWORD --verbose
 
 [tool.setuptools]
-zip-safe = true
+    zip-safe = true
+    [tool.setuptools.dynamic]
+        version = {attr = "gitautobackup.__version__"}
+        readme = {file = ["README.md", "LICENSE"], content-type = "text/markdown"}
+
+[tool.pylint."MESSAGES CONTROL"]
+    disable = "C0301, C0415"
+    # Disables the warnings for importing out of the top level and long lines
```

