# Comparing `tmp/ayon-python-api-0.1.9.tar.gz` & `tmp/ayon-python-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-0.1.9.tar", last modified: Fri Jan 27 20:30:24 2023, max compression
+gzip compressed data, was "ayon-python-api-0.2.0.tar", last modified: Wed May 31 08:28:29 2023, max compression
```

## Comparing `ayon-python-api-0.1.9.tar` & `ayon-python-api-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-01-27 20:30:24.903319 ayon-python-api-0.1.9/
--rw-rw-rw-   0        0        0    11558 2022-04-28 15:40:50.000000 ayon-python-api-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     1877 2023-01-27 20:30:24.902459 ayon-python-api-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1233 2023-01-10 17:48:41.000000 ayon-python-api-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-01-27 20:30:24.889407 ayon-python-api-0.1.9/ayon_api/
--rw-rw-rw-   0        0        0     4253 2023-01-27 20:18:18.000000 ayon-python-api-0.1.9/ayon_api/__init__.py
--rw-rw-rw-   0        0        0     1397 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/constants.py
--rw-rw-rw-   0        0        0    52144 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/entity_hub.py
--rw-rw-rw-   0        0        0     2992 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/events.py
--rw-rw-rw-   0        0        0     2576 2023-01-20 15:39:24.000000 ayon-python-api-0.1.9/ayon_api/exceptions.py
--rw-rw-rw-   0        0        0    24216 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/graphql.py
--rw-rw-rw-   0        0        0    11497 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/graphql_queries.py
--rw-rw-rw-   0        0        0    23308 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/operations.py
--rw-rw-rw-   0        0        0    92141 2023-01-27 20:18:18.000000 ayon-python-api-0.1.9/ayon_api/server.py
--rw-rw-rw-   0        0        0    16725 2023-01-27 20:18:18.000000 ayon-python-api-0.1.9/ayon_api/server_api.py
--rw-rw-rw-   0        0        0     7075 2023-01-18 15:06:41.000000 ayon-python-api-0.1.9/ayon_api/thumbnails.py
--rw-rw-rw-   0        0        0    11553 2023-01-20 15:39:24.000000 ayon-python-api-0.1.9/ayon_api/utils.py
--rw-rw-rw-   0        0        0       74 2023-01-27 20:26:14.000000 ayon-python-api-0.1.9/ayon_api/version.py
-drwxrwxrwx   0        0        0        0 2023-01-27 20:30:24.901553 ayon-python-api-0.1.9/ayon_python_api.egg-info/
--rw-rw-rw-   0        0        0     1877 2023-01-27 20:30:24.000000 ayon-python-api-0.1.9/ayon_python_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-01-27 20:30:24.000000 ayon-python-api-0.1.9/ayon_python_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-27 20:30:24.000000 ayon-python-api-0.1.9/ayon_python_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-01-27 20:30:24.000000 ayon-python-api-0.1.9/ayon_python_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-27 20:30:24.000000 ayon-python-api-0.1.9/ayon_python_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      387 2023-01-27 20:28:07.000000 ayon-python-api-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-27 20:30:24.903319 ayon-python-api-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1197 2023-01-27 20:26:06.000000 ayon-python-api-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:28:29.524663 ayon-python-api-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-31 08:28:29.524663 ayon-python-api-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:28:29.520663 ayon-python-api-0.2.0/ayon_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56730 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/entity_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161889 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:28:29.524663 ayon-python-api-0.2.0/ayon_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-31 08:28:29.000000 ayon-python-api-0.2.0/ayon_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-31 08:28:29.000000 ayon-python-api-0.2.0/ayon_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:28:29.000000 ayon-python-api-0.2.0/ayon_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 08:28:29.000000 ayon-python-api-0.2.0/ayon_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 08:28:29.000000 ayon-python-api-0.2.0/ayon_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 08:28:29.524663 ayon-python-api-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/setup.py
```

### Comparing `ayon-python-api-0.1.9/LICENSE` & `ayon-python-api-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `ayon-python-api-0.1.9/PKG-INFO` & `ayon-python-api-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,80 @@
-Metadata-Version: 2.1
-Name: ayon-python-api
-Version: 0.1.9
-Summary: AYON Python API
-Home-page: https://github.com/ynput/ayon-python-api
-Author: ynput.io
-Author-email: info@ynput.io
-License: Apache License (2.0)
-Description: # AYON server API
-        Python client for connection server. Client must be (at least for some time) Python 2 compatible because will be used in DCC that are "older".
-        
-        Client should support connection to server with raw REST functions and prepared functionality for work with entities. Must not contain only functionality that can be used with core server functionality.
-        
-        
-        ## TODOs
-        - Current implementation contains prepared functions for entity queries which is not using full potential of OpenPype server but is MongoDB compatible.
-            - only functions related to v4 should stay at that place and v3 compatible functions should be moved
-        - Missing settings getter
-        - Missing CRUD operations for entities (Only read is possible)
-        - More clear what is difference in `ServerAPIBase` and `ServerAPI`
-            - `ServerAPI` was added primarily for desktop app which handle login and logout in a different way so the class should be maybe removed and `ServerAPIBase` should be renamed to `ServerAPI`
-            - find more suitable names of classes
-            - find more suitable name of objects (right now is used `connection` or `conn`)
-        - Add folder and task changes to operations
-          - Entity hub should use operations to update folders and tasks 
-Keywords: AYON,ynput,OpenPype,vfx
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: ayon-python-api
+Version: 0.2.0
+Summary: AYON Python API
+Home-page: https://github.com/ynput/ayon-python-api
+Author: ynput.io
+Author-email: info@ynput.io
+License: Apache License (2.0)
+Keywords: AYON,ynput,OpenPype,vfx
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AYON server API
+Python client for connection server. Client must be (at least for some time) Python 2 compatible because will be used in DCC that are "older".
+
+AYON Python api should support connection to server with raw REST functions and prepared functionality for work with entities. Must not contain only functionality that can be used with core server functionality.
+
+Module support singleton connection which is using `AYON_SERVER_URL` and `AYON_API_KEY` environment variables as source for connection. The singleton connection is using `ServerAPI` object. There can be created multiple connection to different server at one time, for that purpose use `ServerAPIBase` object.
+
+## Install
+AYON python api is available on PyPi:
+
+    pip install ayon-python-api
+
+For development purposes you may follow [build](#build-wheel) guide to build and install custom wheels.
+
+
+## Cloning the repository
+Repository does not have submodules or special cases. Clone is simple as:
+
+    git clone git@github.com:ynput/ayon-python-api.git
+
+
+## Build wheel
+For wheel build is required a `wheel` module from PyPi:
+
+    pip install wheel
+
+Open terminal and change directory to ayon-python-api repository and build wheel:
+
+    cd <REPOSITORY ROOT>/ayon-python-api
+    python setup.py sdist bdist_wheel   
+    
+
+Once finished a wheel should be created in `./dist/ayon_python_api-<VERSION>-py3-none-any`.
+
+---
+
+### Wheel installation
+The wheel file can be used to install using pip:
+
+    pip install <REPOSITORY ROOT>/dist/ayon_python_api-<VERSION>-py3-none-any
+
+If pip complain that `ayon-python-api` is already installed just uninstall existing one first:
+    
+    pip uninstall ayon-python-api
+
+
+## TODOs
+- Find more suitable name of `ServerAPI` objects (right now is used `con` or `connection`)
+- Add all available CRUD operation on entities using REST
+- Add folder and task changes to operations
+- Enhance entity hub
+  - Missing docstrings in EntityHub -> especially entity arguments are missing
+  - Better order of arguments for entity classes
+    - Move entity hub to first place
+    - Skip those which are invalid for the entity and fake it for base or remove it from base
+  - Entity hub should use operations session to do changes
+  - Entity hub could also handle 'subset', 'version' and 'representation' entities
+  - Missing 'statuses' on project
+  - Missing 'status' on folders
+  - Missing assignees on tasks
+  - Pass docstrings and arguments definitions from `ServerAPI` methods to global functions
+- Split `ServerAPI` into smaller chunks (somehow), the class has 4k+ lines of code
+- Add .pyi stub for ServerAPI 
+- Missing websockets connection
```

### Comparing `ayon-python-api-0.1.9/ayon_api/entity_hub.py` & `ayon-python-api-0.2.0/ayon_api/entity_hub.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1667 +1,1819 @@
-import copy
-import collections
-from abc import ABCMeta, abstractmethod, abstractproperty
-
-import six
-from .server_api import get_server_api_connection
-from .utils import create_entity_id, convert_entity_id
-
-UNKNOWN_VALUE = object()
-PROJECT_PARENT_ID = object()
-_NOT_SET = object()
-
-
-class EntityHub(object):
-    """Helper to create, update or remove entities in project.
-
-    The hub is a guide to operation with folder entities and update of project.
-    Project entity must already exist on server (can be only updated).
-
-    Object is caching entities queried from server. They won't be required once
-    they were queried, so it is recommended to create new hub or clear cache
-    frequently.
-
-    Todos:
-        Listen to server events about entity changes to be able update already
-            queried entities.
-
-    Args:
-        project_name (str): Name of project where changes will happen.
-        connection (ServerAPIBase): Connection to server with logged user.
-        allow_data_changes (bool): This option gives ability to change 'data'
-            key on entities. This is not recommended as 'data' may be use for
-            secure information and would also slow down server queries. Content
-            of 'data' key can't be received only GraphQl.
-    """
-
-    def __init__(
-        self, project_name, connection=None, allow_data_changes=False
-    ):
-        if not connection:
-            connection = get_server_api_connection()
-        self._connection = connection
-
-        self._project_name = project_name
-        self._entities_by_id = {}
-        self._entities_by_parent_id = collections.defaultdict(list)
-        self._project_entity = UNKNOWN_VALUE
-
-        self._allow_data_changes = allow_data_changes
-
-        self._path_reset_queue = None
-
-    @property
-    def allow_data_changes(self):
-        """Entity hub allows changes of 'data' key on entities."""
-
-        return self._allow_data_changes
-
-    @property
-    def project_name(self):
-        return self._project_name
-
-    @property
-    def project_entity(self):
-        """Project entity."""
-
-        if self._project_entity is UNKNOWN_VALUE:
-            self.fill_project_from_server()
-        return self._project_entity
-
-    def get_attributes_for_type(self, entity_type):
-        """Get attributes available for a type.
-
-        Attributes are based on entity types.
-
-        Todos:
-            Use attribute schema to validate values on entities.
-
-        Args:
-            entity_type (Literal["project", "folder", "task"]): Entity type
-                for which should be attributes received.
-
-        Returns:
-            Dict[str, Dict[str, Any]]: Attribute schemas that are available
-                for entered entity type.
-        """
-
-        return self._connection.get_attributes_for_type(entity_type)
-
-    def get_entity_by_id(self, entity_id):
-        """Receive entity by its id without entity type.
-
-        The entity must be already existing in cached objects.
-
-        Args:
-            entity_id (str): Id of entity.
-
-        Returns:
-            Union[BaseEntity, None]: Entity object or None.
-        """
-
-        return self._entities_by_id.get(entity_id)
-
-    def get_folder_by_id(self, entity_id, allow_query=True):
-        """Get folder entity by id.
-
-        Args:
-            entity_id (str): Id of folder entity.
-            allow_query (bool): Try to query entity from server if is not
-                available in cache.
-
-        Returns:
-            Union[FolderEntity, None]: Object of folder or 'None'.
-        """
-
-        if allow_query:
-            return self.get_or_query_entity_by_id(entity_id, ["folder"])
-        return self._entities_by_id.get(entity_id)
-
-    def get_task_by_id(self, entity_id, allow_query=True):
-        """Get task entity by id.
-
-        Args:
-           entity_id (str): Id of task entity.
-           allow_query (bool): Try to query entity from server if is not
-               available in cache.
-
-        Returns:
-           Union[TaskEntity, None]: Object of folder or 'None'.
-        """
-
-        if allow_query:
-            return self.get_or_query_entity_by_id(entity_id, ["task"])
-        return self._entities_by_id.get(entity_id)
-
-    def get_or_query_entity_by_id(self, entity_id, entity_types):
-        """Get or query entity based on it's id and possible entity types.
-
-        This is a helper function when entity id is known but entity type may
-        have multiple possible options.
-
-        Args:
-            entity_id (str): Entity id.
-            entity_types (Iterable[str]): Possible entity types that can the id
-                represent. e.g. '["folder", "project"]'
-        """
-
-        existing_entity = self._entities_by_id.get(entity_id)
-        if existing_entity is not None:
-            return existing_entity
-
-        if not entity_types:
-            return None
-
-        entity_data = None
-        for entity_type in entity_types:
-            if entity_type == "folder":
-                entity_data = self._connection.get_folder_by_id(
-                    self.project_name,
-                    entity_id,
-                    fields=self._get_folder_fields(),
-                    own_attributes=True
-                )
-            elif entity_type == "task":
-                entity_data = self._connection.get_task_by_id(
-                    self.project_name,
-                    entity_id,
-                    own_attributes=True
-                )
-            else:
-                raise ValueError(
-                    "Unknonwn entity type \"{}\"".format(entity_type)
-                )
-
-            if entity_data:
-                break
-
-        if not entity_data:
-            return None
-
-        if entity_type == "folder":
-            return self.add_folder(entity_data)
-        elif entity_type == "task":
-            return self.add_task(entity_data)
-
-        return None
-
-    @property
-    def entities(self):
-        for entity in self._entities_by_id.values():
-            yield entity
-
-    def add_new_folder(self, *args, created=True, **kwargs):
-        """Create folder object and add it to entity hub.
-
-        Args:
-            parent (Union[ProjectEntity, FolderEntity]): Parent of added
-                folder.
-
-        Returns:
-            FolderEntity: Added folder entity.
-        """
-
-        folder_entity = FolderEntity(
-            *args, **kwargs, created=created, entity_hub=self
-        )
-        self.add_entity(folder_entity)
-        return folder_entity
-
-    def add_new_task(self, *args, created=True, **kwargs):
-        task_entity = TaskEntity(
-            *args, **kwargs, created=created, entity_hub=self
-        )
-        self.add_entity(task_entity)
-        return task_entity
-
-    def add_folder(self, folder):
-        """Create folder object and add it to entity hub.
-
-        Args:
-            folder (Dict[str, Any]): Folder entity data.
-
-        Returns:
-            FolderEntity: Added folder entity.
-        """
-
-        folder_entity = FolderEntity.from_entity_data(folder, entity_hub=self)
-        self.add_entity(folder_entity)
-        return folder_entity
-
-    def add_task(self, task):
-        """Create task object and add it to entity hub.
-
-        Args:
-            task (Dict[str, Any]): Task entity data.
-
-        Returns:
-            TaskEntity: Added task entity.
-        """
-
-        task_entity = TaskEntity.from_entity_data(task, entity_hub=self)
-        self.add_entity(task_entity)
-        return task_entity
-
-    def add_entity(self, entity):
-        """Add entity to hub cache.
-
-        Args:
-            entity (BaseEntity): Entity that should be added to hub's cache.
-        """
-
-        self._entities_by_id[entity.id] = entity
-        parent_children = self._entities_by_parent_id[entity.parent_id]
-        if entity not in parent_children:
-            parent_children.append(entity)
-
-        if entity.parent_id is PROJECT_PARENT_ID:
-            return
-
-        parent = self._entities_by_id.get(entity.parent_id)
-        if parent is not None:
-            parent.add_child(entity.id)
-
-    def folder_path_reseted(self, folder_id):
-        """Method called from 'FolderEntity' on path reset.
-
-        This should reset cache of folder paths on all children entities.
-
-        The path cache is always propagated from top to bottom so if an entity
-        has not cached path it means that any children can't have it cached.
-        """
-
-        if self._path_reset_queue is not None:
-            self._path_reset_queue.append(folder_id)
-            return
-
-        self._path_reset_queue = collections.deque()
-        self._path_reset_queue.append(folder_id)
-        while self._path_reset_queue:
-            children = self._entities_by_parent_id[folder_id]
-            for child in children:
-                # Get child path but don't trigger cache
-                path = child.get_path(False)
-                if path is not None:
-                    # Reset it's path cache if is set
-                    child.reset_path()
-                else:
-                    self._path_reset_queue.append(child.id)
-
-        self._path_reset_queue = None
-
-    def unset_entity_parent(self, entity_id, parent_id):
-        entity = self._entities_by_id.get(entity_id)
-        parent = self._entities_by_id.get(parent_id)
-        children_ids = UNKNOWN_VALUE
-        if parent is not None:
-            children_ids = parent.get_children_ids(False)
-
-        has_set_parent = False
-        if entity is not None:
-            has_set_parent = entity.parent_id == parent_id
-
-        new_parent_id = None
-        if has_set_parent:
-            entity.parent_id = new_parent_id
-
-        if children_ids is not UNKNOWN_VALUE and entity_id in children_ids:
-            parent.remove_child(entity_id)
-
-        if entity is None or not has_set_parent:
-            self.reset_immutable_for_hierarchy_cache(parent_id)
-            return
-
-        orig_parent_children = self._entities_by_parent_id[parent_id]
-        if entity in orig_parent_children:
-            orig_parent_children.remove(entity)
-
-        new_parent_children = self._entities_by_parent_id[new_parent_id]
-        if entity not in new_parent_children:
-            new_parent_children.append(entity)
-        self.reset_immutable_for_hierarchy_cache(parent_id)
-
-    def set_entity_parent(self, entity_id, parent_id, orig_parent_id=_NOT_SET):
-        parent = self._entities_by_id.get(parent_id)
-        entity = self._entities_by_id.get(entity_id)
-        if entity is None:
-            if parent is not None:
-                children_ids = parent.get_children_ids(False)
-                if (
-                    children_ids is not UNKNOWN_VALUE
-                    and entity_id in children_ids
-                ):
-                    parent.remove_child(entity_id)
-                self.reset_immutable_for_hierarchy_cache(parent.id)
-            return
-
-        if orig_parent_id is _NOT_SET:
-            orig_parent_id = entity.parent_id
-            if orig_parent_id == parent_id:
-                return
-
-        orig_parent_children = self._entities_by_parent_id[orig_parent_id]
-        if entity in orig_parent_children:
-            orig_parent_children.remove(entity)
-        self.reset_immutable_for_hierarchy_cache(orig_parent_id)
-
-        orig_parent = self._entities_by_id.get(orig_parent_id)
-        if orig_parent is not None:
-            orig_parent.remove_child(entity_id)
-
-        parent_children = self._entities_by_parent_id[parent_id]
-        if entity not in parent_children:
-            parent_children.append(entity)
-
-        entity.parent_id = parent_id
-        if parent is None or parent.get_children_ids(False) is UNKNOWN_VALUE:
-            return
-
-        parent.add_child(entity_id)
-        self.reset_immutable_for_hierarchy_cache(parent_id)
-
-    def _query_entity_children(self, entity):
-        folder_fields = self._get_folder_fields()
-        tasks = []
-        folders = []
-        if entity.entity_type == "project":
-            folders = list(self._connection.get_folders(
-                entity["name"],
-                parent_ids=[entity.id],
-                fields=folder_fields,
-                own_attributes=True
-            ))
-
-        elif entity.entity_type == "folder":
-            folders = list(self._connection.get_folders(
-                self.project_entity["name"],
-                parent_ids=[entity.id],
-                fields=folder_fields,
-                own_attributes=True
-            ))
-
-            tasks = list(self._connection.get_tasks(
-                self.project_entity["name"],
-                folder_ids=[entity.id],
-                own_attributes=True
-            ))
-
-        children_ids = {
-            child.id
-            for child in self._entities_by_parent_id[entity.id]
-        }
-        for folder in folders:
-            folder_entity = self._entities_by_id.get(folder["id"])
-            if folder_entity is not None:
-                if folder_entity.parent_id == entity.id:
-                    children_ids.add(folder_entity.id)
-                continue
-
-            folder_entity = self.add_folder(folder)
-            children_ids.add(folder_entity.id)
-
-        for task in tasks:
-            task_entity = self._entities_by_id.get(task["id"])
-            if task_entity is not None:
-                if task_entity.parent_id == entity.id:
-                    children_ids.add(task_entity.id)
-                continue
-
-            task_entity = self.add_task(task)
-            children_ids.add(task_entity.id)
-
-        entity.fill_children_ids(children_ids)
-
-    def get_entity_children(self, entity, allow_query=True):
-        children_ids = entity.get_children_ids(allow_query=False)
-        if children_ids is not UNKNOWN_VALUE:
-            return entity.get_children()
-
-        if children_ids is UNKNOWN_VALUE and not allow_query:
-            return UNKNOWN_VALUE
-
-        self._query_entity_children(entity)
-
-        return entity.get_children()
-
-    def delete_entity(self, entity):
-        parent_id = entity.parent_id
-        if parent_id is None:
-            return
-
-        parent = self._entities_by_parent_id.get(parent_id)
-        if parent is not None:
-            parent.remove_child(entity.id)
-
-    def reset_immutable_for_hierarchy_cache(
-        self, entity_id, bottom_to_top=True
-    ):
-        if bottom_to_top is None or entity_id is None:
-            return
-
-        reset_queue = collections.deque()
-        reset_queue.append(entity_id)
-        if bottom_to_top:
-            while reset_queue:
-                entity_id = reset_queue.popleft()
-                entity = self.get_entity_by_id(entity_id)
-                if entity is None:
-                    continue
-                entity.reset_immutable_for_hierarchy_cache(None)
-                reset_queue.append(entity.parent_id)
-        else:
-            while reset_queue:
-                entity_id = reset_queue.popleft()
-                entity = self.get_entity_by_id(entity_id)
-                if entity is None:
-                    continue
-                entity.reset_immutable_for_hierarchy_cache(None)
-                for child in self._entities_by_parent_id[entity.id]:
-                    reset_queue.append(child.id)
-
-    def fill_project_from_server(self):
-        """Query project from server and create it's entity.
-
-        Returns:
-            ProjectEntity: Entity that was created based on queried data.
-
-        Raises:
-            ValueError: When project was not found on server.
-        """
-
-        project_name = self.project_name
-        project = self._connection.get_project(
-            project_name,
-            own_attributes=True
-        )
-        if not project:
-            raise ValueError(
-                "Project \"{}\" was not found.".format(project_name)
-            )
-
-        self._project_entity = ProjectEntity(
-            project["code"],
-            parent_id=PROJECT_PARENT_ID,
-            entity_id=project["name"],
-            library=project["library"],
-            folder_types=project["folderTypes"],
-            task_types=project["taskTypes"],
-            name=project["name"],
-            attribs=project["ownAttrib"],
-            data=project["data"],
-            active=project["active"],
-            entity_hub=self
-        )
-        self.add_entity(self._project_entity)
-        return self._project_entity
-
-    def _get_folder_fields(self):
-        folder_fields = set(
-            self._connection.get_default_fields_for_type("folder")
-        )
-        folder_fields.add("hasSubsets")
-        if self._allow_data_changes:
-            folder_fields.add("data")
-        return folder_fields
-
-    def query_entities_from_server(self):
-        """Query whole project at once."""
-
-        project_entity = self.fill_project_from_server()
-
-        folder_fields = self._get_folder_fields()
-
-        folders = self._connection.get_folders(
-            project_entity.name,
-            fields=folder_fields,
-            own_attributes=True
-        )
-        tasks = self._connection.get_tasks(
-            project_entity.name,
-            own_attributes=True
-        )
-        folders_by_parent_id = collections.defaultdict(list)
-        for folder in folders:
-            parent_id = folder["parentId"]
-            folders_by_parent_id[parent_id].append(folder)
-
-        tasks_by_parent_id = collections.defaultdict(list)
-        for task in tasks:
-            parent_id = task["folderId"]
-            tasks_by_parent_id[parent_id].append(task)
-
-        hierarchy_queue = collections.deque()
-        hierarchy_queue.append((None, project_entity))
-        while hierarchy_queue:
-            item = hierarchy_queue.popleft()
-            parent_id, parent_entity = item
-
-            children_ids = set()
-            for folder in folders_by_parent_id[parent_id]:
-                folder_entity = self.add_folder(folder)
-                children_ids.add(folder_entity.id)
-                folder_entity.has_published_content = folder["hasSubsets"]
-                hierarchy_queue.append((folder_entity.id, folder_entity))
-
-            for task in tasks_by_parent_id[parent_id]:
-                task_entity = self.add_task(task)
-                children_ids.add(task_entity.id)
-
-            parent_entity.fill_children_ids(children_ids)
-        self.lock()
-
-    def lock(self):
-        if self._project_entity is None:
-            return
-
-        for entity in self._entities_by_id.values():
-            entity.lock()
-
-    def _get_top_entities(self):
-        all_ids = set(self._entities_by_id.keys())
-        return [
-            entity
-            for entity in self._entities_by_id.values()
-            if entity.parent_id not in all_ids
-        ]
-
-    def _split_entities(self):
-        top_entities = self._get_top_entities()
-        entities_queue = collections.deque(top_entities)
-        removed_entity_ids = []
-        created_entity_ids = []
-        other_entity_ids = []
-        while entities_queue:
-            entity = entities_queue.popleft()
-            removed = entity.removed
-            if removed:
-                removed_entity_ids.append(entity.id)
-            elif entity.created:
-                created_entity_ids.append(entity.id)
-            else:
-                other_entity_ids.append(entity.id)
-
-            for child in tuple(self._entities_by_parent_id[entity.id]):
-                if removed:
-                    self.unset_entity_parent(child.id, entity.id)
-                entities_queue.append(child)
-        return created_entity_ids, other_entity_ids, removed_entity_ids
-
-    def _get_update_body(self, entity, changes=None):
-        if changes is None:
-            changes = entity.changes
-
-        if not changes:
-            return None
-        return {
-            "type": "update",
-            "entityType": entity.entity_type,
-            "entityId": entity.id,
-            "data": changes
-        }
-
-    def _get_create_body(self, entity):
-        return {
-            "type": "create",
-            "entityType": entity.entity_type,
-            "entityId": entity.id,
-            "data": entity.to_create_body_data()
-        }
-
-    def _get_delete_body(self, entity):
-        return {
-            "type": "delete",
-            "entityType": entity.entity_type,
-            "entityId": entity.id
-        }
-
-    def commit_changes(self):
-        """Commit any changes that happened on entities.
-
-        Todos:
-            Use Operations Session instead of known operations body.
-        """
-
-        project_changes = self.project_entity.changes
-        if project_changes:
-            response = self._connection.patch(
-                "projects/{}".format(self.project_name),
-                **project_changes
-            )
-            if response.status_code != 204:
-                raise ValueError("Failed to update project")
-
-        self.project_entity.lock()
-
-        operations_body = []
-
-        created_entity_ids, other_entity_ids, removed_entity_ids = (
-            self._split_entities()
-        )
-        processed_ids = set()
-        for entity_id in other_entity_ids:
-            if entity_id in processed_ids:
-                continue
-
-            entity = self._entities_by_id[entity_id]
-            changes = entity.changes
-            processed_ids.add(entity_id)
-            if not changes:
-                continue
-
-            bodies = [self._get_update_body(entity, changes)]
-            # Parent was created and was not yet added to operations body
-            parent_queue = collections.deque()
-            parent_queue.append(entity.parent_id)
-            while parent_queue:
-                # Make sure entity's parents are created
-                parent_id = parent_queue.popleft()
-                if (
-                    parent_id is UNKNOWN_VALUE
-                    or parent_id in processed_ids
-                    or parent_id not in created_entity_ids
-                ):
-                    continue
-
-                parent = self._entities_by_id.get(parent_id)
-                processed_ids.add(parent.id)
-                bodies.append(self._get_create_body(parent))
-                parent_queue.append(parent.id)
-
-            operations_body.extend(reversed(bodies))
-
-        for entity_id in created_entity_ids:
-            if entity_id in processed_ids:
-                continue
-            entity = self._entities_by_id[entity_id]
-            operations_body.append(self._get_create_body(entity))
-
-        for entity_id in reversed(removed_entity_ids):
-            if entity_id in processed_ids:
-                continue
-
-            entity = self._entities_by_id.pop(entity_id)
-            parent_children = self._entities_by_parent_id[entity.parent_id]
-            if entity in parent_children:
-                parent_children.remove(entity)
-
-            if not entity.created:
-                operations_body.append(self._get_delete_body(entity))
-
-        self._connection.send_batch_operations(
-            self.project_name, operations_body
-        )
-
-        self.lock()
-
-
-class AttributeValue(object):
-    def __init__(self, value):
-        self._value = value
-        self._origin_value = copy.deepcopy(value)
-
-    def get_value(self):
-        return self._value
-
-    def set_value(self, value):
-        self._value = value
-
-    value = property(get_value, set_value)
-
-    @property
-    def changed(self):
-        return self._value != self._origin_value
-
-    def lock(self):
-        self._origin_value = copy.deepcopy(self._value)
-
-
-class Attributes(object):
-    """Object representing attribs of entity.
-
-    Todos:
-        This could be enhanced to know attribute schema and validate values
-        based on the schema.
-
-    Args:
-        attrib_keys (Iterable[str]): Keys that are available in attribs of the
-            entity.
-        values (Union[None, Dict[str, Any]]): Values of attributes.
-    """
-
-    def __init__(self, attrib_keys, values=UNKNOWN_VALUE):
-        if values in (UNKNOWN_VALUE, None):
-            values = {}
-        self._attributes = {
-            key: AttributeValue(values.get(key))
-            for key in attrib_keys
-        }
-
-    def __contains__(self, key):
-        return key in self._attributes
-
-    def __getitem__(self, key):
-        return self._attributes[key].value
-
-    def __setitem__(self, key, value):
-        self._attributes[key].set_value(value)
-
-    def __iter__(self):
-        for key in self._attributes:
-            yield key
-
-    def keys(self):
-        return self._attributes.keys()
-
-    def values(self):
-        for attribute in self._attributes.values():
-            yield attribute.value
-
-    def items(self):
-        for key, attribute in self._attributes.items():
-            yield key, attribute.value
-
-    def get(self, key, default=None):
-        """Get value of attribute.
-
-        Args:
-            key (str): Attribute name.
-            default (Any): Default value to return when attribute was not
-                found.
-        """
-
-        attribute = self._attributes.get(key)
-        if attribute is None:
-            return default
-        return attribute.value
-
-    def set(self, key, value):
-        """Change value of attribute.
-
-        Args:
-            key (str): Attribute name.
-            value (Any): New value of the attribute.
-        """
-
-        self[key] = value
-
-    def get_attribute(self, key):
-        """Access to attribute object.
-
-        Args:
-            key (str): Name of attribute.
-
-        Returns:
-            AttributeValue: Object of attribute value.
-
-        Raises:
-            KeyError: When attribute is not available.
-        """
-
-        return self._attributes[key]
-
-    def lock(self):
-        for attribute in self._attributes.values():
-            attribute.lock()
-
-    @property
-    def changes(self):
-        """Attribute value changes.
-
-        Returns:
-            Dict[str, Any]: Key mapping with new values.
-        """
-
-        return {
-            attr_key: attribute.value
-            for attr_key, attribute in self._attributes.items()
-            if attribute.changed
-        }
-
-    def to_dict(self, ignore_none=True):
-        output = {}
-        for key, value in self.items():
-            if (
-                value is UNKNOWN_VALUE
-                or (ignore_none and value is None)
-            ):
-                continue
-
-            output[key] = value
-        return output
-
-
-@six.add_metaclass(ABCMeta)
-class BaseEntity(object):
-    """Object representation of entity from server which is capturing changes.
-
-    All data on created object are expected as "current data" on server entity
-    unless the entity has set 'created' to 'True'. So if new data should be
-    stored to server entity then fill entity with server data first and
-    then change them.
-
-    Calling 'lock' method will mark entity as "saved" and all changes made on
-    entity are set as "current data" on server.
-
-    Args:
-        name (str): Name of entity.
-        attribs (Dict[str, Any]): Attribute values.
-        data (Dict[str, Any]): Entity data (custom data).
-        parent_id (Union[str, None]): Id of parent entity.
-        entity_id (Union[str, None]): Id of the entity. New id is created if
-            not passed.
-        thumbnail_id (Union[str, None]): Id of entity's thumbnail.
-        active (bool): Is entity active.
-        entity_hub (EntityHub): Object of entity hub which created object of
-            the entity.
-        created (Union[bool, None]): Entity is new. When 'None' is passed the
-            value is defined based on value of 'entity_id'.
-    """
-
-    def __init__(
-        self,
-        entity_id=None,
-        parent_id=UNKNOWN_VALUE,
-        name=UNKNOWN_VALUE,
-        attribs=UNKNOWN_VALUE,
-        data=UNKNOWN_VALUE,
-        thumbnail_id=UNKNOWN_VALUE,
-        active=UNKNOWN_VALUE,
-        entity_hub=None,
-        created=None
-    ):
-        if entity_hub is None:
-            raise ValueError("Missing required kwarg 'entity_hub'")
-
-        self._entity_hub = entity_hub
-
-        if created is None:
-            created = entity_id is None
-
-        entity_id = convert_entity_id(entity_id)
-        if entity_id is None:
-            entity_id = create_entity_id()
-
-        if data is None:
-            data = {}
-
-        children_ids = UNKNOWN_VALUE
-        if created:
-            children_ids = set()
-
-        if not created and parent_id is UNKNOWN_VALUE:
-            raise ValueError("Existing entity is missing parent id.")
-
-        # These are public without any validation at this moment
-        #   may change in future (e.g. name will have regex validation)
-        self._entity_id = entity_id
-
-        self._parent_id = parent_id
-        self._name = name
-        self.active = active
-        self._created = created
-        self._thumbnail_id = thumbnail_id
-        self._attribs = Attributes(
-            self._get_attributes_for_type(self.entity_type),
-            attribs
-        )
-        self._data = data
-        self._children_ids = children_ids
-
-        self._orig_parent_id = parent_id
-        self._orig_name = name
-        self._orig_data = copy.deepcopy(data)
-        self._orig_thumbnail_id = thumbnail_id
-        self._orig_active = active
-
-        self._immutable_for_hierarchy_cache = None
-
-    def __repr__(self):
-        return "<{} - {}>".format(self.__class__.__name__, self.id)
-
-    def __getitem__(self, item):
-        return getattr(self, item)
-
-    def __setitem__(self, item, value):
-        return setattr(self, item, value)
-
-    @property
-    def id(self):
-        """Access to entity id under which is entity available on server.
-
-        Returns:
-            str: Entity id.
-        """
-
-        return self._entity_id
-
-    @property
-    def removed(self):
-        return self._parent_id is None
-
-    @property
-    def orig_parent_id(self):
-        return self._orig_parent_id
-
-    @property
-    def attribs(self):
-        """Entity attributes based on server configuration.
-
-        Returns:
-            Attributes: Attributes object handling changes and values of
-                attributes on entity.
-        """
-
-        return self._attribs
-
-    @property
-    def data(self):
-        """Entity custom data that are not stored by any deterministic model.
-
-        Be aware that 'data' can't be queried using GraphQl and cannot be
-            updated partially.
-
-        Returns:
-            Dict[str, Any]: Custom data on entity.
-        """
-
-        return self._data
-
-    @property
-    def project_name(self):
-        """Quick access to project from entity hub.
-
-        Returns:
-            str: Name of project under which entity lives.
-        """
-
-        return self._entity_hub.project_name
-
-    @abstractproperty
-    def entity_type(self):
-        """Entity type coresponding to server.
-
-        Returns:
-            Literal[project, folder, task]: Entity type.
-        """
-
-        pass
-
-    @abstractproperty
-    def parent_entity_types(self):
-        """Entity type coresponding to server.
-
-        Returns:
-            Iterable[str]: Possible entity types of parent.
-        """
-
-        pass
-
-    @abstractproperty
-    def changes(self):
-        """Receive entity changes.
-
-        Returns:
-            Union[Dict[str, Any], None]: All values that have changed on
-                entity. New entity must return None.
-        """
-
-        pass
-
-    @classmethod
-    @abstractmethod
-    def from_entity_data(cls, entity_data, entity_hub):
-        """Create entity based on queried data from server.
-
-        Args:
-            entity_data (Dict[str, Any]): Entity data from server.
-            entity_hub (EntityHub): Hub which handle the entity.
-
-        Returns:
-            BaseEntity: Object of the class.
-        """
-
-        pass
-
-    @abstractmethod
-    def to_create_body_data(self):
-        """Convert object of entity to data for server on creation.
-
-        Returns:
-            Dict[str, Any]: Entity data.
-        """
-
-        pass
-
-    @property
-    def immutable_for_hierarchy(self):
-        """Entity is immutable for hierarchy changes.
-
-        Hierarchy changes can be considered as change of name or parents.
-
-        Returns:
-            bool: Entity is immutable for hierarchy changes.
-        """
-
-        if self._immutable_for_hierarchy_cache is not None:
-            return self._immutable_for_hierarchy_cache
-
-        immutable_for_hierarchy = self._immutable_for_hierarchy
-        if immutable_for_hierarchy is not None:
-            self._immutable_for_hierarchy_cache = immutable_for_hierarchy
-            return self._immutable_for_hierarchy_cache
-
-        for child in self._entity_hub.get_entity_children(self):
-            if child.immutable_for_hierarchy:
-                self._immutable_for_hierarchy_cache = True
-                return self._immutable_for_hierarchy_cache
-
-        self._immutable_for_hierarchy_cache = False
-        return self._immutable_for_hierarchy_cache
-
-    @property
-    def _immutable_for_hierarchy(self):
-        """Override this method to define if entity object is immutable.
-
-        This property was added to define immutable state of Folder entities
-        which is used in property 'immutable_for_hierarchy'.
-
-        Returns:
-            Union[bool, None]: Bool to explicitly telling if is immutable or
-                not otherwise None.
-        """
-
-        return None
-
-    @property
-    def has_cached_immutable_hierarchy(self):
-        return self._immutable_for_hierarchy_cache is not None
-
-    def reset_immutable_for_hierarchy_cache(self, bottom_to_top=True):
-        """Clear cache of immutable hierarchy property.
-
-        This is used when entity changed parent or a child was added.
-
-        Args:
-            bottom_to_top (bool): Reset cache from top hierarchy to bottom or
-                from bottom hierarchy to top.
-        """
-
-        self._immutable_for_hierarchy_cache = None
-        self._entity_hub.reset_immutable_for_hierarchy_cache(
-            self.id, bottom_to_top
-        )
-
-    def _get_default_changes(self):
-        """Collect changes of common data on entity.
-
-        Returns:
-            Dict[str, Any]: Changes on entity. Key and it's new value.
-        """
-
-        changes = {}
-        if self._orig_name != self._name:
-            changes["name"] = self._name
-
-        if self._entity_hub.allow_data_changes:
-            if self._orig_data != self._data:
-                changes["data"] = self._data
-
-        if self._orig_thumbnail_id != self._thumbnail_id:
-            changes["thumbnailId"] = self._thumbnail_id
-
-        if self._orig_active != self.active:
-            changes["active"] = self.active
-
-        attrib_changes = self.attribs.changes
-        if attrib_changes:
-            changes["attrib"] = attrib_changes
-        return changes
-
-    def _get_attributes_for_type(self, entity_type):
-        return self._entity_hub.get_attributes_for_type(entity_type)
-
-    def lock(self):
-        """Lock entity as 'saved' so all changes are discarded."""
-
-        self._orig_parent_id = self._parent_id
-        self._orig_name = self._name
-        self._orig_data = copy.deepcopy(self._data)
-        self._orig_thumbnail_id = self.thumbnail_id
-        self._attribs.lock()
-
-        self._immutable_for_hierarchy_cache = None
-
-    def _get_entity_by_id(self, entity_id):
-        return self._entity_hub.get_entity_by_id(entity_id)
-
-    def get_name(self):
-        return self._name
-
-    def set_name(self, name):
-        self._name = name
-
-    name = property(get_name, set_name)
-
-    def get_parent_id(self):
-        """Parent entity id.
-
-        Returns:
-            Union[str, None]: Id of parent entity or none if is not set.
-        """
-
-        return self._parent_id
-
-    def set_parent_id(self, parent_id):
-        """Change parent by id.
-
-        Args:
-            parent_id (Union[str, None]): Id of new parent for entity.
-
-        Raises:
-            ValueError: If parent was not found by id.
-            TypeError: If validation of parent does not pass.
-        """
-
-        if parent_id != self._parent_id:
-            orig_parent_id = self._parent_id
-            self._parent_id = parent_id
-            self._entity_hub.set_entity_parent(
-                self.id, parent_id, orig_parent_id
-            )
-
-    parent_id = property(get_parent_id, set_parent_id)
-
-    def get_parent(self, allow_query=True):
-        """Parent entity.
-
-        Returns:
-            Union[BaseEntity, None]: Parent object.
-        """
-
-        parent = self._entity_hub.get_entity_by_id(self._parent_id)
-        if parent is not None:
-            return parent
-
-        if not allow_query:
-            return self._parent_id
-
-        if self._parent_id is UNKNOWN_VALUE:
-            return self._parent_id
-
-        return self._entity_hub.get_or_query_entity_by_id(
-            self._parent_id, self.parent_entity_types
-        )
-
-    def set_parent(self, parent):
-        """Change parent object.
-
-        Args:
-            parent (BaseEntity): New parent for entity.
-
-        Raises:
-            TypeError: If validation of parent does not pass.
-        """
-
-        parent_id = None
-        if parent is not None:
-            parent_id = parent.id
-        self._entity_hub.set_entity_parent(self.id, parent_id)
-
-    parent = property(get_parent, set_parent)
-
-    def get_children_ids(self, allow_query=True):
-        """Access to children objects.
-
-        Todos:
-            Children should be maybe handled by EntityHub instead of entities
-                themselves. That would simplify 'set_entity_parent',
-                'unset_entity_parent' and other logic related to changing
-                hierarchy.
-
-        Returns:
-            Union[List[str], Type[UNKNOWN_VALUE]]: Children iterator.
-        """
-
-        if self._children_ids is UNKNOWN_VALUE:
-            if not allow_query:
-                return self._children_ids
-            self._entity_hub.get_entity_children(self, True)
-        return set(self._children_ids)
-
-    children_ids = property(get_children_ids)
-
-    def get_children(self, allow_query=True):
-        """Access to children objects.
-
-        Returns:
-            Union[List[BaseEntity], Type[UNKNOWN_VALUE]]: Children iterator.
-        """
-
-        if self._children_ids is UNKNOWN_VALUE:
-            if not allow_query:
-                return self._children_ids
-            return self._entity_hub.get_entity_children(self, True)
-
-        return [
-            self._entity_hub.get_entity_by_id(children_id)
-            for children_id in self._children_ids
-        ]
-
-    children = property(get_children)
-
-    def add_child(self, child):
-        """Add child entity.
-
-        Args:
-            child (BaseEntity): Child object to add.
-
-        Raises:
-            TypeError: When child object has invalid type to be children.
-        """
-
-        child_id = child
-        if isinstance(child_id, BaseEntity):
-            child_id = child.id
-
-        if self._children_ids is not UNKNOWN_VALUE:
-            self._children_ids.add(child_id)
-
-        self._entity_hub.set_entity_parent(child_id, self.id)
-
-    def remove_child(self, child):
-        """Remove child entity.
-
-        Is ignored if child is not in children.
-
-        Args:
-            child (Union[str, BaseEntity]): Child object or child id to remove.
-        """
-
-        child_id = child
-        if isinstance(child_id, BaseEntity):
-            child_id = child.id
-
-        if self._children_ids is not UNKNOWN_VALUE:
-            self._children_ids.discard(child_id)
-        self._entity_hub.unset_entity_parent(child_id, self.id)
-
-    def get_thumbnail_id(self):
-        """Thumbnail id of entity.
-
-        Returns:
-            Union[str, None]: Id of parent entity or none if is not set.
-        """
-
-        return self._thumbnail_id
-
-    def set_thumbnail_id(self, thumbnail_id):
-        """Change thumbnail id.
-
-        Args:
-            thumbnail_id (Union[str, None]): Id of thumbnail for entity.
-        """
-
-        self._thumbnail_id = thumbnail_id
-
-    thumbnail_id = property(get_thumbnail_id, set_thumbnail_id)
-
-    @property
-    def created(self):
-        """Entity is new.
-
-        Returns:
-            bool: Entity is newly created.
-        """
-
-        return self._created
-
-    def fill_children_ids(self, children_ids):
-        """Fill children ids on entity.
-
-        Warning:
-            This is not an api call but is called from entity hub.
-        """
-
-        self._children_ids = set(children_ids)
-
-
-class ProjectEntity(BaseEntity):
-    entity_type = "project"
-    parent_entity_types = []
-    # TODO These are hardcoded but maybe should be used from server???
-    default_folder_type_icon = "folder"
-    default_task_type_icon = "task_alt"
-
-    def __init__(
-        self, project_code, library, folder_types, task_types, *args, **kwargs
-    ):
-        super(ProjectEntity, self).__init__(*args, **kwargs)
-
-        self._project_code = project_code
-        self._library_project = library
-        self._folder_types = folder_types
-        self._task_types = task_types
-
-        self._orig_project_code = project_code
-        self._orig_library_project = library
-        self._orig_folder_types = copy.deepcopy(folder_types)
-        self._orig_task_types = copy.deepcopy(task_types)
-
-    def get_parent(self, *args, **kwargs):
-        return None
-
-    def set_parent(self, parent):
-        raise ValueError(
-            "Parent of project cannot be set to {}".format(parent)
-        )
-
-    parent = property(get_parent, set_parent)
-
-    def get_folder_types(self):
-        return copy.deepcopy(self._folder_types)
-
-    def set_folder_types(self, folder_types):
-        new_folder_types = []
-        for folder_type in folder_types:
-            if "icon" not in folder_type:
-                folder_type["icon"] = self.default_folder_type_icon
-            new_folder_types.append(folder_type)
-        self._folder_types = new_folder_types
-
-    def get_task_types(self):
-        return copy.deepcopy(self._task_types)
-
-    def set_task_types(self, task_types):
-        new_task_types = []
-        for task_type in task_types:
-            if "icon" not in task_type:
-                task_type["icon"] = self.default_task_type_icon
-            new_task_types.append(task_type)
-        self._task_types = new_task_types
-
-    folder_types = property(get_folder_types, set_folder_types)
-    task_types = property(get_task_types, set_task_types)
-
-    def lock(self):
-        super(ProjectEntity, self).lock()
-        self._orig_folder_types = copy.deepcopy(self._folder_types)
-        self._orig_task_types = copy.deepcopy(self._task_types)
-
-    @property
-    def changes(self):
-        changes = self._get_default_changes()
-        if self._orig_folder_types != self._folder_types:
-            changes["folderTypes"] = self.get_folder_types()
-
-        if self._orig_task_types != self._task_types:
-            changes["taskTypes"] = self.get_task_types()
-
-        return changes
-
-    @classmethod
-    def from_entity_data(cls, project, entity_hub):
-        return cls(
-            project["code"],
-            parent_id=PROJECT_PARENT_ID,
-            entity_id=project["name"],
-            library=project["library"],
-            folder_types=project["folderTypes"],
-            task_types=project["taskTypes"],
-            name=project["name"],
-            attribs=project["ownAttrib"],
-            data=project["data"],
-            active=project["active"],
-            entity_hub=entity_hub
-        )
-
-    def to_create_body_data(self):
-        raise NotImplementedError(
-            "ProjectEntity does not support conversion to entity data"
-        )
-
-
-class FolderEntity(BaseEntity):
-    entity_type = "folder"
-    parent_entity_types = ["folder", "project"]
-
-    def __init__(self, folder_type, *args, label=None, path=None, **kwargs):
-        super(FolderEntity, self).__init__(*args, **kwargs)
-
-        self._folder_type = folder_type
-        self._label = label
-
-        self._orig_folder_type = folder_type
-        self._orig_label = label
-        # Know if folder has any subsets
-        # - is used to know if folder allows hierarchy changes
-        self._has_published_content = False
-        self._path = path
-
-    def get_folder_type(self):
-        return self._folder_type
-
-    def set_folder_type(self, folder_type):
-        self._folder_type = folder_type
-
-    folder_type = property(get_folder_type, set_folder_type)
-
-    def get_label(self):
-        return self._label
-
-    def set_label(self, label):
-        self._label = label
-
-    label = property(get_label, set_label)
-
-    def get_path(self, dynamic_value=True):
-        if not dynamic_value:
-            return self._path
-
-        if self._path is None:
-            parent = self.parent
-            path = self.name
-            if parent.entity_type == "folder":
-                parent_path = parent.path
-                path = "/".join([parent_path, path])
-            self._path = path
-        return self._path
-
-    def reset_path(self):
-        self._path = None
-        self._entity_hub.folder_path_reseted(self.id)
-
-    path = property(get_path)
-
-    def get_has_published_content(self):
-        return self._has_published_content
-
-    def set_has_published_content(self, has_published_content):
-        if self._has_published_content is has_published_content:
-            return
-
-        self._has_published_content = has_published_content
-        # Reset immutable cache of parents
-        self._entity_hub.reset_immutable_for_hierarchy_cache(self.id)
-
-    has_published_content = property(
-        get_has_published_content, set_has_published_content
-    )
-
-    @property
-    def _immutable_for_hierarchy(self):
-        if self.has_published_content:
-            return True
-        return None
-
-    def lock(self):
-        super(FolderEntity, self).lock()
-        self._orig_folder_type = self._folder_type
-
-    @property
-    def changes(self):
-        changes = self._get_default_changes()
-
-        if self._orig_parent_id != self._parent_id:
-            parent_id = self._parent_id
-            if parent_id == self.project_name:
-                parent_id = None
-            changes["parentId"] = parent_id
-
-        if self._orig_folder_type != self._folder_type:
-            changes["folderType"] = self._folder_type
-
-        label = self._label
-        if self._name == label:
-            label = None
-
-        if label != self._orig_label:
-            changes["label"] = label
-
-        return changes
-
-    @classmethod
-    def from_entity_data(cls, folder, entity_hub):
-        parent_id = folder["parentId"]
-        if parent_id is None:
-            parent_id = entity_hub.project_entity.id
-        return cls(
-            folder["folderType"],
-            label=folder["label"],
-            path=folder["path"],
-            entity_id=folder["id"],
-            parent_id=parent_id,
-            name=folder["name"],
-            data=folder.get("data"),
-            attribs=folder["ownAttrib"],
-            active=folder["active"],
-            thumbnail_id=folder["thumbnailId"],
-            created=False,
-            entity_hub=entity_hub
-        )
-
-    def to_create_body_data(self):
-        parent_id = self._parent_id
-        if parent_id is UNKNOWN_VALUE:
-            raise ValueError("Folder does not have set 'parent_id'")
-
-        if parent_id == self.project_name:
-            parent_id = None
-
-        if not self.name or self.name is UNKNOWN_VALUE:
-            raise ValueError("Folder does not have set 'name'")
-
-        output = {
-            "name": self.name,
-            "folderType": self.folder_type,
-            "parentId": parent_id,
-        }
-        attrib = self.attribs.to_dict()
-        if attrib:
-            output["attrib"] = attrib
-
-        if self.active is not UNKNOWN_VALUE:
-            output["active"] = self.active
-
-        if self.thumbnail_id is not UNKNOWN_VALUE:
-            output["thumbnailId"] = self.thumbnail_id
-
-        if self._entity_hub.allow_data_changes:
-            output["data"] = self._data
-        return output
-
-
-class TaskEntity(BaseEntity):
-    entity_type = "task"
-    parent_entity_types = ["folder"]
-
-    def __init__(self, task_type, *args, label=None, **kwargs):
-        super(TaskEntity, self).__init__(*args, **kwargs)
-
-        self._task_type = task_type
-        self._label = label
-
-        self._orig_task_type = task_type
-        self._orig_label = label
-
-        self._children_ids = set()
-
-    def lock(self):
-        super(TaskEntity, self).lock()
-        self._orig_task_type = self._task_type
-
-    def get_task_type(self):
-        return self._task_type
-
-    def set_task_type(self, task_type):
-        self._task_type = task_type
-
-    task_type = property(get_task_type, set_task_type)
-
-    def get_label(self):
-        return self._label
-
-    def set_label(self, label):
-        self._label = label
-
-    label = property(get_label, set_label)
-
-    def add_child(self, child):
-        raise ValueError("Task does not support to add children")
-
-    @property
-    def changes(self):
-        changes = self._get_default_changes()
-
-        if self._orig_parent_id != self._parent_id:
-            changes["folderId"] = self._parent_id
-
-        if self._orig_task_type != self._task_type:
-            changes["taskType"] = self._task_type
-
-        label = self._label
-        if self._name == label:
-            label = None
-
-        if label != self._orig_label:
-            changes["label"] = label
-
-        return changes
-
-    @classmethod
-    def from_entity_data(cls, task, entity_hub):
-        return cls(
-            task["taskType"],
-            entity_id=task["id"],
-            label=task["label"],
-            parent_id=task["folderId"],
-            name=task["name"],
-            data=task.get("data"),
-            attribs=task["ownAttrib"],
-            active=task["active"],
-            created=False,
-            entity_hub=entity_hub
-        )
-
-    def to_create_body_data(self):
-        if self.parent_id is UNKNOWN_VALUE:
-            raise ValueError("Task does not have set 'parent_id'")
-
-        output = {
-            "name": self.name,
-            "taskType": self.task_type,
-            "folderId": self.parent_id,
-            "attrib": self.attribs.to_dict(),
-        }
-        attrib = self.attribs.to_dict()
-        if attrib:
-            output["attrib"] = attrib
-
-        if self.active is not UNKNOWN_VALUE:
-            output["active"] = self.active
-
-        if (
-            self._entity_hub.allow_data_changes
-            and self._data is not UNKNOWN_VALUE
-        ):
-            output["data"] = self._data
-        return output
+import copy
+import collections
+from abc import ABCMeta, abstractmethod
+
+import six
+from ._api import get_server_api_connection
+from .utils import create_entity_id, convert_entity_id
+
+UNKNOWN_VALUE = object()
+PROJECT_PARENT_ID = object()
+_NOT_SET = object()
+
+
+class EntityHub(object):
+    """Helper to create, update or remove entities in project.
+
+    The hub is a guide to operation with folder entities and update of project.
+    Project entity must already exist on server (can be only updated).
+
+    Object is caching entities queried from server. They won't be required once
+    they were queried, so it is recommended to create new hub or clear cache
+    frequently.
+
+    Todos:
+        Listen to server events about entity changes to be able update already
+            queried entities.
+
+    Args:
+        project_name (str): Name of project where changes will happen.
+        connection (ServerAPI): Connection to server with logged user.
+        allow_data_changes (bool): This option gives ability to change 'data'
+            key on entities. This is not recommended as 'data' may be use for
+            secure information and would also slow down server queries. Content
+            of 'data' key can't be received only GraphQl.
+    """
+
+    def __init__(
+        self, project_name, connection=None, allow_data_changes=False
+    ):
+        if not connection:
+            connection = get_server_api_connection()
+        self._connection = connection
+
+        self._project_name = project_name
+        self._entities_by_id = {}
+        self._entities_by_parent_id = collections.defaultdict(list)
+        self._project_entity = UNKNOWN_VALUE
+
+        self._allow_data_changes = allow_data_changes
+
+        self._path_reset_queue = None
+
+    @property
+    def allow_data_changes(self):
+        """Entity hub allows changes of 'data' key on entities.
+
+        Data are private and not all users may have access to them. Also to get
+        'data' for entity is required to use REST api calls, which means to
+        query each entity on-by-one from server.
+
+        Returns:
+            bool: Data changes are allowed.
+        """
+
+        return self._allow_data_changes
+
+    @property
+    def project_name(self):
+        """Project name which is maintained by hub.
+
+        Returns:
+            str: Name of project.
+        """
+
+        return self._project_name
+
+    @property
+    def project_entity(self):
+        """Project entity.
+
+        Returns:
+            ProjectEntity: Project entity.
+        """
+
+        if self._project_entity is UNKNOWN_VALUE:
+            self.fill_project_from_server()
+        return self._project_entity
+
+    def get_attributes_for_type(self, entity_type):
+        """Get attributes available for a type.
+
+        Attributes are based on entity types.
+
+        Todos:
+            Use attribute schema to validate values on entities.
+
+        Args:
+            entity_type (Literal["project", "folder", "task"]): Entity type
+                for which should be attributes received.
+
+        Returns:
+            Dict[str, Dict[str, Any]]: Attribute schemas that are available
+                for entered entity type.
+        """
+
+        return self._connection.get_attributes_for_type(entity_type)
+
+    def get_entity_by_id(self, entity_id):
+        """Receive entity by its id without entity type.
+
+        The entity must be already existing in cached objects.
+
+        Args:
+            entity_id (str): Id of entity.
+
+        Returns:
+            Union[BaseEntity, None]: Entity object or None.
+        """
+
+        return self._entities_by_id.get(entity_id)
+
+    def get_folder_by_id(self, entity_id, allow_query=True):
+        """Get folder entity by id.
+
+        Args:
+            entity_id (str): Id of folder entity.
+            allow_query (bool): Try to query entity from server if is not
+                available in cache.
+
+        Returns:
+            Union[FolderEntity, None]: Object of folder or 'None'.
+        """
+
+        if allow_query:
+            return self.get_or_query_entity_by_id(entity_id, ["folder"])
+        return self._entities_by_id.get(entity_id)
+
+    def get_task_by_id(self, entity_id, allow_query=True):
+        """Get task entity by id.
+
+        Args:
+           entity_id (str): Id of task entity.
+           allow_query (bool): Try to query entity from server if is not
+               available in cache.
+
+        Returns:
+           Union[TaskEntity, None]: Object of folder or 'None'.
+        """
+
+        if allow_query:
+            return self.get_or_query_entity_by_id(entity_id, ["task"])
+        return self._entities_by_id.get(entity_id)
+
+    def get_or_query_entity_by_id(self, entity_id, entity_types):
+        """Get or query entity based on it's id and possible entity types.
+
+        This is a helper function when entity id is known but entity type may
+        have multiple possible options.
+
+        Args:
+            entity_id (str): Entity id.
+            entity_types (Iterable[str]): Possible entity types that can the id
+                represent. e.g. '["folder", "project"]'
+        """
+
+        existing_entity = self._entities_by_id.get(entity_id)
+        if existing_entity is not None:
+            return existing_entity
+
+        if not entity_types:
+            return None
+
+        entity_data = None
+        for entity_type in entity_types:
+            if entity_type == "folder":
+                entity_data = self._connection.get_folder_by_id(
+                    self.project_name,
+                    entity_id,
+                    fields=self._get_folder_fields(),
+                    own_attributes=True
+                )
+            elif entity_type == "task":
+                entity_data = self._connection.get_task_by_id(
+                    self.project_name,
+                    entity_id,
+                    own_attributes=True
+                )
+            else:
+                raise ValueError(
+                    "Unknonwn entity type \"{}\"".format(entity_type)
+                )
+
+            if entity_data:
+                break
+
+        if not entity_data:
+            return None
+
+        if entity_type == "folder":
+            return self.add_folder(entity_data)
+        elif entity_type == "task":
+            return self.add_task(entity_data)
+
+        return None
+
+    @property
+    def entities(self):
+        """Iterator over available entities.
+
+        Returns:
+            Iterator[BaseEntity]: All queried/created entities cached in hub.
+        """
+
+        for entity in self._entities_by_id.values():
+            yield entity
+
+    def add_new_folder(self, *args, created=True, **kwargs):
+        """Create folder object and add it to entity hub.
+
+        Args:
+            folder_type (str): Type of folder. Folder type must be available in
+                config of project folder types.
+            entity_id (Union[str, None]): Id of the entity. New id is created if
+                not passed.
+            parent_id (Union[str, None]): Id of parent entity.
+            name (str): Name of entity.
+            label (Optional[str]): Folder label.
+            path (Optional[str]): Folder path. Path consist of all parent names
+                with slash('/') used as separator.
+            attribs (Dict[str, Any]): Attribute values.
+            data (Dict[str, Any]): Entity data (custom data).
+            thumbnail_id (Union[str, None]): Id of entity's thumbnail.
+            active (bool): Is entity active.
+            created (Optional[bool]): Entity is new. When 'None' is passed the
+                value is defined based on value of 'entity_id'.
+
+        Returns:
+            FolderEntity: Added folder entity.
+        """
+
+        folder_entity = FolderEntity(
+            *args, **kwargs, created=created, entity_hub=self
+        )
+        self.add_entity(folder_entity)
+        return folder_entity
+
+    def add_new_task(self, *args, created=True, **kwargs):
+        """Create folder object and add it to entity hub.
+
+        Args:
+            task_type (str): Type of task. Task type must be available in
+                config of project folder types.
+            entity_id (Union[str, None]): Id of the entity. New id is created if
+                not passed.
+            parent_id (Union[str, None]): Id of parent entity.
+            name (str): Name of entity.
+            label (Optional[str]): Folder label.
+            attribs (Dict[str, Any]): Attribute values.
+            data (Dict[str, Any]): Entity data (custom data).
+            thumbnail_id (Union[str, None]): Id of entity's thumbnail.
+            active (bool): Is entity active.
+            created (Optional[bool]): Entity is new. When 'None' is passed the
+                value is defined based on value of 'entity_id'.
+
+        Returns:
+            TaskEntity: Added task entity.
+        """
+
+        task_entity = TaskEntity(
+            *args, **kwargs, created=created, entity_hub=self
+        )
+        self.add_entity(task_entity)
+        return task_entity
+
+    def add_folder(self, folder):
+        """Create folder object and add it to entity hub.
+
+        Args:
+            folder (Dict[str, Any]): Folder entity data.
+
+        Returns:
+            FolderEntity: Added folder entity.
+        """
+
+        folder_entity = FolderEntity.from_entity_data(folder, entity_hub=self)
+        self.add_entity(folder_entity)
+        return folder_entity
+
+    def add_task(self, task):
+        """Create task object and add it to entity hub.
+
+        Args:
+            task (Dict[str, Any]): Task entity data.
+
+        Returns:
+            TaskEntity: Added task entity.
+        """
+
+        task_entity = TaskEntity.from_entity_data(task, entity_hub=self)
+        self.add_entity(task_entity)
+        return task_entity
+
+    def add_entity(self, entity):
+        """Add entity to hub cache.
+
+        Args:
+            entity (BaseEntity): Entity that should be added to hub's cache.
+        """
+
+        self._entities_by_id[entity.id] = entity
+        parent_children = self._entities_by_parent_id[entity.parent_id]
+        if entity not in parent_children:
+            parent_children.append(entity)
+
+        if entity.parent_id is PROJECT_PARENT_ID:
+            return
+
+        parent = self._entities_by_id.get(entity.parent_id)
+        if parent is not None:
+            parent.add_child(entity.id)
+
+    def folder_path_reseted(self, folder_id):
+        """Method called from 'FolderEntity' on path reset.
+
+        This should reset cache of folder paths on all children entities.
+
+        The path cache is always propagated from top to bottom so if an entity
+        has not cached path it means that any children can't have it cached.
+        """
+
+        if self._path_reset_queue is not None:
+            self._path_reset_queue.append(folder_id)
+            return
+
+        self._path_reset_queue = collections.deque()
+        self._path_reset_queue.append(folder_id)
+        while self._path_reset_queue:
+            children = self._entities_by_parent_id[folder_id]
+            for child in children:
+                # Get child path but don't trigger cache
+                path = child.get_path(False)
+                if path is not None:
+                    # Reset it's path cache if is set
+                    child.reset_path()
+                else:
+                    self._path_reset_queue.append(child.id)
+
+        self._path_reset_queue = None
+
+    def unset_entity_parent(self, entity_id, parent_id):
+        entity = self._entities_by_id.get(entity_id)
+        parent = self._entities_by_id.get(parent_id)
+        children_ids = UNKNOWN_VALUE
+        if parent is not None:
+            children_ids = parent.get_children_ids(False)
+
+        has_set_parent = False
+        if entity is not None:
+            has_set_parent = entity.parent_id == parent_id
+
+        new_parent_id = None
+        if has_set_parent:
+            entity.parent_id = new_parent_id
+
+        if children_ids is not UNKNOWN_VALUE and entity_id in children_ids:
+            parent.remove_child(entity_id)
+
+        if entity is None or not has_set_parent:
+            self.reset_immutable_for_hierarchy_cache(parent_id)
+            return
+
+        orig_parent_children = self._entities_by_parent_id[parent_id]
+        if entity in orig_parent_children:
+            orig_parent_children.remove(entity)
+
+        new_parent_children = self._entities_by_parent_id[new_parent_id]
+        if entity not in new_parent_children:
+            new_parent_children.append(entity)
+        self.reset_immutable_for_hierarchy_cache(parent_id)
+
+    def set_entity_parent(self, entity_id, parent_id, orig_parent_id=_NOT_SET):
+        parent = self._entities_by_id.get(parent_id)
+        entity = self._entities_by_id.get(entity_id)
+        if entity is None:
+            if parent is not None:
+                children_ids = parent.get_children_ids(False)
+                if (
+                    children_ids is not UNKNOWN_VALUE
+                    and entity_id in children_ids
+                ):
+                    parent.remove_child(entity_id)
+                self.reset_immutable_for_hierarchy_cache(parent.id)
+            return
+
+        if orig_parent_id is _NOT_SET:
+            orig_parent_id = entity.parent_id
+            if orig_parent_id == parent_id:
+                return
+
+        orig_parent_children = self._entities_by_parent_id[orig_parent_id]
+        if entity in orig_parent_children:
+            orig_parent_children.remove(entity)
+        self.reset_immutable_for_hierarchy_cache(orig_parent_id)
+
+        orig_parent = self._entities_by_id.get(orig_parent_id)
+        if orig_parent is not None:
+            orig_parent.remove_child(entity_id)
+
+        parent_children = self._entities_by_parent_id[parent_id]
+        if entity not in parent_children:
+            parent_children.append(entity)
+
+        entity.parent_id = parent_id
+        if parent is None or parent.get_children_ids(False) is UNKNOWN_VALUE:
+            return
+
+        parent.add_child(entity_id)
+        self.reset_immutable_for_hierarchy_cache(parent_id)
+
+    def _query_entity_children(self, entity):
+        folder_fields = self._get_folder_fields()
+        tasks = []
+        folders = []
+        if entity.entity_type == "project":
+            folders = list(self._connection.get_folders(
+                entity["name"],
+                parent_ids=[entity.id],
+                fields=folder_fields,
+                own_attributes=True
+            ))
+
+        elif entity.entity_type == "folder":
+            folders = list(self._connection.get_folders(
+                self.project_entity["name"],
+                parent_ids=[entity.id],
+                fields=folder_fields,
+                own_attributes=True
+            ))
+
+            tasks = list(self._connection.get_tasks(
+                self.project_entity["name"],
+                folder_ids=[entity.id],
+                own_attributes=True
+            ))
+
+        children_ids = {
+            child.id
+            for child in self._entities_by_parent_id[entity.id]
+        }
+        for folder in folders:
+            folder_entity = self._entities_by_id.get(folder["id"])
+            if folder_entity is not None:
+                if folder_entity.parent_id == entity.id:
+                    children_ids.add(folder_entity.id)
+                continue
+
+            folder_entity = self.add_folder(folder)
+            children_ids.add(folder_entity.id)
+
+        for task in tasks:
+            task_entity = self._entities_by_id.get(task["id"])
+            if task_entity is not None:
+                if task_entity.parent_id == entity.id:
+                    children_ids.add(task_entity.id)
+                continue
+
+            task_entity = self.add_task(task)
+            children_ids.add(task_entity.id)
+
+        entity.fill_children_ids(children_ids)
+
+    def get_entity_children(self, entity, allow_query=True):
+        children_ids = entity.get_children_ids(allow_query=False)
+        if children_ids is not UNKNOWN_VALUE:
+            return entity.get_children()
+
+        if children_ids is UNKNOWN_VALUE and not allow_query:
+            return UNKNOWN_VALUE
+
+        self._query_entity_children(entity)
+
+        return entity.get_children()
+
+    def delete_entity(self, entity):
+        parent_id = entity.parent_id
+        if parent_id is None:
+            return
+
+        parent = self._entities_by_id.get(parent_id)
+        if parent is not None:
+            parent.remove_child(entity.id)
+
+    def reset_immutable_for_hierarchy_cache(
+        self, entity_id, bottom_to_top=True
+    ):
+        if bottom_to_top is None or entity_id is None:
+            return
+
+        reset_queue = collections.deque()
+        reset_queue.append(entity_id)
+        if bottom_to_top:
+            while reset_queue:
+                entity_id = reset_queue.popleft()
+                entity = self.get_entity_by_id(entity_id)
+                if entity is None:
+                    continue
+                entity.reset_immutable_for_hierarchy_cache(None)
+                reset_queue.append(entity.parent_id)
+        else:
+            while reset_queue:
+                entity_id = reset_queue.popleft()
+                entity = self.get_entity_by_id(entity_id)
+                if entity is None:
+                    continue
+                entity.reset_immutable_for_hierarchy_cache(None)
+                for child in self._entities_by_parent_id[entity.id]:
+                    reset_queue.append(child.id)
+
+    def fill_project_from_server(self):
+        """Query project data from server and create project entity.
+
+        This method will invalidate previous object of Project entity.
+
+        Returns:
+            ProjectEntity: Entity that was updated with server data.
+
+        Raises:
+            ValueError: When project was not found on server.
+        """
+
+        project_name = self.project_name
+        project = self._connection.get_project(
+            project_name,
+            own_attributes=True
+        )
+        if not project:
+            raise ValueError(
+                "Project \"{}\" was not found.".format(project_name)
+            )
+
+        self._project_entity = ProjectEntity(
+            project["code"],
+            parent_id=PROJECT_PARENT_ID,
+            entity_id=project["name"],
+            library=project["library"],
+            folder_types=project["folderTypes"],
+            task_types=project["taskTypes"],
+            name=project["name"],
+            attribs=project["ownAttrib"],
+            data=project["data"],
+            active=project["active"],
+            entity_hub=self
+        )
+        self.add_entity(self._project_entity)
+        return self._project_entity
+
+    def _get_folder_fields(self):
+        folder_fields = set(
+            self._connection.get_default_fields_for_type("folder")
+        )
+        folder_fields.add("hasProducts")
+        if self._allow_data_changes:
+            folder_fields.add("data")
+        return folder_fields
+
+    def query_entities_from_server(self):
+        """Query whole project at once."""
+
+        project_entity = self.fill_project_from_server()
+
+        folder_fields = self._get_folder_fields()
+
+        folders = self._connection.get_folders(
+            project_entity.name,
+            fields=folder_fields,
+            own_attributes=True
+        )
+        tasks = self._connection.get_tasks(
+            project_entity.name,
+            own_attributes=True
+        )
+        folders_by_parent_id = collections.defaultdict(list)
+        for folder in folders:
+            parent_id = folder["parentId"]
+            folders_by_parent_id[parent_id].append(folder)
+
+        tasks_by_parent_id = collections.defaultdict(list)
+        for task in tasks:
+            parent_id = task["folderId"]
+            tasks_by_parent_id[parent_id].append(task)
+
+        lock_queue = collections.deque()
+        hierarchy_queue = collections.deque()
+        hierarchy_queue.append((None, project_entity))
+        while hierarchy_queue:
+            item = hierarchy_queue.popleft()
+            parent_id, parent_entity = item
+
+            lock_queue.append(parent_entity)
+
+            children_ids = set()
+            for folder in folders_by_parent_id[parent_id]:
+                folder_entity = self.add_folder(folder)
+                children_ids.add(folder_entity.id)
+                folder_entity.has_published_content = folder["hasProducts"]
+                hierarchy_queue.append((folder_entity.id, folder_entity))
+
+            for task in tasks_by_parent_id[parent_id]:
+                task_entity = self.add_task(task)
+                lock_queue.append(task_entity)
+                children_ids.add(task_entity.id)
+
+            parent_entity.fill_children_ids(children_ids)
+
+        # Lock entities when all are added to hub
+        # - lock only entities added in this method
+        while lock_queue:
+            entity = lock_queue.popleft()
+            entity.lock()
+
+    def lock(self):
+        if self._project_entity is None:
+            return
+
+        for entity in self._entities_by_id.values():
+            entity.lock()
+
+    def _get_top_entities(self):
+        all_ids = set(self._entities_by_id.keys())
+        return [
+            entity
+            for entity in self._entities_by_id.values()
+            if entity.parent_id not in all_ids
+        ]
+
+    def _split_entities(self):
+        top_entities = self._get_top_entities()
+        entities_queue = collections.deque(top_entities)
+        removed_entity_ids = []
+        created_entity_ids = []
+        other_entity_ids = []
+        while entities_queue:
+            entity = entities_queue.popleft()
+            removed = entity.removed
+            if removed:
+                removed_entity_ids.append(entity.id)
+            elif entity.created:
+                created_entity_ids.append(entity.id)
+            else:
+                other_entity_ids.append(entity.id)
+
+            for child in tuple(self._entities_by_parent_id[entity.id]):
+                if removed:
+                    self.unset_entity_parent(child.id, entity.id)
+                entities_queue.append(child)
+        return created_entity_ids, other_entity_ids, removed_entity_ids
+
+    def _get_update_body(self, entity, changes=None):
+        if changes is None:
+            changes = entity.changes
+
+        if not changes:
+            return None
+        return {
+            "type": "update",
+            "entityType": entity.entity_type,
+            "entityId": entity.id,
+            "data": changes
+        }
+
+    def _get_create_body(self, entity):
+        return {
+            "type": "create",
+            "entityType": entity.entity_type,
+            "entityId": entity.id,
+            "data": entity.to_create_body_data()
+        }
+
+    def _get_delete_body(self, entity):
+        return {
+            "type": "delete",
+            "entityType": entity.entity_type,
+            "entityId": entity.id
+        }
+
+    def commit_changes(self):
+        """Commit any changes that happened on entities.
+
+        Todos:
+            Use Operations Session instead of known operations body.
+        """
+
+        project_changes = self.project_entity.changes
+        if project_changes:
+            response = self._connection.patch(
+                "projects/{}".format(self.project_name),
+                **project_changes
+            )
+            if response.status_code != 204:
+                raise ValueError("Failed to update project")
+
+        self.project_entity.lock()
+
+        operations_body = []
+
+        created_entity_ids, other_entity_ids, removed_entity_ids = (
+            self._split_entities()
+        )
+        processed_ids = set()
+        for entity_id in other_entity_ids:
+            if entity_id in processed_ids:
+                continue
+
+            entity = self._entities_by_id[entity_id]
+            changes = entity.changes
+            processed_ids.add(entity_id)
+            if not changes:
+                continue
+
+            bodies = [self._get_update_body(entity, changes)]
+            # Parent was created and was not yet added to operations body
+            parent_queue = collections.deque()
+            parent_queue.append(entity.parent_id)
+            while parent_queue:
+                # Make sure entity's parents are created
+                parent_id = parent_queue.popleft()
+                if (
+                    parent_id is UNKNOWN_VALUE
+                    or parent_id in processed_ids
+                    or parent_id not in created_entity_ids
+                ):
+                    continue
+
+                parent = self._entities_by_id.get(parent_id)
+                processed_ids.add(parent.id)
+                bodies.append(self._get_create_body(parent))
+                parent_queue.append(parent.id)
+
+            operations_body.extend(reversed(bodies))
+
+        for entity_id in created_entity_ids:
+            if entity_id in processed_ids:
+                continue
+            entity = self._entities_by_id[entity_id]
+            processed_ids.add(entity_id)
+            operations_body.append(self._get_create_body(entity))
+
+        for entity_id in reversed(removed_entity_ids):
+            if entity_id in processed_ids:
+                continue
+
+            entity = self._entities_by_id.pop(entity_id)
+            parent_children = self._entities_by_parent_id[entity.parent_id]
+            if entity in parent_children:
+                parent_children.remove(entity)
+
+            if not entity.created:
+                operations_body.append(self._get_delete_body(entity))
+
+        self._connection.send_batch_operations(
+            self.project_name, operations_body
+        )
+
+        self.lock()
+
+
+class AttributeValue(object):
+    def __init__(self, value):
+        self._value = value
+        self._origin_value = copy.deepcopy(value)
+
+    def get_value(self):
+        return self._value
+
+    def set_value(self, value):
+        self._value = value
+
+    value = property(get_value, set_value)
+
+    @property
+    def changed(self):
+        return self._value != self._origin_value
+
+    def lock(self):
+        self._origin_value = copy.deepcopy(self._value)
+
+
+class Attributes(object):
+    """Object representing attribs of entity.
+
+    Todos:
+        This could be enhanced to know attribute schema and validate values
+        based on the schema.
+
+    Args:
+        attrib_keys (Iterable[str]): Keys that are available in attribs of the
+            entity.
+        values (Union[None, Dict[str, Any]]): Values of attributes.
+    """
+
+    def __init__(self, attrib_keys, values=UNKNOWN_VALUE):
+        if values in (UNKNOWN_VALUE, None):
+            values = {}
+        self._attributes = {
+            key: AttributeValue(values.get(key))
+            for key in attrib_keys
+        }
+
+    def __contains__(self, key):
+        return key in self._attributes
+
+    def __getitem__(self, key):
+        return self._attributes[key].value
+
+    def __setitem__(self, key, value):
+        self._attributes[key].set_value(value)
+
+    def __iter__(self):
+        for key in self._attributes:
+            yield key
+
+    def keys(self):
+        return self._attributes.keys()
+
+    def values(self):
+        for attribute in self._attributes.values():
+            yield attribute.value
+
+    def items(self):
+        for key, attribute in self._attributes.items():
+            yield key, attribute.value
+
+    def get(self, key, default=None):
+        """Get value of attribute.
+
+        Args:
+            key (str): Attribute name.
+            default (Any): Default value to return when attribute was not
+                found.
+        """
+
+        attribute = self._attributes.get(key)
+        if attribute is None:
+            return default
+        return attribute.value
+
+    def set(self, key, value):
+        """Change value of attribute.
+
+        Args:
+            key (str): Attribute name.
+            value (Any): New value of the attribute.
+        """
+
+        self[key] = value
+
+    def get_attribute(self, key):
+        """Access to attribute object.
+
+        Args:
+            key (str): Name of attribute.
+
+        Returns:
+            AttributeValue: Object of attribute value.
+
+        Raises:
+            KeyError: When attribute is not available.
+        """
+
+        return self._attributes[key]
+
+    def lock(self):
+        for attribute in self._attributes.values():
+            attribute.lock()
+
+    @property
+    def changes(self):
+        """Attribute value changes.
+
+        Returns:
+            Dict[str, Any]: Key mapping with new values.
+        """
+
+        return {
+            attr_key: attribute.value
+            for attr_key, attribute in self._attributes.items()
+            if attribute.changed
+        }
+
+    def to_dict(self, ignore_none=True):
+        output = {}
+        for key, value in self.items():
+            if (
+                value is UNKNOWN_VALUE
+                or (ignore_none and value is None)
+            ):
+                continue
+
+            output[key] = value
+        return output
+
+
+@six.add_metaclass(ABCMeta)
+class BaseEntity(object):
+    """Object representation of entity from server which is capturing changes.
+
+    All data on created object are expected as "current data" on server entity
+    unless the entity has set 'created' to 'True'. So if new data should be
+    stored to server entity then fill entity with server data first and
+    then change them.
+
+    Calling 'lock' method will mark entity as "saved" and all changes made on
+    entity are set as "current data" on server.
+
+    Args:
+        entity_id (Union[str, None]): Id of the entity. New id is created if
+            not passed.
+        parent_id (Union[str, None]): Id of parent entity.
+        name (str): Name of entity.
+        attribs (Dict[str, Any]): Attribute values.
+        data (Dict[str, Any]): Entity data (custom data).
+        thumbnail_id (Union[str, None]): Id of entity's thumbnail.
+        active (bool): Is entity active.
+        entity_hub (EntityHub): Object of entity hub which created object of
+            the entity.
+        created (Optional[bool]): Entity is new. When 'None' is passed the
+            value is defined based on value of 'entity_id'.
+    """
+
+    def __init__(
+        self,
+        entity_id=None,
+        parent_id=UNKNOWN_VALUE,
+        name=UNKNOWN_VALUE,
+        attribs=UNKNOWN_VALUE,
+        data=UNKNOWN_VALUE,
+        thumbnail_id=UNKNOWN_VALUE,
+        active=UNKNOWN_VALUE,
+        entity_hub=None,
+        created=None
+    ):
+        if entity_hub is None:
+            raise ValueError("Missing required kwarg 'entity_hub'")
+
+        self._entity_hub = entity_hub
+
+        if created is None:
+            created = entity_id is None
+
+        entity_id = self._prepare_entity_id(entity_id)
+
+        if data is None:
+            data = {}
+
+        children_ids = UNKNOWN_VALUE
+        if created:
+            children_ids = set()
+
+        if not created and parent_id is UNKNOWN_VALUE:
+            raise ValueError("Existing entity is missing parent id.")
+
+        # These are public without any validation at this moment
+        #   may change in future (e.g. name will have regex validation)
+        self._entity_id = entity_id
+
+        self._parent_id = parent_id
+        self._name = name
+        self.active = active
+        self._created = created
+        self._thumbnail_id = thumbnail_id
+        self._attribs = Attributes(
+            self._get_attributes_for_type(self.entity_type),
+            attribs
+        )
+        self._data = data
+        self._children_ids = children_ids
+
+        self._orig_parent_id = parent_id
+        self._orig_name = name
+        self._orig_data = copy.deepcopy(data)
+        self._orig_thumbnail_id = thumbnail_id
+        self._orig_active = active
+
+        self._immutable_for_hierarchy_cache = None
+
+    def __repr__(self):
+        return "<{} - {}>".format(self.__class__.__name__, self.id)
+
+    def __getitem__(self, item):
+        return getattr(self, item)
+
+    def __setitem__(self, item, value):
+        return setattr(self, item, value)
+
+    def _prepare_entity_id(self, entity_id):
+        entity_id = convert_entity_id(entity_id)
+        if entity_id is None:
+            entity_id = create_entity_id()
+        return entity_id
+
+    @property
+    def id(self):
+        """Access to entity id under which is entity available on server.
+
+        Returns:
+            str: Entity id.
+        """
+
+        return self._entity_id
+
+    @property
+    def removed(self):
+        return self._parent_id is None
+
+    @property
+    def orig_parent_id(self):
+        return self._orig_parent_id
+
+    @property
+    def attribs(self):
+        """Entity attributes based on server configuration.
+
+        Returns:
+            Attributes: Attributes object handling changes and values of
+                attributes on entity.
+        """
+
+        return self._attribs
+
+    @property
+    def data(self):
+        """Entity custom data that are not stored by any deterministic model.
+
+        Be aware that 'data' can't be queried using GraphQl and cannot be
+            updated partially.
+
+        Returns:
+            Dict[str, Any]: Custom data on entity.
+        """
+
+        return self._data
+
+    @property
+    def project_name(self):
+        """Quick access to project from entity hub.
+
+        Returns:
+            str: Name of project under which entity lives.
+        """
+
+        return self._entity_hub.project_name
+
+    @property
+    @abstractmethod
+    def entity_type(self):
+        """Entity type coresponding to server.
+
+        Returns:
+            Literal[project, folder, task]: Entity type.
+        """
+
+        pass
+
+    @property
+    @abstractmethod
+    def parent_entity_types(self):
+        """Entity type coresponding to server.
+
+        Returns:
+            Iterable[str]: Possible entity types of parent.
+        """
+
+        pass
+
+    @property
+    @abstractmethod
+    def changes(self):
+        """Receive entity changes.
+
+        Returns:
+            Union[Dict[str, Any], None]: All values that have changed on
+                entity. New entity must return None.
+        """
+
+        pass
+
+    @classmethod
+    @abstractmethod
+    def from_entity_data(cls, entity_data, entity_hub):
+        """Create entity based on queried data from server.
+
+        Args:
+            entity_data (Dict[str, Any]): Entity data from server.
+            entity_hub (EntityHub): Hub which handle the entity.
+
+        Returns:
+            BaseEntity: Object of the class.
+        """
+
+        pass
+
+    @abstractmethod
+    def to_create_body_data(self):
+        """Convert object of entity to data for server on creation.
+
+        Returns:
+            Dict[str, Any]: Entity data.
+        """
+
+        pass
+
+    @property
+    def immutable_for_hierarchy(self):
+        """Entity is immutable for hierarchy changes.
+
+        Hierarchy changes can be considered as change of name or parents.
+
+        Returns:
+            bool: Entity is immutable for hierarchy changes.
+        """
+
+        if self._immutable_for_hierarchy_cache is not None:
+            return self._immutable_for_hierarchy_cache
+
+        immutable_for_hierarchy = self._immutable_for_hierarchy
+        if immutable_for_hierarchy is not None:
+            self._immutable_for_hierarchy_cache = immutable_for_hierarchy
+            return self._immutable_for_hierarchy_cache
+
+        for child in self._entity_hub.get_entity_children(self):
+            if child.immutable_for_hierarchy:
+                self._immutable_for_hierarchy_cache = True
+                return self._immutable_for_hierarchy_cache
+
+        self._immutable_for_hierarchy_cache = False
+        return self._immutable_for_hierarchy_cache
+
+    @property
+    def _immutable_for_hierarchy(self):
+        """Override this method to define if entity object is immutable.
+
+        This property was added to define immutable state of Folder entities
+        which is used in property 'immutable_for_hierarchy'.
+
+        Returns:
+            Union[bool, None]: Bool to explicitly telling if is immutable or
+                not otherwise None.
+        """
+
+        return None
+
+    @property
+    def has_cached_immutable_hierarchy(self):
+        return self._immutable_for_hierarchy_cache is not None
+
+    def reset_immutable_for_hierarchy_cache(self, bottom_to_top=True):
+        """Clear cache of immutable hierarchy property.
+
+        This is used when entity changed parent or a child was added.
+
+        Args:
+            bottom_to_top (bool): Reset cache from top hierarchy to bottom or
+                from bottom hierarchy to top.
+        """
+
+        self._immutable_for_hierarchy_cache = None
+        self._entity_hub.reset_immutable_for_hierarchy_cache(
+            self.id, bottom_to_top
+        )
+
+    def _get_default_changes(self):
+        """Collect changes of common data on entity.
+
+        Returns:
+            Dict[str, Any]: Changes on entity. Key and it's new value.
+        """
+
+        changes = {}
+        if self._orig_name != self._name:
+            changes["name"] = self._name
+
+        if self._entity_hub.allow_data_changes:
+            if self._orig_data != self._data:
+                changes["data"] = self._data
+
+        if self._orig_thumbnail_id != self._thumbnail_id:
+            changes["thumbnailId"] = self._thumbnail_id
+
+        if self._orig_active != self.active:
+            changes["active"] = self.active
+
+        attrib_changes = self.attribs.changes
+        if attrib_changes:
+            changes["attrib"] = attrib_changes
+        return changes
+
+    def _get_attributes_for_type(self, entity_type):
+        return self._entity_hub.get_attributes_for_type(entity_type)
+
+    def lock(self):
+        """Lock entity as 'saved' so all changes are discarded."""
+
+        self._orig_parent_id = self._parent_id
+        self._orig_name = self._name
+        self._orig_data = copy.deepcopy(self._data)
+        self._orig_thumbnail_id = self.thumbnail_id
+        self._attribs.lock()
+
+        self._immutable_for_hierarchy_cache = None
+        self._created = False
+
+    def _get_entity_by_id(self, entity_id):
+        return self._entity_hub.get_entity_by_id(entity_id)
+
+    def get_name(self):
+        return self._name
+
+    def set_name(self, name):
+        self._name = name
+
+    name = property(get_name, set_name)
+
+    def get_parent_id(self):
+        """Parent entity id.
+
+        Returns:
+            Union[str, None]: Id of parent entity or none if is not set.
+        """
+
+        return self._parent_id
+
+    def set_parent_id(self, parent_id):
+        """Change parent by id.
+
+        Args:
+            parent_id (Union[str, None]): Id of new parent for entity.
+
+        Raises:
+            ValueError: If parent was not found by id.
+            TypeError: If validation of parent does not pass.
+        """
+
+        if parent_id != self._parent_id:
+            orig_parent_id = self._parent_id
+            self._parent_id = parent_id
+            self._entity_hub.set_entity_parent(
+                self.id, parent_id, orig_parent_id
+            )
+
+    parent_id = property(get_parent_id, set_parent_id)
+
+    def get_parent(self, allow_query=True):
+        """Parent entity.
+
+        Returns:
+            Union[BaseEntity, None]: Parent object.
+        """
+
+        parent = self._entity_hub.get_entity_by_id(self._parent_id)
+        if parent is not None:
+            return parent
+
+        if not allow_query:
+            return self._parent_id
+
+        if self._parent_id is UNKNOWN_VALUE:
+            return self._parent_id
+
+        return self._entity_hub.get_or_query_entity_by_id(
+            self._parent_id, self.parent_entity_types
+        )
+
+    def set_parent(self, parent):
+        """Change parent object.
+
+        Args:
+            parent (BaseEntity): New parent for entity.
+
+        Raises:
+            TypeError: If validation of parent does not pass.
+        """
+
+        parent_id = None
+        if parent is not None:
+            parent_id = parent.id
+        self._entity_hub.set_entity_parent(self.id, parent_id)
+
+    parent = property(get_parent, set_parent)
+
+    def get_children_ids(self, allow_query=True):
+        """Access to children objects.
+
+        Todos:
+            Children should be maybe handled by EntityHub instead of entities
+                themselves. That would simplify 'set_entity_parent',
+                'unset_entity_parent' and other logic related to changing
+                hierarchy.
+
+        Returns:
+            Union[List[str], Type[UNKNOWN_VALUE]]: Children iterator.
+        """
+
+        if self._children_ids is UNKNOWN_VALUE:
+            if not allow_query:
+                return self._children_ids
+            self._entity_hub.get_entity_children(self, True)
+        return set(self._children_ids)
+
+    children_ids = property(get_children_ids)
+
+    def get_children(self, allow_query=True):
+        """Access to children objects.
+
+        Returns:
+            Union[List[BaseEntity], Type[UNKNOWN_VALUE]]: Children iterator.
+        """
+
+        if self._children_ids is UNKNOWN_VALUE:
+            if not allow_query:
+                return self._children_ids
+            return self._entity_hub.get_entity_children(self, True)
+
+        return [
+            self._entity_hub.get_entity_by_id(children_id)
+            for children_id in self._children_ids
+        ]
+
+    children = property(get_children)
+
+    def add_child(self, child):
+        """Add child entity.
+
+        Args:
+            child (BaseEntity): Child object to add.
+
+        Raises:
+            TypeError: When child object has invalid type to be children.
+        """
+
+        child_id = child
+        if isinstance(child_id, BaseEntity):
+            child_id = child.id
+
+        if self._children_ids is not UNKNOWN_VALUE:
+            self._children_ids.add(child_id)
+
+        self._entity_hub.set_entity_parent(child_id, self.id)
+
+    def remove_child(self, child):
+        """Remove child entity.
+
+        Is ignored if child is not in children.
+
+        Args:
+            child (Union[str, BaseEntity]): Child object or child id to remove.
+        """
+
+        child_id = child
+        if isinstance(child_id, BaseEntity):
+            child_id = child.id
+
+        if self._children_ids is not UNKNOWN_VALUE:
+            self._children_ids.discard(child_id)
+        self._entity_hub.unset_entity_parent(child_id, self.id)
+
+    def get_thumbnail_id(self):
+        """Thumbnail id of entity.
+
+        Returns:
+            Union[str, None]: Id of parent entity or none if is not set.
+        """
+
+        return self._thumbnail_id
+
+    def set_thumbnail_id(self, thumbnail_id):
+        """Change thumbnail id.
+
+        Args:
+            thumbnail_id (Union[str, None]): Id of thumbnail for entity.
+        """
+
+        self._thumbnail_id = thumbnail_id
+
+    thumbnail_id = property(get_thumbnail_id, set_thumbnail_id)
+
+    @property
+    def created(self):
+        """Entity is new.
+
+        Returns:
+            bool: Entity is newly created.
+        """
+
+        return self._created
+
+    def fill_children_ids(self, children_ids):
+        """Fill children ids on entity.
+
+        Warning:
+            This is not an api call but is called from entity hub.
+        """
+
+        self._children_ids = set(children_ids)
+
+
+class ProjectEntity(BaseEntity):
+    """Entity representing project on AYON server.
+
+    Args:
+        project_code (str): Project code.
+        library (bool): Is project library project.
+        folder_types (list[dict[str, Any]]): Folder types definition.
+        task_types (list[dict[str, Any]]): Task types definition.
+        entity_id (Optional[str]): Id of the entity. New id is created if
+            not passed.
+        parent_id (Union[str, None]): Id of parent entity.
+        name (str): Name of entity.
+        attribs (Dict[str, Any]): Attribute values.
+        data (Dict[str, Any]): Entity data (custom data).
+        thumbnail_id (Union[str, None]): Id of entity's thumbnail.
+        active (bool): Is entity active.
+        entity_hub (EntityHub): Object of entity hub which created object of
+            the entity.
+        created (Optional[bool]): Entity is new. When 'None' is passed the
+            value is defined based on value of 'entity_id'.
+    """
+
+    entity_type = "project"
+    parent_entity_types = []
+    # TODO These are hardcoded but maybe should be used from server???
+    default_folder_type_icon = "folder"
+    default_task_type_icon = "task_alt"
+
+    def __init__(
+        self, project_code, library, folder_types, task_types, *args, **kwargs
+    ):
+        super(ProjectEntity, self).__init__(*args, **kwargs)
+
+        self._project_code = project_code
+        self._library_project = library
+        self._folder_types = folder_types
+        self._task_types = task_types
+
+        self._orig_project_code = project_code
+        self._orig_library_project = library
+        self._orig_folder_types = copy.deepcopy(folder_types)
+        self._orig_task_types = copy.deepcopy(task_types)
+
+    def _prepare_entity_id(self, entity_id):
+        if entity_id != self.project_name:
+            raise ValueError(
+                "Unexpected entity id value \"{}\". Expected \"{}\"".format(
+                    entity_id, self.project_name))
+        return entity_id
+
+    def get_parent(self, *args, **kwargs):
+        return None
+
+    def set_parent(self, parent):
+        raise ValueError(
+            "Parent of project cannot be set to {}".format(parent)
+        )
+
+    parent = property(get_parent, set_parent)
+
+    def get_folder_types(self):
+        return copy.deepcopy(self._folder_types)
+
+    def set_folder_types(self, folder_types):
+        new_folder_types = []
+        for folder_type in folder_types:
+            if "icon" not in folder_type:
+                folder_type["icon"] = self.default_folder_type_icon
+            new_folder_types.append(folder_type)
+        self._folder_types = new_folder_types
+
+    def get_task_types(self):
+        return copy.deepcopy(self._task_types)
+
+    def set_task_types(self, task_types):
+        new_task_types = []
+        for task_type in task_types:
+            if "icon" not in task_type:
+                task_type["icon"] = self.default_task_type_icon
+            new_task_types.append(task_type)
+        self._task_types = new_task_types
+
+    folder_types = property(get_folder_types, set_folder_types)
+    task_types = property(get_task_types, set_task_types)
+
+    def lock(self):
+        super(ProjectEntity, self).lock()
+        self._orig_folder_types = copy.deepcopy(self._folder_types)
+        self._orig_task_types = copy.deepcopy(self._task_types)
+
+    @property
+    def changes(self):
+        changes = self._get_default_changes()
+        if self._orig_folder_types != self._folder_types:
+            changes["folderTypes"] = self.get_folder_types()
+
+        if self._orig_task_types != self._task_types:
+            changes["taskTypes"] = self.get_task_types()
+
+        return changes
+
+    @classmethod
+    def from_entity_data(cls, project, entity_hub):
+        return cls(
+            project["code"],
+            parent_id=PROJECT_PARENT_ID,
+            entity_id=project["name"],
+            library=project["library"],
+            folder_types=project["folderTypes"],
+            task_types=project["taskTypes"],
+            name=project["name"],
+            attribs=project["ownAttrib"],
+            data=project["data"],
+            active=project["active"],
+            entity_hub=entity_hub
+        )
+
+    def to_create_body_data(self):
+        raise NotImplementedError(
+            "ProjectEntity does not support conversion to entity data"
+        )
+
+
+class FolderEntity(BaseEntity):
+    """Entity representing a folder on AYON server.
+
+    Args:
+        folder_type (str): Type of folder. Folder type must be available in
+            config of project folder types.
+        entity_id (Union[str, None]): Id of the entity. New id is created if
+            not passed.
+        parent_id (Union[str, None]): Id of parent entity.
+        name (str): Name of entity.
+        attribs (Dict[str, Any]): Attribute values.
+        data (Dict[str, Any]): Entity data (custom data).
+        thumbnail_id (Union[str, None]): Id of entity's thumbnail.
+        active (bool): Is entity active.
+        label (Optional[str]): Folder label.
+        path (Optional[str]): Folder path. Path consist of all parent names
+            with slash('/') used as separator.
+        entity_hub (EntityHub): Object of entity hub which created object of
+            the entity.
+        created (Optional[bool]): Entity is new. When 'None' is passed the
+            value is defined based on value of 'entity_id'.
+    """
+
+    entity_type = "folder"
+    parent_entity_types = ["folder", "project"]
+
+    def __init__(self, folder_type, *args, label=None, path=None, **kwargs):
+        super(FolderEntity, self).__init__(*args, **kwargs)
+        # Autofill project as parent of folder if is not yet set
+        # - this can be guessed only if folder was just created
+        if self.created and self._parent_id is UNKNOWN_VALUE:
+            self._parent_id = self.project_name
+
+        self._folder_type = folder_type
+        self._label = label
+
+        self._orig_folder_type = folder_type
+        self._orig_label = label
+        # Know if folder has any products
+        # - is used to know if folder allows hierarchy changes
+        self._has_published_content = False
+        self._path = path
+
+    def get_folder_type(self):
+        return self._folder_type
+
+    def set_folder_type(self, folder_type):
+        self._folder_type = folder_type
+
+    folder_type = property(get_folder_type, set_folder_type)
+
+    def get_label(self):
+        return self._label
+
+    def set_label(self, label):
+        self._label = label
+
+    label = property(get_label, set_label)
+
+    def get_path(self, dynamic_value=True):
+        if not dynamic_value:
+            return self._path
+
+        if self._path is None:
+            parent = self.parent
+            path = self.name
+            if parent.entity_type == "folder":
+                parent_path = parent.path
+                path = "/".join([parent_path, path])
+            self._path = path
+        return self._path
+
+    def reset_path(self):
+        self._path = None
+        self._entity_hub.folder_path_reseted(self.id)
+
+    path = property(get_path)
+
+    def get_has_published_content(self):
+        return self._has_published_content
+
+    def set_has_published_content(self, has_published_content):
+        if self._has_published_content is has_published_content:
+            return
+
+        self._has_published_content = has_published_content
+        # Reset immutable cache of parents
+        self._entity_hub.reset_immutable_for_hierarchy_cache(self.id)
+
+    has_published_content = property(
+        get_has_published_content, set_has_published_content
+    )
+
+    @property
+    def _immutable_for_hierarchy(self):
+        if self.has_published_content:
+            return True
+        return None
+
+    def lock(self):
+        super(FolderEntity, self).lock()
+        self._orig_folder_type = self._folder_type
+
+    @property
+    def changes(self):
+        changes = self._get_default_changes()
+
+        if self._orig_parent_id != self._parent_id:
+            parent_id = self._parent_id
+            if parent_id == self.project_name:
+                parent_id = None
+            changes["parentId"] = parent_id
+
+        if self._orig_folder_type != self._folder_type:
+            changes["folderType"] = self._folder_type
+
+        label = self._label
+        if self._name == label:
+            label = None
+
+        if label != self._orig_label:
+            changes["label"] = label
+
+        return changes
+
+    @classmethod
+    def from_entity_data(cls, folder, entity_hub):
+        parent_id = folder["parentId"]
+        if parent_id is None:
+            parent_id = entity_hub.project_entity.id
+        return cls(
+            folder["folderType"],
+            label=folder["label"],
+            path=folder["path"],
+            entity_id=folder["id"],
+            parent_id=parent_id,
+            name=folder["name"],
+            data=folder.get("data"),
+            attribs=folder["ownAttrib"],
+            active=folder["active"],
+            thumbnail_id=folder["thumbnailId"],
+            created=False,
+            entity_hub=entity_hub
+        )
+
+    def to_create_body_data(self):
+        parent_id = self._parent_id
+        if parent_id is UNKNOWN_VALUE:
+            raise ValueError("Folder does not have set 'parent_id'")
+
+        if parent_id == self.project_name:
+            parent_id = None
+
+        if not self.name or self.name is UNKNOWN_VALUE:
+            raise ValueError("Folder does not have set 'name'")
+
+        output = {
+            "name": self.name,
+            "folderType": self.folder_type,
+            "parentId": parent_id,
+        }
+        attrib = self.attribs.to_dict()
+        if attrib:
+            output["attrib"] = attrib
+
+        if self.active is not UNKNOWN_VALUE:
+            output["active"] = self.active
+
+        if self.thumbnail_id is not UNKNOWN_VALUE:
+            output["thumbnailId"] = self.thumbnail_id
+
+        if self._entity_hub.allow_data_changes:
+            output["data"] = self._data
+        return output
+
+
+class TaskEntity(BaseEntity):
+    """Entity representing a task on AYON server.
+
+    Args:
+        task_type (str): Type of task. Task type must be available in config
+            of project task types.
+        entity_id (Union[str, None]): Id of the entity. New id is created if
+            not passed.
+        parent_id (Union[str, None]): Id of parent entity.
+        name (str): Name of entity.
+        label (Optional[str]): Task label.
+        attribs (Dict[str, Any]): Attribute values.
+        data (Dict[str, Any]): Entity data (custom data).
+        thumbnail_id (Union[str, None]): Id of entity's thumbnail.
+        active (bool): Is entity active.
+        entity_hub (EntityHub): Object of entity hub which created object of
+            the entity.
+        created (Optional[bool]): Entity is new. When 'None' is passed the
+            value is defined based on value of 'entity_id'.
+    """
+
+    entity_type = "task"
+    parent_entity_types = ["folder"]
+
+    def __init__(self, task_type, *args, label=None, **kwargs):
+        super(TaskEntity, self).__init__(*args, **kwargs)
+
+        self._task_type = task_type
+        self._label = label
+
+        self._orig_task_type = task_type
+        self._orig_label = label
+
+        self._children_ids = set()
+
+    def lock(self):
+        super(TaskEntity, self).lock()
+        self._orig_task_type = self._task_type
+
+    def get_task_type(self):
+        return self._task_type
+
+    def set_task_type(self, task_type):
+        self._task_type = task_type
+
+    task_type = property(get_task_type, set_task_type)
+
+    def get_label(self):
+        return self._label
+
+    def set_label(self, label):
+        self._label = label
+
+    label = property(get_label, set_label)
+
+    def add_child(self, child):
+        raise ValueError("Task does not support to add children")
+
+    @property
+    def changes(self):
+        changes = self._get_default_changes()
+
+        if self._orig_parent_id != self._parent_id:
+            changes["folderId"] = self._parent_id
+
+        if self._orig_task_type != self._task_type:
+            changes["taskType"] = self._task_type
+
+        label = self._label
+        if self._name == label:
+            label = None
+
+        if label != self._orig_label:
+            changes["label"] = label
+
+        return changes
+
+    @classmethod
+    def from_entity_data(cls, task, entity_hub):
+        return cls(
+            task["taskType"],
+            entity_id=task["id"],
+            label=task["label"],
+            parent_id=task["folderId"],
+            name=task["name"],
+            data=task.get("data"),
+            attribs=task["ownAttrib"],
+            active=task["active"],
+            created=False,
+            entity_hub=entity_hub
+        )
+
+    def to_create_body_data(self):
+        if self.parent_id is UNKNOWN_VALUE:
+            raise ValueError("Task does not have set 'parent_id'")
+
+        output = {
+            "name": self.name,
+            "taskType": self.task_type,
+            "folderId": self.parent_id,
+            "attrib": self.attribs.to_dict(),
+        }
+        attrib = self.attribs.to_dict()
+        if attrib:
+            output["attrib"] = attrib
+
+        if self.active is not UNKNOWN_VALUE:
+            output["active"] = self.active
+
+        if (
+            self._entity_hub.allow_data_changes
+            and self._data is not UNKNOWN_VALUE
+        ):
+            output["data"] = self._data
+        return output
```

### Comparing `ayon-python-api-0.1.9/ayon_api/exceptions.py` & `ayon-python-api-0.2.0/ayon_api/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,107 @@
-import copy
-
-
-class UrlError(Exception):
-    """Url cannot be parsed as url.
-
-    Exception may contain hints of possible fixes of url that can be used in
-    UI if needed.
-    """
-
-    def __init__(self, message, title, hints=None):
-        if hints is None:
-            hints = []
-
-        self.title = title
-        self.hints = hints
-        super(UrlError, self).__init__(message)
-
-
-class ServerError(Exception):
-    pass
-
-
-class UnauthorizedError(ServerError):
-    pass
-
-
-class AuthenticationError(ServerError):
-    pass
-
-
-class ServerNotReached(ServerError):
-    pass
-
-
-class GraphQlQueryFailed(Exception):
-    def __init__(self, errors, query, variables):
-        if variables is None:
-            variables = {}
-
-        error_messages = []
-        for error in errors:
-            msg = error["message"]
-            path = error.get("path")
-            if path:
-                msg += " on item '{}'".format("/".join(path))
-            locations = error.get("locations")
-            if locations:
-                _locations = [
-                    "Line {} Column {}".format(
-                        location["line"], location["column"]
-                    )
-                    for location in locations
-                ]
-
-                msg += " ({})".format(" and ".join(_locations))
-            error_messages.append(msg)
-
-        message = "GraphQl query Failed"
-        if error_messages:
-            message = "{}: {}".format(message, " | ".join(error_messages))
-
-        self.errors = errors
-        self.query = query
-        self.variables = copy.deepcopy(variables)
-        super(GraphQlQueryFailed, self).__init__(message)
-
-
-class MissingEntityError(Exception):
-    pass
-
-
-class ProjectNotFound(MissingEntityError):
-    def __init__(self, project_name, message=None):
-        if not message:
-            message = "Project \"{}\" was not found".format(project_name)
-        self.project_name = project_name
-        super(ProjectNotFound, self).__init__(message)
-
-
-class FolderNotFound(MissingEntityError):
-    def __init__(self, project_name, folder_id, message=None):
-        self.project_name = project_name
-        self.folder_id = folder_id
-        if not message:
-            message = (
-                "Folder with id \"{}\" was not found in project \"{}\""
-            ).format(folder_id, project_name)
-        super(FolderNotFound, self).__init__(message)
-
-
-class FailedOperations(Exception):
-    pass
-
-
-class FailedServiceInit(Exception):
-    pass
+import copy
+
+
+class UrlError(Exception):
+    """Url cannot be parsed as url.
+
+    Exception may contain hints of possible fixes of url that can be used in
+    UI if needed.
+    """
+
+    def __init__(self, message, title, hints=None):
+        if hints is None:
+            hints = []
+
+        self.title = title
+        self.hints = hints
+        super(UrlError, self).__init__(message)
+
+
+class ServerError(Exception):
+    pass
+
+
+class UnauthorizedError(ServerError):
+    pass
+
+
+class AuthenticationError(ServerError):
+    pass
+
+
+class ServerNotReached(ServerError):
+    pass
+
+
+class RequestError(Exception):
+    def __init__(self, message, response):
+        self.response = response
+        super(RequestError, self).__init__(message)
+
+
+class HTTPRequestError(RequestError):
+    pass
+
+
+class GraphQlQueryFailed(Exception):
+    def __init__(self, errors, query, variables):
+        if variables is None:
+            variables = {}
+
+        error_messages = []
+        for error in errors:
+            msg = error["message"]
+            path = error.get("path")
+            if path:
+                msg += " on item '{}'".format("/".join(path))
+            locations = error.get("locations")
+            if locations:
+                _locations = [
+                    "Line {} Column {}".format(
+                        location["line"], location["column"]
+                    )
+                    for location in locations
+                ]
+
+                msg += " ({})".format(" and ".join(_locations))
+            error_messages.append(msg)
+
+        message = "GraphQl query Failed"
+        if error_messages:
+            message = "{}: {}".format(message, " | ".join(error_messages))
+
+        self.errors = errors
+        self.query = query
+        self.variables = copy.deepcopy(variables)
+        super(GraphQlQueryFailed, self).__init__(message)
+
+
+class MissingEntityError(Exception):
+    pass
+
+
+class ProjectNotFound(MissingEntityError):
+    def __init__(self, project_name, message=None):
+        if not message:
+            message = "Project \"{}\" was not found".format(project_name)
+        self.project_name = project_name
+        super(ProjectNotFound, self).__init__(message)
+
+
+class FolderNotFound(MissingEntityError):
+    def __init__(self, project_name, folder_id, message=None):
+        self.project_name = project_name
+        self.folder_id = folder_id
+        if not message:
+            message = (
+                "Folder with id \"{}\" was not found in project \"{}\""
+            ).format(folder_id, project_name)
+        super(FolderNotFound, self).__init__(message)
+
+
+class FailedOperations(Exception):
+    pass
+
+
+class FailedServiceInit(Exception):
+    pass
```

### Comparing `ayon-python-api-0.1.9/ayon_api/graphql.py` & `ayon-python-api-0.2.0/ayon_api/graphql.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,896 +1,983 @@
-import copy
-import numbers
-from abc import ABCMeta, abstractproperty, abstractmethod
-
-import six
-
-from .exceptions import GraphQlQueryFailed
-
-FIELD_VALUE = object()
-
-
-def fields_to_dict(fields):
-    if not fields:
-        return None
-
-    output = {}
-    for field in fields:
-        hierarchy = field.split(".")
-        last = hierarchy.pop(-1)
-        value = output
-        for part in hierarchy:
-            if value is FIELD_VALUE:
-                break
-
-            if part not in value:
-                value[part] = {}
-            value = value[part]
-
-        if value is not FIELD_VALUE:
-            value[last] = FIELD_VALUE
-    return output
-
-
-class QueryVariable(object):
-    """Object representing single varible used in GraphQlQuery.
-
-    Variable definition is in GraphQl query header but it's value is used
-    in fields.
-
-    Args:
-        variable_name (str): Name of variable in query.
-    """
-
-    def __init__(self, variable_name):
-        self._variable_name = variable_name
-        self._name = "${}".format(variable_name)
-
-    @property
-    def name(self):
-        """Name used in field filter."""
-
-        return self._name
-
-    @property
-    def variable_name(self):
-        """Name of variable in query definition."""
-
-        return self._variable_name
-
-    def __hash__(self):
-        return self._name.__hash__()
-
-    def __str__(self):
-        return self._name
-
-    def __format__(self, *args, **kwargs):
-        return self._name.__format__(*args, **kwargs)
-
-
-class GraphQlQuery:
-    """GraphQl query which can have fields to query.
-
-    Single use object which can be used only for one query. Object and children
-    objects keep track about paging and progress.
-
-    Args:
-        name (str): Name of query.
-    """
-
-    offset = 2
-
-    def __init__(self, name):
-        self._name = name
-        self._variables = {}
-        self._children = []
-        self._has_multiple_edge_fields = None
-
-    @property
-    def indent(self):
-        """Indentation for preparation of query string.
-
-        Returns:
-            int: Ident spaces.
-        """
-
-        return 0
-
-    @property
-    def child_indent(self):
-        """Indentation for preparation of query string used by children.
-
-        Returns:
-            int: Ident spaces for children.
-        """
-
-        return self.indent
-
-    @property
-    def need_query(self):
-        """Still need query from server.
-
-        Needed for edges which use pagination.
-
-        Returns:
-            bool: If still need query from server.
-        """
-
-        for child in self._children:
-            if child.need_query:
-                return True
-        return False
-
-    @property
-    def has_multiple_edge_fields(self):
-        if self._has_multiple_edge_fields is None:
-            edge_counter = 0
-            for child in self._children:
-                edge_counter += child.sum_edge_fields(2)
-                if edge_counter > 1:
-                    break
-            self._has_multiple_edge_fields = edge_counter > 1
-
-        return self._has_multiple_edge_fields
-
-    def add_variable(self, key, value_type, value=None):
-        """Add variable to query.
-
-        Args:
-            key (str): Variable name.
-            value_type (str): Type of expected value in variables. This is
-                graphql type e.g. "[String!]", "Int", "Boolean", etc.
-            value (Any): Default value for variable. Can be changed later.
-
-        Returns:
-            QueryVariable: Created variable object.
-
-        Raises:
-            KeyError: If variable was already added before.
-        """
-
-        if key in self._variables:
-            raise KeyError(
-                "Variable \"{}\" was already set with type {}.".format(
-                    key, value_type
-                )
-            )
-
-        variable = QueryVariable(key)
-        self._variables[key] = {
-            "type": value_type,
-            "variable": variable,
-            "value": value
-        }
-        return variable
-
-    def get_variable(self, key):
-        """Variable object.
-
-        Args:
-            key (str): Variable name added to headers.
-
-        Returns:
-            QueryVariable: Variable object used in query string.
-        """
-
-        return self._variables[key]["variable"]
-
-    def get_variable_value(self, key, default=None):
-        """Get Current value of variable.
-
-        Args:
-            key (str): Variable name.
-            default (Any): Default value if variable is available.
-
-        Returns:
-            Any: Variable value.
-        """
-
-        variable_item = self._variables.get(key)
-        if variable_item:
-            return variable_item["value"]
-        return default
-
-    def set_variable_value(self, key, value):
-        """Set value for variable.
-
-        Args:
-            key (str): Variable name under which the value is stored.
-            value (Any): Variable value used in query. Variable is not used
-                if value is 'None'.
-        """
-
-        self._variables[key]["value"] = value
-
-    def get_variables_values(self):
-        """Calculate variable values used that should be used in query.
-
-        Variables with value set to 'None' are skipped.
-
-        Returns:
-            Dict[str, Any]: Variable values by their name.
-        """
-
-        output = {}
-        for key, item in self._variables.items():
-            value = item["value"]
-            if value is not None:
-                output[key] = item["value"]
-
-        return output
-
-    def add_obj_field(self, field):
-        """Add field object to children.
-
-        Args:
-            field (BaseGraphQlQueryField): Add field to query children.
-        """
-
-        if field in self._children:
-            return
-
-        self._children.append(field)
-        field.set_parent(self)
-
-    def add_field(self, name, has_edges=None):
-        """Add field to query.
-
-        Args:
-            name (str): Field name e.g. 'id'.
-            has_edges (bool): Field has edges so it need paging.
-
-        Returns:
-            BaseGraphQlQueryField: Created field object.
-        """
-
-        if has_edges:
-            item = GraphQlQueryEdgeField(name, self)
-        else:
-            item = GraphQlQueryField(name, self)
-        self.add_obj_field(item)
-        return item
-
-    def calculate_query(self):
-        """Calculate query string which is sent to server.
-
-        Returns:
-            str: GraphQl string with variables and headers.
-
-        Raises:
-            ValueError: Query has no fiels.
-        """
-
-        if not self._children:
-            raise ValueError("Missing fields to query")
-
-        variables = []
-        for item in self._variables.values():
-            if item["value"] is None:
-                continue
-
-            variables.append(
-                "{}: {}".format(item["variable"], item["type"])
-            )
-
-        variables_str = ""
-        if variables:
-            variables_str = "({})".format(",".join(variables))
-        header = "query {}{}".format(self._name, variables_str)
-
-        output = []
-        output.append(header + " {")
-        for field in self._children:
-            output.append(field.calculate_query())
-        output.append("}")
-
-        return "\n".join(output)
-
-    def parse_result(self, data, output, progress_data):
-        """Parse data from response for output.
-
-        Output is stored to passed 'output' variable. That's because of paging
-        during which objects must have access to both new and previous values.
-
-        Args:
-            data (Dict[str, Any]): Data received using calculated query.
-            output (Dict[str, Any]): Where parsed data are stored.
-        """
-
-        if not data:
-            return
-
-        for child in self._children:
-            child.parse_result(data, output, progress_data)
-
-    def query(self, con):
-        """Do a query from server.
-
-        Args:
-            con (ServerAPI): Connection to server with 'query' method.
-
-        Returns:
-            Dict[str, Any]: Parsed output from GraphQl query.
-        """
-
-        progress_data = {}
-        output = {}
-        while self.need_query:
-            query_str = self.calculate_query()
-            variables = self.get_variables_values()
-            response = con.query_graphql(
-                query_str,
-                self.get_variables_values()
-            )
-            if response.errors:
-                raise GraphQlQueryFailed(response.errors, query_str, variables)
-            self.parse_result(response.data["data"], output, progress_data)
-
-        return output
-
-    def continuous_query(self, con):
-        """Do a query from server.
-
-        Args:
-            con (ServerAPI): Connection to server with 'query' method.
-
-        Returns:
-            Dict[str, Any]: Parsed output from GraphQl query.
-        """
-
-        progress_data = {}
-        if self.has_multiple_edge_fields:
-            output = {}
-            while self.need_query:
-                query_str = self.calculate_query()
-                variables = self.get_variables_values()
-                response = con.query_graphql(query_str, variables)
-                if response.errors:
-                    raise GraphQlQueryFailed(
-                        response.errors, query_str, variables
-                    )
-                self.parse_result(response.data["data"], output, progress_data)
-
-            yield output
-
-        else:
-            while self.need_query:
-                output = {}
-                query_str = self.calculate_query()
-                variables = self.get_variables_values()
-                response = con.query_graphql(query_str, variables)
-                if response.errors:
-                    raise GraphQlQueryFailed(
-                        response.errors, query_str, variables
-                    )
-
-                self.parse_result(response.data["data"], output, progress_data)
-
-                yield output
-
-
-@six.add_metaclass(ABCMeta)
-class BaseGraphQlQueryField(object):
-    """Field in GraphQl query.
-
-    Args:
-        name (str): Name of field.
-        parent (Union[BaseGraphQlQueryField, GraphQlQuery]): Parent object of a
-            field.
-        has_edges (bool): Field has edges and should handle paging.
-    """
-
-    def __init__(self, name, parent):
-        if isinstance(parent, GraphQlQuery):
-            query_item = parent
-        else:
-            query_item = parent.query_item
-
-        self._name = name
-        self._parent = parent
-
-        self._filters = {}
-
-        self._children = []
-        # Value is changed on first parse of result
-        self._need_query = True
-
-        self._query_item = query_item
-
-        self._path = None
-
-    def __repr__(self):
-        return "<{} {}>".format(self.__class__.__name__, self.path)
-
-    @property
-    def need_query(self):
-        """Still need query from server.
-
-        Needed for edges which use pagination. Look into children values too.
-
-        Returns:
-            bool: If still need query from server.
-        """
-
-        if self._need_query:
-            return True
-
-        for child in self._children:
-            if child.need_query:
-                return True
-        return False
-
-    def sum_edge_fields(self, max_limit=None):
-        """Check how many edge fields query has.
-
-        In case there are multiple edge fields or are nested the query can't
-        yield mid cursor results.
-
-        Args:
-            max_limit (int): Skip rest of counting if counter is bigger then
-                entered number.
-
-        Returns:
-            int: Counter edge fields
-        """
-
-        counter = 0
-        if isinstance(self, GraphQlQueryEdgeField):
-            counter = 1
-
-        for child in self._children:
-            counter += child.sum_edge_fields(max_limit)
-            if max_limit is not None and counter >= max_limit:
-                break
-        return counter
-
-    @property
-    def offset(self):
-        return self._query_item.offset
-
-    @property
-    def indent(self):
-        return self._parent.child_indent + self.offset
-
-    @abstractproperty
-    def child_indent(self):
-        pass
-
-    @property
-    def query_item(self):
-        return self._query_item
-
-    @abstractproperty
-    def has_edges(self):
-        pass
-
-    @property
-    def child_has_edges(self):
-        for child in self._children:
-            if child.has_edges or child.child_has_edges:
-                return True
-        return False
-
-    @property
-    def path(self):
-        """Field path for debugging purposes.
-
-        Returns:
-            str: Field path in query.
-        """
-
-        if self._path is None:
-            if isinstance(self._parent, GraphQlQuery):
-                path = self._name
-            else:
-                path = "/".join((self._parent.path, self._name))
-            self._path = path
-        return self._path
-
-    def reset_cursor(self):
-        for child in self._children:
-            child.reset_cursor()
-
-    def get_variable_value(self, *args, **kwargs):
-        return self._query_item.get_variable_value(*args, **kwargs)
-
-    def set_variable_value(self, *args, **kwargs):
-        return self._query_item.set_variable_value(*args, **kwargs)
-
-    def set_filter(self, key, value):
-        self._filters[key] = value
-
-    def has_filter(self, key):
-        return key in self._filters
-
-    def remove_filter(self, key):
-        self._filters.pop(key, None)
-
-    def set_parent(self, parent):
-        if self._parent is parent:
-            return
-        self._parent = parent
-        parent.add_obj_field(self)
-
-    def add_obj_field(self, field):
-        if field in self._children:
-            return
-
-        self._children.append(field)
-        field.set_parent(self)
-
-    def add_field(self, name, has_edges=None):
-        if has_edges:
-            item = GraphQlQueryEdgeField(name, self)
-        else:
-            item = GraphQlQueryField(name, self)
-        self.add_obj_field(item)
-        return item
-
-    def _filter_value_to_str(self, value):
-        if isinstance(value, QueryVariable):
-            if self.get_variable_value(value.variable_name) is None:
-                return None
-            return str(value)
-
-        if isinstance(value, numbers.Number):
-            return str(value)
-
-        if isinstance(value, six.string_types):
-            return '"{}"'.format(value)
-
-        if isinstance(value, (list, set, tuple)):
-            return "[{}]".format(
-                ", ".join(
-                    self._filter_value_to_str(item)
-                    for item in iter(value)
-                )
-            )
-        raise TypeError(
-            "Unknown type to convert '{}'".format(str(type(value)))
-        )
-
-    def get_filters(self):
-        """Receive filters for item.
-
-        By default just use copy of set filters.
-
-        Returns:
-            Dict[str, Any]: Fields filters.
-        """
-
-        return copy.deepcopy(self._filters)
-
-    def _filters_to_string(self):
-        filters = self.get_filters()
-        if not filters:
-            return ""
-
-        filter_items = []
-        for key, value in filters.items():
-            string_value = self._filter_value_to_str(value)
-            if string_value is None:
-                continue
-
-            filter_items.append("{}: {}".format(key, string_value))
-
-        if not filter_items:
-            return ""
-        return "({})".format(", ".join(filter_items))
-
-    def _fake_children_parse(self):
-        """Mark children as they don't need query."""
-
-        for child in self._children:
-            child.parse_result({}, {}, {})
-
-    @abstractmethod
-    def calculate_query(self):
-        pass
-
-    @abstractmethod
-    def parse_result(self, data, output, progress_data):
-        pass
-
-
-class GraphQlQueryField(BaseGraphQlQueryField):
-    has_edges = False
-
-    @property
-    def child_indent(self):
-        return self.indent
-
-    def parse_result(self, data, output, progress_data):
-        if not isinstance(data, dict):
-            raise TypeError("{} Expected 'dict' type got '{}'".format(
-                self._name, str(type(data))
-            ))
-
-        self._need_query = False
-        value = data.get(self._name)
-        if value is None:
-            self._fake_children_parse()
-            if self._name in data:
-                output[self._name] = None
-            return
-
-        if not self._children:
-            output[self._name] = value
-            return
-
-        output_value = output.get(self._name)
-        if isinstance(value, dict):
-            if output_value is None:
-                output_value = {}
-                output[self._name] = output_value
-
-            for child in self._children:
-                child.parse_result(value, output_value, progress_data)
-            return
-
-        if output_value is None:
-            output_value = []
-            output[self._name] = output_value
-
-        if not value:
-            self._fake_children_parse()
-            return
-
-        diff = len(value) - len(output_value)
-        if diff > 0:
-            for _ in range(diff):
-                output_value.append({})
-
-        for idx, item in enumerate(value):
-            item_value = output_value[idx]
-            for child in self._children:
-                child.parse_result(item, item_value, progress_data)
-
-    def calculate_query(self):
-        offset = self.indent * " "
-        header = "{}{}{}".format(
-            offset,
-            self._name,
-            self._filters_to_string()
-        )
-        if not self._children:
-            return header
-
-        output = []
-        output.append(header + " {")
-
-        output.extend([
-            field.calculate_query()
-            for field in self._children
-        ])
-        output.append(offset + "}")
-
-        return "\n".join(output)
-
-
-class GraphQlQueryEdgeField(BaseGraphQlQueryField):
-    has_edges = True
-
-    def __init__(self, *args, **kwargs):
-        super(GraphQlQueryEdgeField, self).__init__(*args, **kwargs)
-        self._cursor = None
-
-    @property
-    def child_indent(self):
-        offset = self.offset * 2
-        return self.indent + offset
-
-    def reset_cursor(self):
-        # Reset cursor only for edges
-        self._cursor = None
-        self._need_query = True
-
-        super(GraphQlQueryEdgeField, self).reset_cursor()
-
-    def parse_result(self, data, output, progress_data):
-        if not isinstance(data, dict):
-            raise TypeError("{} Expected 'dict' type got '{}'".format(
-                self._name, str(type(data))
-            ))
-
-        value = data.get(self._name)
-        if value is None:
-            self._fake_children_parse()
-            self._need_query = False
-            return
-
-        if self._name in output:
-            node_values = output[self._name]
-        else:
-            node_values = []
-            output[self._name] = node_values
-
-        handle_cursors = self.child_has_edges
-        if handle_cursors:
-            cursor_key = self._get_cursor_key()
-            if cursor_key in progress_data:
-                nodes_by_cursor = progress_data[cursor_key]
-            else:
-                nodes_by_cursor = {}
-                progress_data[cursor_key] = nodes_by_cursor
-
-        page_info = value["pageInfo"]
-        new_cursor = page_info["endCursor"]
-        self._need_query = page_info["hasNextPage"]
-        edges = value["edges"]
-        # Fake result parse
-        if not edges:
-            self._fake_children_parse()
-
-        for edge in edges:
-            if not handle_cursors:
-                edge_value = {}
-                node_values.append(edge_value)
-            else:
-                edge_cursor = edge["cursor"]
-                edge_value = nodes_by_cursor.get(edge_cursor)
-                if edge_value is None:
-                    edge_value = {}
-                    nodes_by_cursor[edge_cursor] = edge_value
-                    node_values.append(edge_value)
-
-            for child in self._children:
-                child.parse_result(edge["node"], edge_value, progress_data)
-
-        if not self._need_query:
-            return
-
-        change_cursor = True
-        for child in self._children:
-            if child.need_query:
-                change_cursor = False
-
-        if change_cursor:
-            for child in self._children:
-                child.reset_cursor()
-            self._cursor = new_cursor
-
-    def _get_cursor_key(self):
-        return "{}/__cursor__".format(self.path)
-
-    def get_filters(self):
-        filters = super(GraphQlQueryEdgeField, self).get_filters()
-
-        filters["first"] = 300
-        if self._cursor:
-            filters["after"] = self._cursor
-        return filters
-
-    def calculate_query(self):
-        if not self._children:
-            raise ValueError("Missing child definitions for edges {}".format(
-                self.path
-            ))
-
-        offset = self.indent * " "
-        header = "{}{}{}".format(
-            offset,
-            self._name,
-            self._filters_to_string()
-        )
-
-        output = []
-        output.append(header + " {")
-
-        edges_offset = offset + self.offset * " "
-        node_offset = edges_offset + self.offset * " "
-        output.append(edges_offset + "edges {")
-        output.append(node_offset + "node {")
-
-        for field in self._children:
-            output.append(
-                field.calculate_query()
-            )
-
-        output.append(node_offset + "}")
-        if self.child_has_edges:
-            output.append(node_offset + "cursor")
-        output.append(edges_offset + "}")
-
-        # Add page information
-        output.append(edges_offset + "pageInfo {")
-        for page_key in (
-            "endCursor",
-            "hasNextPage",
-        ):
-            output.append(node_offset + page_key)
-        output.append(edges_offset + "}")
-        output.append(offset + "}")
-
-        return "\n".join(output)
-
-
-INTROSPECTION_QUERY = """
-  query IntrospectionQuery {
-    __schema {
-      queryType { name }
-      mutationType { name }
-      subscriptionType { name }
-      types {
-        ...FullType
-      }
-      directives {
-        name
-        description
-        locations
-        args {
-          ...InputValue
-        }
-      }
-    }
-  }
-  fragment FullType on __Type {
-    kind
-    name
-    description
-    fields(includeDeprecated: true) {
-      name
-      description
-      args {
-        ...InputValue
-      }
-      type {
-        ...TypeRef
-      }
-      isDeprecated
-      deprecationReason
-    }
-    inputFields {
-      ...InputValue
-    }
-    interfaces {
-      ...TypeRef
-    }
-    enumValues(includeDeprecated: true) {
-      name
-      description
-      isDeprecated
-      deprecationReason
-    }
-    possibleTypes {
-      ...TypeRef
-    }
-  }
-  fragment InputValue on __InputValue {
-    name
-    description
-    type { ...TypeRef }
-    defaultValue
-  }
-  fragment TypeRef on __Type {
-    kind
-    name
-    ofType {
-      kind
-      name
-      ofType {
-        kind
-        name
-        ofType {
-          kind
-          name
-          ofType {
-            kind
-            name
-            ofType {
-              kind
-              name
-              ofType {
-                kind
-                name
-                ofType {
-                  kind
-                  name
-                }
-              }
-            }
-          }
-        }
-      }
-    }
-  }
-"""
+import copy
+import numbers
+from abc import ABCMeta, abstractmethod
+
+import six
+
+from .exceptions import GraphQlQueryFailed
+
+FIELD_VALUE = object()
+
+
+def fields_to_dict(fields):
+    if not fields:
+        return None
+
+    output = {}
+    for field in fields:
+        hierarchy = field.split(".")
+        last = hierarchy.pop(-1)
+        value = output
+        for part in hierarchy:
+            if value is FIELD_VALUE:
+                break
+
+            if part not in value:
+                value[part] = {}
+            value = value[part]
+
+        if value is not FIELD_VALUE:
+            value[last] = FIELD_VALUE
+    return output
+
+
+class QueryVariable(object):
+    """Object representing single varible used in GraphQlQuery.
+
+    Variable definition is in GraphQl query header but it's value is used
+    in fields.
+
+    Args:
+        variable_name (str): Name of variable in query.
+    """
+
+    def __init__(self, variable_name):
+        self._variable_name = variable_name
+        self._name = "${}".format(variable_name)
+
+    @property
+    def name(self):
+        """Name used in field filter."""
+
+        return self._name
+
+    @property
+    def variable_name(self):
+        """Name of variable in query definition."""
+
+        return self._variable_name
+
+    def __hash__(self):
+        return self._name.__hash__()
+
+    def __str__(self):
+        return self._name
+
+    def __format__(self, *args, **kwargs):
+        return self._name.__format__(*args, **kwargs)
+
+
+class GraphQlQuery:
+    """GraphQl query which can have fields to query.
+
+    Single use object which can be used only for one query. Object and children
+    objects keep track about paging and progress.
+
+    Args:
+        name (str): Name of query.
+    """
+
+    offset = 2
+
+    def __init__(self, name):
+        self._name = name
+        self._variables = {}
+        self._children = []
+        self._has_multiple_edge_fields = None
+
+    @property
+    def indent(self):
+        """Indentation for preparation of query string.
+
+        Returns:
+            int: Ident spaces.
+        """
+
+        return 0
+
+    @property
+    def child_indent(self):
+        """Indentation for preparation of query string used by children.
+
+        Returns:
+            int: Ident spaces for children.
+        """
+
+        return self.indent
+
+    @property
+    def need_query(self):
+        """Still need query from server.
+
+        Needed for edges which use pagination.
+
+        Returns:
+            bool: If still need query from server.
+        """
+
+        for child in self._children:
+            if child.need_query:
+                return True
+        return False
+
+    @property
+    def has_multiple_edge_fields(self):
+        if self._has_multiple_edge_fields is None:
+            edge_counter = 0
+            for child in self._children:
+                edge_counter += child.sum_edge_fields(2)
+                if edge_counter > 1:
+                    break
+            self._has_multiple_edge_fields = edge_counter > 1
+
+        return self._has_multiple_edge_fields
+
+    def add_variable(self, key, value_type, value=None):
+        """Add variable to query.
+
+        Args:
+            key (str): Variable name.
+            value_type (str): Type of expected value in variables. This is
+                graphql type e.g. "[String!]", "Int", "Boolean", etc.
+            value (Any): Default value for variable. Can be changed later.
+
+        Returns:
+            QueryVariable: Created variable object.
+
+        Raises:
+            KeyError: If variable was already added before.
+        """
+
+        if key in self._variables:
+            raise KeyError(
+                "Variable \"{}\" was already set with type {}.".format(
+                    key, value_type
+                )
+            )
+
+        variable = QueryVariable(key)
+        self._variables[key] = {
+            "type": value_type,
+            "variable": variable,
+            "value": value
+        }
+        return variable
+
+    def get_variable(self, key):
+        """Variable object.
+
+        Args:
+            key (str): Variable name added to headers.
+
+        Returns:
+            QueryVariable: Variable object used in query string.
+        """
+
+        return self._variables[key]["variable"]
+
+    def get_variable_value(self, key, default=None):
+        """Get Current value of variable.
+
+        Args:
+            key (str): Variable name.
+            default (Any): Default value if variable is available.
+
+        Returns:
+            Any: Variable value.
+        """
+
+        variable_item = self._variables.get(key)
+        if variable_item:
+            return variable_item["value"]
+        return default
+
+    def set_variable_value(self, key, value):
+        """Set value for variable.
+
+        Args:
+            key (str): Variable name under which the value is stored.
+            value (Any): Variable value used in query. Variable is not used
+                if value is 'None'.
+        """
+
+        self._variables[key]["value"] = value
+
+    def get_variables_values(self):
+        """Calculate variable values used that should be used in query.
+
+        Variables with value set to 'None' are skipped.
+
+        Returns:
+            Dict[str, Any]: Variable values by their name.
+        """
+
+        output = {}
+        for key, item in self._variables.items():
+            value = item["value"]
+            if value is not None:
+                output[key] = item["value"]
+
+        return output
+
+    def add_obj_field(self, field):
+        """Add field object to children.
+
+        Args:
+            field (BaseGraphQlQueryField): Add field to query children.
+        """
+
+        if field in self._children:
+            return
+
+        self._children.append(field)
+        field.set_parent(self)
+
+    def add_field_with_edges(self, name):
+        """Add field with edges to query.
+
+        Args:
+            name (str): Field name e.g. 'tasks'.
+
+        Returns:
+            GraphQlQueryEdgeField: Created field object.
+        """
+
+        item = GraphQlQueryEdgeField(name, self)
+        self.add_obj_field(item)
+        return item
+
+    def add_field(self, name):
+        """Add field to query.
+
+        Args:
+            name (str): Field name e.g. 'id'.
+
+        Returns:
+            GraphQlQueryField: Created field object.
+        """
+
+        item = GraphQlQueryField(name, self)
+        self.add_obj_field(item)
+        return item
+
+    def calculate_query(self):
+        """Calculate query string which is sent to server.
+
+        Returns:
+            str: GraphQl string with variables and headers.
+
+        Raises:
+            ValueError: Query has no fiels.
+        """
+
+        if not self._children:
+            raise ValueError("Missing fields to query")
+
+        variables = []
+        for item in self._variables.values():
+            if item["value"] is None:
+                continue
+
+            variables.append(
+                "{}: {}".format(item["variable"], item["type"])
+            )
+
+        variables_str = ""
+        if variables:
+            variables_str = "({})".format(",".join(variables))
+        header = "query {}{}".format(self._name, variables_str)
+
+        output = []
+        output.append(header + " {")
+        for field in self._children:
+            output.append(field.calculate_query())
+        output.append("}")
+
+        return "\n".join(output)
+
+    def parse_result(self, data, output, progress_data):
+        """Parse data from response for output.
+
+        Output is stored to passed 'output' variable. That's because of paging
+        during which objects must have access to both new and previous values.
+
+        Args:
+            data (Dict[str, Any]): Data received using calculated query.
+            output (Dict[str, Any]): Where parsed data are stored.
+        """
+
+        if not data:
+            return
+
+        for child in self._children:
+            child.parse_result(data, output, progress_data)
+
+    def query(self, con):
+        """Do a query from server.
+
+        Args:
+            con (ServerAPI): Connection to server with 'query' method.
+
+        Returns:
+            Dict[str, Any]: Parsed output from GraphQl query.
+        """
+
+        progress_data = {}
+        output = {}
+        while self.need_query:
+            query_str = self.calculate_query()
+            variables = self.get_variables_values()
+            response = con.query_graphql(
+                query_str,
+                self.get_variables_values()
+            )
+            if response.errors:
+                raise GraphQlQueryFailed(response.errors, query_str, variables)
+            self.parse_result(response.data["data"], output, progress_data)
+
+        return output
+
+    def continuous_query(self, con):
+        """Do a query from server.
+
+        Args:
+            con (ServerAPI): Connection to server with 'query' method.
+
+        Returns:
+            Dict[str, Any]: Parsed output from GraphQl query.
+        """
+
+        progress_data = {}
+        if self.has_multiple_edge_fields:
+            output = {}
+            while self.need_query:
+                query_str = self.calculate_query()
+                variables = self.get_variables_values()
+                response = con.query_graphql(query_str, variables)
+                if response.errors:
+                    raise GraphQlQueryFailed(
+                        response.errors, query_str, variables
+                    )
+                self.parse_result(response.data["data"], output, progress_data)
+
+            yield output
+
+        else:
+            while self.need_query:
+                output = {}
+                query_str = self.calculate_query()
+                variables = self.get_variables_values()
+                response = con.query_graphql(query_str, variables)
+                if response.errors:
+                    raise GraphQlQueryFailed(
+                        response.errors, query_str, variables
+                    )
+
+                self.parse_result(response.data["data"], output, progress_data)
+
+                yield output
+
+
+@six.add_metaclass(ABCMeta)
+class BaseGraphQlQueryField(object):
+    """Field in GraphQl query.
+
+    Args:
+        name (str): Name of field.
+        parent (Union[BaseGraphQlQueryField, GraphQlQuery]): Parent object of a
+            field.
+    """
+
+    def __init__(self, name, parent):
+        if isinstance(parent, GraphQlQuery):
+            query_item = parent
+        else:
+            query_item = parent.query_item
+
+        self._name = name
+        self._parent = parent
+
+        self._filters = {}
+
+        self._children = []
+        # Value is changed on first parse of result
+        self._need_query = True
+
+        self._query_item = query_item
+
+        self._path = None
+
+    def __repr__(self):
+        return "<{} {}>".format(self.__class__.__name__, self.path)
+
+    def add_variable(self, key, value_type, value=None):
+        """Add variable to query.
+
+        Args:
+            key (str): Variable name.
+            value_type (str): Type of expected value in variables. This is
+                graphql type e.g. "[String!]", "Int", "Boolean", etc.
+            value (Any): Default value for variable. Can be changed later.
+
+        Returns:
+            QueryVariable: Created variable object.
+
+        Raises:
+            KeyError: If variable was already added before.
+        """
+
+        return self._parent.add_variable(key, value_type, value)
+
+    def get_variable(self, key):
+        """Variable object.
+
+        Args:
+            key (str): Variable name added to headers.
+
+        Returns:
+            QueryVariable: Variable object used in query string.
+        """
+
+        return self._parent.get_variable(key)
+
+    @property
+    def need_query(self):
+        """Still need query from server.
+
+        Needed for edges which use pagination. Look into children values too.
+
+        Returns:
+            bool: If still need query from server.
+        """
+
+        if self._need_query:
+            return True
+
+        for child in self._children_iter():
+            if child.need_query:
+                return True
+        return False
+
+    def _children_iter(self):
+        """Iterate over all children fields of object.
+
+        Returns:
+            Iterator[BaseGraphQlQueryField]: Children fields.
+        """
+
+        for child in self._children:
+            yield child
+
+    def sum_edge_fields(self, max_limit=None):
+        """Check how many edge fields query has.
+
+        In case there are multiple edge fields or are nested the query can't
+        yield mid cursor results.
+
+        Args:
+            max_limit (int): Skip rest of counting if counter is bigger then
+                entered number.
+
+        Returns:
+            int: Counter edge fields
+        """
+
+        counter = 0
+        if isinstance(self, GraphQlQueryEdgeField):
+            counter = 1
+
+        for child in self._children_iter():
+            counter += child.sum_edge_fields(max_limit)
+            if max_limit is not None and counter >= max_limit:
+                break
+        return counter
+
+    @property
+    def offset(self):
+        return self._query_item.offset
+
+    @property
+    def indent(self):
+        return self._parent.child_indent + self.offset
+
+    @property
+    @abstractmethod
+    def child_indent(self):
+        pass
+
+    @property
+    def query_item(self):
+        return self._query_item
+
+    @property
+    @abstractmethod
+    def has_edges(self):
+        pass
+
+    @property
+    def child_has_edges(self):
+        for child in self._children_iter():
+            if child.has_edges or child.child_has_edges:
+                return True
+        return False
+
+    @property
+    def path(self):
+        """Field path for debugging purposes.
+
+        Returns:
+            str: Field path in query.
+        """
+
+        if self._path is None:
+            if isinstance(self._parent, GraphQlQuery):
+                path = self._name
+            else:
+                path = "/".join((self._parent.path, self._name))
+            self._path = path
+        return self._path
+
+    def reset_cursor(self):
+        for child in self._children_iter():
+            child.reset_cursor()
+
+    def get_variable_value(self, *args, **kwargs):
+        return self._query_item.get_variable_value(*args, **kwargs)
+
+    def set_variable_value(self, *args, **kwargs):
+        return self._query_item.set_variable_value(*args, **kwargs)
+
+    def set_filter(self, key, value):
+        self._filters[key] = value
+
+    def has_filter(self, key):
+        return key in self._filters
+
+    def remove_filter(self, key):
+        self._filters.pop(key, None)
+
+    def set_parent(self, parent):
+        if self._parent is parent:
+            return
+        self._parent = parent
+        parent.add_obj_field(self)
+
+    def add_obj_field(self, field):
+        if field in self._children:
+            return
+
+        self._children.append(field)
+        field.set_parent(self)
+
+    def add_field_with_edges(self, name):
+        item = GraphQlQueryEdgeField(name, self)
+        self.add_obj_field(item)
+        return item
+
+    def add_field(self, name):
+        item = GraphQlQueryField(name, self)
+        self.add_obj_field(item)
+        return item
+
+    def _filter_value_to_str(self, value):
+        if isinstance(value, QueryVariable):
+            if self.get_variable_value(value.variable_name) is None:
+                return None
+            return str(value)
+
+        if isinstance(value, numbers.Number):
+            return str(value)
+
+        if isinstance(value, six.string_types):
+            return '"{}"'.format(value)
+
+        if isinstance(value, (list, set, tuple)):
+            return "[{}]".format(
+                ", ".join(
+                    self._filter_value_to_str(item)
+                    for item in iter(value)
+                )
+            )
+        raise TypeError(
+            "Unknown type to convert '{}'".format(str(type(value)))
+        )
+
+    def get_filters(self):
+        """Receive filters for item.
+
+        By default just use copy of set filters.
+
+        Returns:
+            Dict[str, Any]: Fields filters.
+        """
+
+        return copy.deepcopy(self._filters)
+
+    def _filters_to_string(self):
+        filters = self.get_filters()
+        if not filters:
+            return ""
+
+        filter_items = []
+        for key, value in filters.items():
+            string_value = self._filter_value_to_str(value)
+            if string_value is None:
+                continue
+
+            filter_items.append("{}: {}".format(key, string_value))
+
+        if not filter_items:
+            return ""
+        return "({})".format(", ".join(filter_items))
+
+    def _fake_children_parse(self):
+        """Mark children as they don't need query."""
+
+        for child in self._children_iter():
+            child.parse_result({}, {}, {})
+
+    @abstractmethod
+    def calculate_query(self):
+        pass
+
+    @abstractmethod
+    def parse_result(self, data, output, progress_data):
+        pass
+
+
+class GraphQlQueryField(BaseGraphQlQueryField):
+    has_edges = False
+
+    @property
+    def child_indent(self):
+        return self.indent
+
+    def parse_result(self, data, output, progress_data):
+        if not isinstance(data, dict):
+            raise TypeError("{} Expected 'dict' type got '{}'".format(
+                self._name, str(type(data))
+            ))
+
+        self._need_query = False
+        value = data.get(self._name)
+        if value is None:
+            self._fake_children_parse()
+            if self._name in data:
+                output[self._name] = None
+            return
+
+        if not self._children:
+            output[self._name] = value
+            return
+
+        output_value = output.get(self._name)
+        if isinstance(value, dict):
+            if output_value is None:
+                output_value = {}
+                output[self._name] = output_value
+
+            for child in self._children:
+                child.parse_result(value, output_value, progress_data)
+            return
+
+        if output_value is None:
+            output_value = []
+            output[self._name] = output_value
+
+        if not value:
+            self._fake_children_parse()
+            return
+
+        diff = len(value) - len(output_value)
+        if diff > 0:
+            for _ in range(diff):
+                output_value.append({})
+
+        for idx, item in enumerate(value):
+            item_value = output_value[idx]
+            for child in self._children:
+                child.parse_result(item, item_value, progress_data)
+
+    def calculate_query(self):
+        offset = self.indent * " "
+        header = "{}{}{}".format(
+            offset,
+            self._name,
+            self._filters_to_string()
+        )
+        if not self._children:
+            return header
+
+        output = []
+        output.append(header + " {")
+
+        output.extend([
+            field.calculate_query()
+            for field in self._children
+        ])
+        output.append(offset + "}")
+
+        return "\n".join(output)
+
+
+class GraphQlQueryEdgeField(BaseGraphQlQueryField):
+    has_edges = True
+
+    def __init__(self, *args, **kwargs):
+        super(GraphQlQueryEdgeField, self).__init__(*args, **kwargs)
+        self._cursor = None
+        self._edge_children = []
+
+    @property
+    def child_indent(self):
+        offset = self.offset * 2
+        return self.indent + offset
+
+    def _children_iter(self):
+        for child in super(GraphQlQueryEdgeField, self)._children_iter():
+            yield child
+
+        for child in self._edge_children:
+            yield child
+
+    def add_obj_field(self, field):
+        if field in self._edge_children:
+            return
+
+        super(GraphQlQueryEdgeField, self).add_obj_field(field)
+
+    def add_obj_edge_field(self, field):
+        if field in self._edge_children or field in self._children:
+            return
+
+        self._edge_children.append(field)
+        field.set_parent(self)
+
+    def add_edge_field(self, name):
+        item = GraphQlQueryField(name, self)
+        self.add_obj_edge_field(item)
+        return item
+
+    def reset_cursor(self):
+        # Reset cursor only for edges
+        self._cursor = None
+        self._need_query = True
+
+        super(GraphQlQueryEdgeField, self).reset_cursor()
+
+    def parse_result(self, data, output, progress_data):
+        if not isinstance(data, dict):
+            raise TypeError("{} Expected 'dict' type got '{}'".format(
+                self._name, str(type(data))
+            ))
+
+        value = data.get(self._name)
+        if value is None:
+            self._fake_children_parse()
+            self._need_query = False
+            return
+
+        if self._name in output:
+            node_values = output[self._name]
+        else:
+            node_values = []
+            output[self._name] = node_values
+
+        handle_cursors = self.child_has_edges
+        if handle_cursors:
+            cursor_key = self._get_cursor_key()
+            if cursor_key in progress_data:
+                nodes_by_cursor = progress_data[cursor_key]
+            else:
+                nodes_by_cursor = {}
+                progress_data[cursor_key] = nodes_by_cursor
+
+        page_info = value["pageInfo"]
+        new_cursor = page_info["endCursor"]
+        self._need_query = page_info["hasNextPage"]
+        edges = value["edges"]
+        # Fake result parse
+        if not edges:
+            self._fake_children_parse()
+
+        for edge in edges:
+            if not handle_cursors:
+                edge_value = {}
+                node_values.append(edge_value)
+            else:
+                edge_cursor = edge["cursor"]
+                edge_value = nodes_by_cursor.get(edge_cursor)
+                if edge_value is None:
+                    edge_value = {}
+                    nodes_by_cursor[edge_cursor] = edge_value
+                    node_values.append(edge_value)
+
+            for child in self._edge_children:
+                child.parse_result(edge, edge_value, progress_data)
+
+            for child in self._children:
+                child.parse_result(edge["node"], edge_value, progress_data)
+
+        if not self._need_query:
+            return
+
+        change_cursor = True
+        for child in self._children_iter():
+            if child.need_query:
+                change_cursor = False
+
+        if change_cursor:
+            for child in self._children_iter():
+                child.reset_cursor()
+            self._cursor = new_cursor
+
+    def _get_cursor_key(self):
+        return "{}/__cursor__".format(self.path)
+
+    def get_filters(self):
+        filters = super(GraphQlQueryEdgeField, self).get_filters()
+
+        filters["first"] = 300
+        if self._cursor:
+            filters["after"] = self._cursor
+        return filters
+
+    def calculate_query(self):
+        if not self._children and not self._edge_children:
+            raise ValueError("Missing child definitions for edges {}".format(
+                self.path
+            ))
+
+        offset = self.indent * " "
+        header = "{}{}{}".format(
+            offset,
+            self._name,
+            self._filters_to_string()
+        )
+
+        output = []
+        output.append(header + " {")
+
+        edges_offset = offset + self.offset * " "
+        node_offset = edges_offset + self.offset * " "
+        output.append(edges_offset + "edges {")
+        for field in self._edge_children:
+            output.append(field.calculate_query())
+
+        if self._children:
+            output.append(node_offset + "node {")
+
+            for field in self._children:
+                output.append(
+                    field.calculate_query()
+                )
+
+            output.append(node_offset + "}")
+            if self.child_has_edges:
+                output.append(node_offset + "cursor")
+
+        output.append(edges_offset + "}")
+
+        # Add page information
+        output.append(edges_offset + "pageInfo {")
+        for page_key in (
+            "endCursor",
+            "hasNextPage",
+        ):
+            output.append(node_offset + page_key)
+        output.append(edges_offset + "}")
+        output.append(offset + "}")
+
+        return "\n".join(output)
+
+
+INTROSPECTION_QUERY = """
+  query IntrospectionQuery {
+    __schema {
+      queryType { name }
+      mutationType { name }
+      subscriptionType { name }
+      types {
+        ...FullType
+      }
+      directives {
+        name
+        description
+        locations
+        args {
+          ...InputValue
+        }
+      }
+    }
+  }
+  fragment FullType on __Type {
+    kind
+    name
+    description
+    fields(includeDeprecated: true) {
+      name
+      description
+      args {
+        ...InputValue
+      }
+      type {
+        ...TypeRef
+      }
+      isDeprecated
+      deprecationReason
+    }
+    inputFields {
+      ...InputValue
+    }
+    interfaces {
+      ...TypeRef
+    }
+    enumValues(includeDeprecated: true) {
+      name
+      description
+      isDeprecated
+      deprecationReason
+    }
+    possibleTypes {
+      ...TypeRef
+    }
+  }
+  fragment InputValue on __InputValue {
+    name
+    description
+    type { ...TypeRef }
+    defaultValue
+  }
+  fragment TypeRef on __Type {
+    kind
+    name
+    ofType {
+      kind
+      name
+      ofType {
+        kind
+        name
+        ofType {
+          kind
+          name
+          ofType {
+            kind
+            name
+            ofType {
+              kind
+              name
+              ofType {
+                kind
+                name
+                ofType {
+                  kind
+                  name
+                }
+              }
+            }
+          }
+        }
+      }
+    }
+  }
+"""
```

### Comparing `ayon-python-api-0.1.9/ayon_api/graphql_queries.py` & `ayon-python-api-0.2.0/ayon_api/graphql_queries.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,329 +1,464 @@
-import collections
-
-from .graphql import FIELD_VALUE, GraphQlQuery
-
-
-def fields_to_dict(fields):
-    if not fields:
-        return None
-
-    output = {}
-    for field in fields:
-        hierarchy = field.split(".")
-        last = hierarchy.pop(-1)
-        value = output
-        for part in hierarchy:
-            if value is FIELD_VALUE:
-                break
-
-            if part not in value:
-                value[part] = {}
-            value = value[part]
-
-        if value is not FIELD_VALUE:
-            value[last] = FIELD_VALUE
-    return output
-
-
-def project_graphql_query(fields):
-    query = GraphQlQuery("ProjectQuery")
-    project_name_var = query.add_variable("projectName", "String!")
-    project_field = query.add_field("project")
-    project_field.set_filter("name", project_name_var)
-
-    nested_fields = fields_to_dict(fields)
-
-    query_queue = collections.deque()
-    for key, value in nested_fields.items():
-        query_queue.append((key, value, project_field))
-
-    while query_queue:
-        item = query_queue.popleft()
-        key, value, parent = item
-        field = parent.add_field(key)
-        if value is FIELD_VALUE:
-            continue
-
-        for k, v in value.items():
-            query_queue.append((k, v, field))
-    return query
-
-
-def projects_graphql_query(fields):
-    query = GraphQlQuery("ProjectsQuery")
-    projects_field = query.add_field("projects", has_edges=True)
-
-    nested_fields = fields_to_dict(fields)
-
-    query_queue = collections.deque()
-    for key, value in nested_fields.items():
-        query_queue.append((key, value, projects_field))
-
-    while query_queue:
-        item = query_queue.popleft()
-        key, value, parent = item
-        field = parent.add_field(key)
-        if value is FIELD_VALUE:
-            continue
-
-        for k, v in value.items():
-            query_queue.append((k, v, field))
-    return query
-
-
-def folders_graphql_query(fields):
-    query = GraphQlQuery("FoldersQuery")
-    project_name_var = query.add_variable("projectName", "String!")
-    folder_ids_var = query.add_variable("folderIds", "[String!]")
-    parent_folder_ids_var = query.add_variable("parentFolderIds", "[String!]")
-    folder_paths_var = query.add_variable("folderPaths", "[String!]")
-    folder_names_var = query.add_variable("folderNames", "[String!]")
-    has_subsets_var = query.add_variable("folderHasSubsets", "Boolean!")
-
-    project_field = query.add_field("project")
-    project_field.set_filter("name", project_name_var)
-
-    folders_field = project_field.add_field("folders", has_edges=True)
-    folders_field.set_filter("ids", folder_ids_var)
-    folders_field.set_filter("parentIds", parent_folder_ids_var)
-    folders_field.set_filter("names", folder_names_var)
-    folders_field.set_filter("paths", folder_paths_var)
-    folders_field.set_filter("hasSubsets", has_subsets_var)
-
-    nested_fields = fields_to_dict(fields)
-
-    query_queue = collections.deque()
-    for key, value in nested_fields.items():
-        query_queue.append((key, value, folders_field))
-
-    while query_queue:
-        item = query_queue.popleft()
-        key, value, parent = item
-        field = parent.add_field(key)
-        if value is FIELD_VALUE:
-            continue
-
-        for k, v in value.items():
-            query_queue.append((k, v, field))
-    return query
-
-
-def tasks_graphql_query(fields):
-    query = GraphQlQuery("TasksQuery")
-    project_name_var = query.add_variable("projectName", "String!")
-    task_ids_var = query.add_variable("taskIds", "[String!]")
-    task_names_var = query.add_variable("taskNames", "[String!]")
-    task_types_var = query.add_variable("taskTypes", "[String!]")
-    folder_ids_var = query.add_variable("folderIds", "[String!]")
-
-    project_field = query.add_field("project")
-    project_field.set_filter("name", project_name_var)
-
-    tasks_field = project_field.add_field("tasks", has_edges=True)
-    tasks_field.set_filter("ids", task_ids_var)
-    # WARNING: At moment when this been created 'names' filter is not supported
-    tasks_field.set_filter("names", task_names_var)
-    tasks_field.set_filter("taskTypes", task_types_var)
-    tasks_field.set_filter("folderIds", folder_ids_var)
-
-    nested_fields = fields_to_dict(fields)
-
-    query_queue = collections.deque()
-    for key, value in nested_fields.items():
-        query_queue.append((key, value, tasks_field))
-
-    while query_queue:
-        item = query_queue.popleft()
-        key, value, parent = item
-        field = parent.add_field(key)
-        if value is FIELD_VALUE:
-            continue
-
-        for k, v in value.items():
-            query_queue.append((k, v, field))
-    return query
-
-
-def subsets_graphql_query(fields):
-    query = GraphQlQuery("SubsetsQuery")
-
-    project_name_var = query.add_variable("projectName", "String!")
-    folder_ids_var = query.add_variable("folderIds", "[String!]")
-    subset_ids_var = query.add_variable("subsetIds", "[String!]")
-    subset_names_var = query.add_variable("subsetNames", "[String!]")
-
-    project_field = query.add_field("project")
-    project_field.set_filter("name", project_name_var)
-
-    subsets_field = project_field.add_field("subsets", has_edges=True)
-    subsets_field.set_filter("ids", subset_ids_var)
-    subsets_field.set_filter("names", subset_names_var)
-    subsets_field.set_filter("folderIds", folder_ids_var)
-
-    nested_fields = fields_to_dict(set(fields))
-
-    query_queue = collections.deque()
-    for key, value in nested_fields.items():
-        query_queue.append((key, value, subsets_field))
-
-    while query_queue:
-        item = query_queue.popleft()
-        key, value, parent = item
-        field = parent.add_field(key)
-        if value is FIELD_VALUE:
-            continue
-
-        for k, v in value.items():
-            query_queue.append((k, v, field))
-    return query
-
-
-def versions_graphql_query(fields):
-    query = GraphQlQuery("VersionsQuery")
-
-    project_name_var = query.add_variable("projectName", "String!")
-    subset_ids_var = query.add_variable("subsetIds", "[String!]")
-    version_ids_var = query.add_variable("versionIds", "[String!]")
-    versions_var = query.add_variable("versions", "[Int!]")
-    hero_only_var = query.add_variable("heroOnly", "Boolean")
-    latest_only_var = query.add_variable("latestOnly", "Boolean")
-    hero_or_latest_only_var = query.add_variable(
-        "heroOrLatestOnly", "Boolean"
-    )
-
-    project_field = query.add_field("project")
-    project_field.set_filter("name", project_name_var)
-
-    subsets_field = project_field.add_field("versions", has_edges=True)
-    subsets_field.set_filter("ids", version_ids_var)
-    subsets_field.set_filter("subsetIds", subset_ids_var)
-    subsets_field.set_filter("versions", versions_var)
-    subsets_field.set_filter("heroOnly", hero_only_var)
-    subsets_field.set_filter("latestOnly", latest_only_var)
-    subsets_field.set_filter("heroOrLatestOnly", hero_or_latest_only_var)
-
-    nested_fields = fields_to_dict(set(fields))
-
-    query_queue = collections.deque()
-    for key, value in nested_fields.items():
-        query_queue.append((key, value, subsets_field))
-
-    while query_queue:
-        item = query_queue.popleft()
-        key, value, parent = item
-        field = parent.add_field(key)
-        if value is FIELD_VALUE:
-            continue
-
-        for k, v in value.items():
-            query_queue.append((k, v, field))
-    return query
-
-
-def representations_graphql_query(fields):
-    query = GraphQlQuery("RepresentationsQuery")
-
-    project_name_var = query.add_variable("projectName", "String!")
-    repre_ids_var = query.add_variable("representationIds", "[String!]")
-    repre_names_var = query.add_variable("representationNames", "[String!]")
-    version_ids_var = query.add_variable("versionIds", "[String!]")
-
-    project_field = query.add_field("project")
-    project_field.set_filter("name", project_name_var)
-
-    repres_field = project_field.add_field("representations", has_edges=True)
-    repres_field.set_filter("ids", repre_ids_var)
-    repres_field.set_filter("versionIds", version_ids_var)
-    repres_field.set_filter("names", repre_names_var)
-
-    nested_fields = fields_to_dict(set(fields))
-
-    query_queue = collections.deque()
-    for key, value in nested_fields.items():
-        query_queue.append((key, value, repres_field))
-
-    while query_queue:
-        item = query_queue.popleft()
-        key, value, parent = item
-        field = parent.add_field(key)
-        if value is FIELD_VALUE:
-            continue
-
-        for k, v in value.items():
-            query_queue.append((k, v, field))
-    return query
-
-
-def representations_parents_qraphql_query(
-    version_fields, subset_fields, folder_fields
-):
-
-    query = GraphQlQuery("RepresentationsParentsQuery")
-
-    project_name_var = query.add_variable("projectName", "String!")
-    repre_ids_var = query.add_variable("representationIds", "[String!]")
-
-    project_field = query.add_field("project")
-    project_field.set_filter("name", project_name_var)
-
-    repres_field = project_field.add_field("representations", has_edges=True)
-    repres_field.add_field("id")
-    repres_field.set_filter("ids", repre_ids_var)
-    version_field = repres_field.add_field("version")
-
-    fields_queue = collections.deque()
-    for key, value in fields_to_dict(version_fields).items():
-        fields_queue.append((key, value, version_field))
-
-    subset_field = version_field.add_field("subset")
-    for key, value in fields_to_dict(subset_fields).items():
-        fields_queue.append((key, value, subset_field))
-
-    folder_field = subset_field.add_field("folder")
-    for key, value in fields_to_dict(folder_fields).items():
-        fields_queue.append((key, value, folder_field))
-
-    while fields_queue:
-        item = fields_queue.popleft()
-        key, value, parent = item
-        field = parent.add_field(key)
-        if value is FIELD_VALUE:
-            continue
-
-        for k, v in value.items():
-            fields_queue.append((k, v, field))
-
-    return query
-
-
-def workfiles_info_graphql_query(fields):
-    query = GraphQlQuery("WorkfilesInfo")
-    project_name_var = query.add_variable("projectName", "String!")
-    workfiles_info_ids = query.add_variable("workfileIds", "[String!]")
-    task_ids_var = query.add_variable("taskIds", "[String!]")
-    paths_var = query.add_variable("paths", "[String!]")
-
-    project_field = query.add_field("project")
-    project_field.set_filter("name", project_name_var)
-
-    workfiles_field = project_field.add_field("workfiles", has_edges=True)
-    workfiles_field.set_filter("ids", workfiles_info_ids)
-    workfiles_field.set_filter("taskIds", task_ids_var)
-    workfiles_field.set_filter("paths", paths_var)
-
-    nested_fields = fields_to_dict(set(fields))
-
-    query_queue = collections.deque()
-    for key, value in nested_fields.items():
-        query_queue.append((key, value, workfiles_field))
-
-    while query_queue:
-        item = query_queue.popleft()
-        key, value, parent = item
-        field = parent.add_field(key)
-        if value is FIELD_VALUE:
-            continue
-
-        for k, v in value.items():
-            query_queue.append((k, v, field))
-    return query
+import collections
+
+from .graphql import FIELD_VALUE, GraphQlQuery
+
+
+def fields_to_dict(fields):
+    if not fields:
+        return None
+
+    output = {}
+    for field in fields:
+        hierarchy = field.split(".")
+        last = hierarchy.pop(-1)
+        value = output
+        for part in hierarchy:
+            if value is FIELD_VALUE:
+                break
+
+            if part not in value:
+                value[part] = {}
+            value = value[part]
+
+        if value is not FIELD_VALUE:
+            value[last] = FIELD_VALUE
+    return output
+
+
+def add_links_fields(entity_field, nested_fields):
+    if "links" not in nested_fields:
+        return
+    links_fields = nested_fields.pop("links")
+
+    link_edge_fields = {
+        "id",
+        "linkType",
+        "projectName",
+        "entityType",
+        "entityId",
+        "direction",
+        "description",
+        "author",
+    }
+    if isinstance(links_fields, dict):
+        simple_fields = set(links_fields)
+        simple_variant = len(simple_fields - link_edge_fields) == 0
+    else:
+        simple_variant = True
+        simple_fields = link_edge_fields
+
+    link_field = entity_field.add_field_with_edges("links")
+
+    link_type_var = link_field.add_variable("linkTypes", "[String!]")
+    link_dir_var = link_field.add_variable("linkDirection", "String!")
+    link_field.set_filter("linkTypes", link_type_var)
+    link_field.set_filter("direction", link_dir_var)
+
+    if simple_variant:
+        for key in simple_fields:
+            link_field.add_edge_field(key)
+        return
+
+    query_queue = collections.deque()
+    for key, value in links_fields.items():
+        if key in link_edge_fields:
+            link_field.add_edge_field(key)
+            continue
+        query_queue.append((key, value, link_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+
+
+def project_graphql_query(fields):
+    query = GraphQlQuery("ProjectQuery")
+    project_name_var = query.add_variable("projectName", "String!")
+    project_field = query.add_field("project")
+    project_field.set_filter("name", project_name_var)
+
+    nested_fields = fields_to_dict(fields)
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, project_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
+
+
+def projects_graphql_query(fields):
+    query = GraphQlQuery("ProjectsQuery")
+    projects_field = query.add_field_with_edges("projects")
+
+    nested_fields = fields_to_dict(fields)
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, projects_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
+
+
+def product_types_query(fields):
+    query = GraphQlQuery("ProductTypes")
+    product_types_field = query.add_field("productTypes")
+
+    nested_fields = fields_to_dict(fields)
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, product_types_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
+
+def project_product_types_query(fields):
+    query = GraphQlQuery("ProjectProductTypes")
+    project_query = query.add_field("project")
+    project_name_var = query.add_variable("projectName", "String!")
+    project_query.set_filter("name", project_name_var)
+    product_types_field = project_query.add_field("productTypes")
+    nested_fields = fields_to_dict(fields)
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, product_types_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
+
+
+def folders_graphql_query(fields):
+    query = GraphQlQuery("FoldersQuery")
+    project_name_var = query.add_variable("projectName", "String!")
+    folder_ids_var = query.add_variable("folderIds", "[String!]")
+    parent_folder_ids_var = query.add_variable("parentFolderIds", "[String!]")
+    folder_paths_var = query.add_variable("folderPaths", "[String!]")
+    folder_names_var = query.add_variable("folderNames", "[String!]")
+    has_products_var = query.add_variable("folderHasProducts", "Boolean!")
+
+    project_field = query.add_field("project")
+    project_field.set_filter("name", project_name_var)
+
+    folders_field = project_field.add_field_with_edges("folders")
+    folders_field.set_filter("ids", folder_ids_var)
+    folders_field.set_filter("parentIds", parent_folder_ids_var)
+    folders_field.set_filter("names", folder_names_var)
+    folders_field.set_filter("paths", folder_paths_var)
+    folders_field.set_filter("hasProducts", has_products_var)
+
+    nested_fields = fields_to_dict(fields)
+    add_links_fields(folders_field, nested_fields)
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, folders_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
+
+
+def tasks_graphql_query(fields):
+    query = GraphQlQuery("TasksQuery")
+    project_name_var = query.add_variable("projectName", "String!")
+    task_ids_var = query.add_variable("taskIds", "[String!]")
+    task_names_var = query.add_variable("taskNames", "[String!]")
+    task_types_var = query.add_variable("taskTypes", "[String!]")
+    folder_ids_var = query.add_variable("folderIds", "[String!]")
+
+    project_field = query.add_field("project")
+    project_field.set_filter("name", project_name_var)
+
+    tasks_field = project_field.add_field_with_edges("tasks")
+    tasks_field.set_filter("ids", task_ids_var)
+    # WARNING: At moment when this been created 'names' filter is not supported
+    tasks_field.set_filter("names", task_names_var)
+    tasks_field.set_filter("taskTypes", task_types_var)
+    tasks_field.set_filter("folderIds", folder_ids_var)
+
+    nested_fields = fields_to_dict(fields)
+    add_links_fields(tasks_field, nested_fields)
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, tasks_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
+
+
+def products_graphql_query(fields):
+    query = GraphQlQuery("ProductsQuery")
+
+    project_name_var = query.add_variable("projectName", "String!")
+    folder_ids_var = query.add_variable("folderIds", "[String!]")
+    product_ids_var = query.add_variable("productIds", "[String!]")
+    product_names_var = query.add_variable("productNames", "[String!]")
+
+    project_field = query.add_field("project")
+    project_field.set_filter("name", project_name_var)
+
+    products_field = project_field.add_field_with_edges("products")
+    products_field.set_filter("ids", product_ids_var)
+    products_field.set_filter("names", product_names_var)
+    products_field.set_filter("folderIds", folder_ids_var)
+
+    nested_fields = fields_to_dict(set(fields))
+    add_links_fields(products_field, nested_fields)
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, products_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
+
+
+def versions_graphql_query(fields):
+    query = GraphQlQuery("VersionsQuery")
+
+    project_name_var = query.add_variable("projectName", "String!")
+    product_ids_var = query.add_variable("productIds", "[String!]")
+    version_ids_var = query.add_variable("versionIds", "[String!]")
+    versions_var = query.add_variable("versions", "[Int!]")
+    hero_only_var = query.add_variable("heroOnly", "Boolean")
+    latest_only_var = query.add_variable("latestOnly", "Boolean")
+    hero_or_latest_only_var = query.add_variable(
+        "heroOrLatestOnly", "Boolean"
+    )
+
+    project_field = query.add_field("project")
+    project_field.set_filter("name", project_name_var)
+
+    products_field = project_field.add_field_with_edges("versions")
+    products_field.set_filter("ids", version_ids_var)
+    products_field.set_filter("productIds", product_ids_var)
+    products_field.set_filter("versions", versions_var)
+    products_field.set_filter("heroOnly", hero_only_var)
+    products_field.set_filter("latestOnly", latest_only_var)
+    products_field.set_filter("heroOrLatestOnly", hero_or_latest_only_var)
+
+    nested_fields = fields_to_dict(set(fields))
+    add_links_fields(products_field, nested_fields)
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, products_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
+
+
+def representations_graphql_query(fields):
+    query = GraphQlQuery("RepresentationsQuery")
+
+    project_name_var = query.add_variable("projectName", "String!")
+    repre_ids_var = query.add_variable("representationIds", "[String!]")
+    repre_names_var = query.add_variable("representationNames", "[String!]")
+    version_ids_var = query.add_variable("versionIds", "[String!]")
+
+    project_field = query.add_field("project")
+    project_field.set_filter("name", project_name_var)
+
+    repres_field = project_field.add_field_with_edges("representations")
+    repres_field.set_filter("ids", repre_ids_var)
+    repres_field.set_filter("versionIds", version_ids_var)
+    repres_field.set_filter("names", repre_names_var)
+
+    nested_fields = fields_to_dict(set(fields))
+    add_links_fields(repres_field, nested_fields)
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, repres_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
+
+
+def representations_parents_qraphql_query(
+    version_fields, product_fields, folder_fields
+):
+    query = GraphQlQuery("RepresentationsParentsQuery")
+
+    project_name_var = query.add_variable("projectName", "String!")
+    repre_ids_var = query.add_variable("representationIds", "[String!]")
+
+    project_field = query.add_field("project")
+    project_field.set_filter("name", project_name_var)
+
+    repres_field = project_field.add_field_with_edges("representations")
+    repres_field.add_field("id")
+    repres_field.set_filter("ids", repre_ids_var)
+    version_field = repres_field.add_field("version")
+
+    fields_queue = collections.deque()
+    for key, value in fields_to_dict(version_fields).items():
+        fields_queue.append((key, value, version_field))
+
+    product_field = version_field.add_field("product")
+    for key, value in fields_to_dict(product_fields).items():
+        fields_queue.append((key, value, product_field))
+
+    folder_field = product_field.add_field("folder")
+    for key, value in fields_to_dict(folder_fields).items():
+        fields_queue.append((key, value, folder_field))
+
+    while fields_queue:
+        item = fields_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            fields_queue.append((k, v, field))
+
+    return query
+
+
+def workfiles_info_graphql_query(fields):
+    query = GraphQlQuery("WorkfilesInfo")
+    project_name_var = query.add_variable("projectName", "String!")
+    workfiles_info_ids = query.add_variable("workfileIds", "[String!]")
+    task_ids_var = query.add_variable("taskIds", "[String!]")
+    paths_var = query.add_variable("paths", "[String!]")
+
+    project_field = query.add_field("project")
+    project_field.set_filter("name", project_name_var)
+
+    workfiles_field = project_field.add_field_with_edges("workfiles")
+    workfiles_field.set_filter("ids", workfiles_info_ids)
+    workfiles_field.set_filter("taskIds", task_ids_var)
+    workfiles_field.set_filter("paths", paths_var)
+
+    nested_fields = fields_to_dict(set(fields))
+    add_links_fields(workfiles_field, nested_fields)
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, workfiles_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
+
+
+def events_graphql_query(fields):
+    query = GraphQlQuery("Events")
+    topics_var = query.add_variable("eventTopics", "[String!]")
+    projects_var = query.add_variable("projectNames", "[String!]")
+    states_var = query.add_variable("eventStates", "[String!]")
+    users_var = query.add_variable("eventUsers", "[String!]")
+    include_logs_var = query.add_variable("includeLogsFilter", "Boolean!")
+
+    events_field = query.add_field_with_edges("events")
+    events_field.set_filter("topics", topics_var)
+    events_field.set_filter("projects", projects_var)
+    events_field.set_filter("states", states_var)
+    events_field.set_filter("users", users_var)
+    events_field.set_filter("includeLogs", include_logs_var)
+
+    nested_fields = fields_to_dict(set(fields))
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, events_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
```

### Comparing `ayon-python-api-0.1.9/ayon_api/operations.py` & `ayon-python-api-0.2.0/ayon_api/operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,821 +1,706 @@
-import copy
-import collections
-import uuid
-import datetime
-from abc import ABCMeta, abstractproperty
-
-import six
-
-from .server_api import get_server_api_connection
-from .utils import create_entity_id, REMOVED_VALUE
-
-
-def _create_or_convert_to_id(entity_id=None):
-    if entity_id is None:
-        return create_entity_id()
-
-    # Validate if can be converted to uuid
-    uuid.UUID(entity_id)
-    return entity_id
-
-
-def new_folder_entity(
-    name,
-    folder_type,
-    parent_id=None,
-    attribs=None,
-    data=None,
-    thumbnail_id=None,
-    entity_id=None
-):
-    """Create skeleton data of folder entity.
-
-    Args:
-        name (str): Is considered as unique identifier of folder in project.
-        parent_id (str): Id of parent folder.
-        attribs (Dict[str, Any]): Explicitly set attributes of folder.
-        data (Dict[str, Any]): Custom folder data. Empty dictionary is used
-            if not passed.
-        thumbnail_id (str): Id of thumbnail related to folder.
-        entity_id (str): Predefined id of entity. New id is
-            created if not passed.
-
-    Returns:
-        Dict[str, Any]: Skeleton of folder entity.
-    """
-
-    if attribs is None:
-        attribs = {}
-
-    if data is None:
-        data = {}
-
-    if parent_id is not None:
-        parent_id = _create_or_convert_to_id(parent_id)
-
-    return {
-        "id": _create_or_convert_to_id(entity_id),
-        "name": name,
-        # This will be ignored
-        "folderType": folder_type,
-        "parentId": parent_id,
-        "data": data,
-        "attrib": attribs,
-        "thumbnailId": thumbnail_id
-    }
-
-
-def new_subset_entity(
-    name, family, folder_id, attribs=None, data=None, entity_id=None
-):
-    """Create skeleton data of subset entity.
-
-    Args:
-        name (str): Is considered as unique identifier of subset under folder.
-        family (str): Subset's family.
-        folder_id (str): Id of parent folder.
-        attribs (Dict[str, Any]): Explicitly set attributes of subset.
-        data (Dict[str, Any]): Subset entity data. Empty dictionary is used
-            if not passed. Value of 'family' is used to fill 'family'.
-        entity_id (str): Predefined id of entity. New id is
-            created if not passed.
-
-    Returns:
-        Dict[str, Any]: Skeleton of subset entity.
-    """
-
-    if attribs is None:
-        attribs = {}
-
-    if data is None:
-        data = {}
-
-    return {
-        "id": _create_or_convert_to_id(entity_id),
-        "name": name,
-        "family": family,
-        "attrib": attribs,
-        "data": data,
-        "folderId": _create_or_convert_to_id(folder_id)
-    }
-
-
-def new_version_entity(
-    version,
-    subset_id,
-    task_id=None,
-    thumbnail_id=None,
-    author=None,
-    attribs=None,
-    data=None,
-    entity_id=None
-):
-    """Create skeleton data of version entity.
-
-    Args:
-        version (int): Is considered as unique identifier of version
-            under subset.
-        subset_id (str): Id of parent subset.
-        task_id (str): Id of task under which subset was created.
-        thumbnail_id (str): Thumbnail related to version.
-        author (str): Name of version author.
-        attribs (Dict[str, Any]): Explicitly set attributes of version.
-        data (Dict[str, Any]): Version entity custom data.
-        entity_id (str): Predefined id of entity. New id is
-            created if not passed.
-
-    Returns:
-        Dict[str, Any]: Skeleton of version entity.
-    """
-
-    if attribs is None:
-        attribs = {}
-
-    if data is None:
-        data = {}
-
-    if data is None:
-        data = {}
-
-    return {
-        "id": _create_or_convert_to_id(entity_id),
-        "version": int(version),
-        "subsetId": _create_or_convert_to_id(subset_id),
-        "attrib": attribs,
-        "data": data
-    }
-
-
-def new_hero_version_entity(
-    version,
-    subset_id,
-    task_id=None,
-    thumbnail_id=None,
-    author=None,
-    attribs=None,
-    data=None,
-    entity_id=None
-):
-    """Create skeleton data of hero version entity.
-
-    Args:
-        version (int): Is considered as unique identifier of version
-            under subset. Should be same as standard version if there is any.
-        subset_id (str): Id of parent subset.
-        task_id (str): Id of task under which subset was created.
-        thumbnail_id (str): Thumbnail related to version.
-        author (str): Name of version author.
-        attribs (Dict[str, Any]): Explicitly set attributes of version.
-        data (Dict[str, Any]): Version entity data.
-        entity_id (str): Predefined id of entity. New id is
-            created if not passed.
-
-    Returns:
-        Dict[str, Any]: Skeleton of version entity.
-    """
-
-    if attribs is None:
-        attribs = {}
-
-    if data is None:
-        data = {}
-
-    return {
-        "id": _create_or_convert_to_id(entity_id),
-        "version": -abs(int(version)),
-        "subsetId": subset_id,
-        "attrib": attribs,
-        "data": data
-    }
-
-
-def new_representation_entity(
-    name, version_id, attribs=None, data=None, entity_id=None
-):
-    """Create skeleton data of representation entity.
-
-    Args:
-        name (str): Representation name considered as unique identifier
-            of representation under version.
-        version_id (str): Id of parent version.
-        context (Dict[str, Any]): Representation context used to fill template.
-        attribs (Dict[str, Any]): Explicitly set attributes of representation.
-        data (Dict[str, Any]): Representation entity data.
-        entity_id (str): Predefined id of entity. New id is created
-            if not passed.
-
-    Returns:
-        Dict[str, Any]: Skeleton of representation entity.
-    """
-
-    if attribs is None:
-        attribs = {}
-
-    if data is None:
-        data = {}
-
-    return {
-        "id": _create_or_convert_to_id(entity_id),
-        "versionId": _create_or_convert_to_id(version_id),
-        "name": name,
-        "data": data,
-        "attrib": attribs
-    }
-
-
-def new_workfile_info_doc(
-    filename, folder_id, task_name, files, data=None, entity_id=None
-):
-    """Create skeleton data of workfile info entity.
-
-    Workfile entity is at this moment used primarily for artist notes.
-
-    Args:
-        filename (str): Filename of workfile.
-        folder_id (str): Id of folder under which workfile live.
-        task_name (str): Task under which was workfile created.
-        files (List[str]): List of rootless filepaths related to workfile.
-        data (Dict[str, Any]): Additional metadata.
-
-    Returns:
-        Dict[str, Any]: Skeleton of workfile info entity.
-    """
-
-    if not data:
-        data = {}
-
-    return {
-        "id": _create_or_convert_to_id(entity_id),
-        "parent": _create_or_convert_to_id(folder_id),
-        "task_name": task_name,
-        "filename": filename,
-        "data": data,
-        "files": files
-    }
-
-
-def _prepare_update_data(old_doc, new_doc, replace):
-    changes = {}
-    for key, value in new_doc.items():
-        if key not in old_doc or value != old_doc[key]:
-            changes[key] = value
-
-    if replace:
-        for key in old_doc.keys():
-            if key not in new_doc:
-                changes[key] = REMOVED_VALUE
-    return changes
-
-
-def prepare_folder_update_data(old_doc, new_doc, replace=True):
-    """Compare two folder entities and prepare update data.
-
-    Based on compared values will create update data for
-    'UpdateOperation'.
-
-    Empty output means that entities data are identical.
-
-    Returns:
-        Dict[str, Any]: Changes between old and new entity.
-    """
-
-    # changes = {}
-    # for key, value in new_doc.items():
-    #     if key in ("data", ):
-    #         continue
-    #
-    #     if key not in old_doc or value != old_doc[key]:
-    #         changes[key] = value
-    #
-    # return _prepare_update_data(old_doc, new_doc, replace)
-
-    raise NotImplementedError(
-        "'prepare_folder_update_data' not yet implemented"
-    )
-
-
-def prepare_subset_update_data(old_doc, new_doc, replace=True):
-    """Compare two subset entities and prepare update data.
-
-    Based on compared values will create update data for
-    'UpdateOperation'.
-
-    Empty output means that entities are identical.
-
-    Returns:
-        Dict[str, Any]: Changes between old and new entity.
-    """
-
-    # return _prepare_update_data(old_doc, new_doc, replace)
-
-    raise NotImplementedError(
-        "'prepare_folder_update_data' not yet implemented"
-    )
-
-
-def prepare_version_update_data(old_doc, new_doc, replace=True):
-    """Compare two version entities and prepare update data.
-
-    Based on compared values will create update data for
-    'UpdateOperation'.
-
-    Empty output means that entities are identical.
-
-    Returns:
-        Dict[str, Any]: Changes between old and new entity.
-    """
-
-    # return _prepare_update_data(old_doc, new_doc, replace)
-
-    raise NotImplementedError(
-        "'prepare_folder_update_data' not yet implemented"
-    )
-
-
-def prepare_hero_version_update_data(old_doc, new_doc, replace=True):
-    """Compare two hero version entities and prepare update data.
-
-    Based on compared values will create update data for 'UpdateOperation'.
-
-    Empty output means that entities are identical.
-
-    Returns:
-        Dict[str, Any]: Changes between old and new entity.
-    """
-
-    # return _prepare_update_data(old_doc, new_doc, replace)
-
-    raise NotImplementedError(
-        "'prepare_folder_update_data' not yet implemented"
-    )
-
-
-def prepare_representation_update_data(old_doc, new_doc, replace=True):
-    """Compare two representation entities and prepare update data.
-
-    Based on compared values will create update data for
-    'UpdateOperation'.
-
-    Empty output means that entities are identical.
-
-    Returns:
-        Dict[str, Any]: Changes between old and new entity.
-    """
-
-    # return _prepare_update_data(old_doc, new_doc, replace)
-
-    raise NotImplementedError(
-        "'prepare_folder_update_data' not yet implemented"
-    )
-
-
-def prepare_workfile_info_update_data(old_doc, new_doc, replace=True):
-    """Compare two workfile info entities and prepare update data.
-
-    Based on compared values will create update data for
-    'UpdateOperation'.
-
-    Empty output means that entities are identical.
-
-    Returns:
-        Dict[str, Any]: Changes between old and new entity.
-    """
-
-    # return _prepare_update_data(old_doc, new_doc, replace)
-
-    raise NotImplementedError(
-        "'prepare_folder_update_data' not yet implemented"
-    )
-
-
-def entity_data_json_default(value):
-    if isinstance(value, datetime.datetime):
-        return int(value.timestamp())
-
-    raise TypeError(
-        "Object of type {} is not JSON serializable".format(str(type(value)))
-    )
-
-
-def failed_json_default(value):
-    return "< Failed value {} > {}".format(type(value), str(value))
-
-
-@six.add_metaclass(ABCMeta)
-class AbstractOperation(object):
-    """Base operation class.
-
-    Opration represent a call into database. The call can create, change or
-    remove data.
-
-    Args:
-        project_name (str): On which project operation will happen.
-        entity_type (str): Type of entity on which change happens.
-            e.g. 'folder', 'representation' etc.
-    """
-
-    def __init__(self, project_name, entity_type, session):
-        self._project_name = project_name
-        self._entity_type = entity_type
-        self._session = session
-        self._id = str(uuid.uuid4())
-
-    @property
-    def project_name(self):
-        return self._project_name
-
-    @property
-    def id(self):
-        """Identifier of operation."""
-
-        return self._id
-
-    @property
-    def entity_type(self):
-        return self._entity_type
-
-    @abstractproperty
-    def operation_name(self):
-        """Stringified type of operation."""
-
-        pass
-
-    def to_data(self):
-        """Convert opration to data that can be converted to json or others.
-
-        Returns:
-            Dict[str, Any]: Description of operation.
-        """
-
-        return {
-            "id": self._id,
-            "entity_type": self.entity_type,
-            "project_name": self.project_name,
-            "operation": self.operation_name
-        }
-
-
-class CreateOperation(AbstractOperation):
-    """Opeartion to create an entity.
-
-    Args:
-        project_name (str): On which project operation will happen.
-        entity_type (str): Type of entity on which change happens.
-            e.g. 'folder', 'representation' etc.
-        data (Dict[str, Any]): Data of entity that will be created.
-    """
-
-    operation_name = "create"
-
-    def __init__(self, project_name, entity_type, data, session):
-        if not data:
-            data = {}
-        else:
-            data = copy.deepcopy(dict(data))
-
-        if "id" not in data:
-            data["id"] = create_entity_id()
-
-        self._data = data
-        super(CreateOperation, self).__init__(
-            project_name, entity_type, session
-        )
-
-    def __setitem__(self, key, value):
-        self.set_value(key, value)
-
-    def __getitem__(self, key):
-        return self.data[key]
-
-    def set_value(self, key, value):
-        self.data[key] = value
-
-    def get(self, key, *args, **kwargs):
-        return self.data.get(key, *args, **kwargs)
-
-    @property
-    def con(self):
-        return self.session.con
-
-    @property
-    def session(self):
-        return self._session
-
-    @property
-    def entity_id(self):
-        return self._data["id"]
-
-    @property
-    def data(self):
-        return self._data
-
-    def to_data(self):
-        output = super(CreateOperation, self).to_data()
-        output["data"] = copy.deepcopy(self.data)
-        return output
-
-    def to_server_operation(self):
-        return {
-            "id": self.id,
-            "type": "create",
-            "entityType": self.entity_type,
-            "entityId": self.entity_id,
-            "data": self._data
-        }
-
-
-class UpdateOperation(AbstractOperation):
-    """Operation to update an entity.
-
-    Args:
-        project_name (str): On which project operation will happen.
-        entity_type (str): Type of entity on which change happens.
-            e.g. 'folder', 'representation' etc.
-        entity_id (str): Identifier of an entity.
-        update_data (Dict[str, Any]): Key -> value changes that will be set in
-            database. If value is set to 'REMOVED_VALUE' the key will be
-            removed. Only first level of dictionary is checked (on purpose).
-    """
-
-    operation_name = "update"
-
-    def __init__(
-        self, project_name, entity_type, entity_id, update_data, session
-    ):
-        super(UpdateOperation, self).__init__(
-            project_name, entity_type, session
-        )
-
-        self._entity_id = entity_id
-        self._update_data = update_data
-
-    @property
-    def entity_id(self):
-        return self._entity_id
-
-    @property
-    def update_data(self):
-        return self._update_data
-
-    @property
-    def con(self):
-        return self.session.con
-
-    @property
-    def session(self):
-        return self._session
-
-    def to_data(self):
-        changes = {}
-        for key, value in self._update_data.items():
-            if value is REMOVED_VALUE:
-                value = None
-            changes[key] = value
-
-        output = super(UpdateOperation, self).to_data()
-        output.update({
-            "entity_id": self.entity_id,
-            "changes": changes
-        })
-        return output
-
-    def to_server_operation(self):
-        if not self._update_data:
-            return None
-
-        update_data = {}
-        for key, value in self._update_data.items():
-            if value is REMOVED_VALUE:
-                value = None
-            update_data[key] = value
-
-        return {
-            "id": self.id,
-            "type": "update",
-            "entityType": self.entity_type,
-            "entityId": self.entity_id,
-            "data": update_data
-        }
-
-
-class DeleteOperation(AbstractOperation):
-    """Opeartion to delete an entity.
-
-    Args:
-        project_name (str): On which project operation will happen.
-        entity_type (str): Type of entity on which change happens.
-            e.g. 'folder', 'representation' etc.
-        entity_id (str): Entity id that will be removed.
-    """
-
-    operation_name = "delete"
-
-    def __init__(self, project_name, entity_type, entity_id, session):
-        self._entity_id = entity_id
-
-        super(DeleteOperation, self).__init__(
-            project_name, entity_type, session
-        )
-
-    @property
-    def entity_id(self):
-        return self._entity_id
-
-    @property
-    def con(self):
-        return self.session.con
-
-    @property
-    def session(self):
-        return self._session
-
-    def to_data(self):
-        output = super(DeleteOperation, self).to_data()
-        output["entity_id"] = self.entity_id
-        return output
-
-    def to_server_operation(self):
-        return {
-            "id": self.id,
-            "type": self.operation_name,
-            "entityId": self.entity_id,
-            "entityType": self.entity_type,
-        }
-
-
-class OperationsSession(object):
-    """Session storing operations that should happen in an order.
-
-    At this moment does not handle anything special can be sonsidered as
-    stupid list of operations that will happen after each other. If creation
-    of same entity is there multiple times it's handled in any way and entity
-    values are not validated.
-
-    All operations must be related to single project.
-
-    Args:
-        project_name (str): Project name to which are operations related.
-    """
-
-    def __init__(self, con=None):
-        if con is None:
-            con = get_server_api_connection()
-        self._con = con
-        self._project_cache = {}
-        self._operations = []
-        self._nested_operations = collections.defaultdict(list)
-
-    @property
-    def con(self):
-        return self._con
-
-    def get_project(self, project_name):
-        if project_name not in self._project_cache:
-            self._project_cache[project_name] = self.con.get_project(
-                project_name)
-        return copy.deepcopy(self._project_cache[project_name])
-
-    def __len__(self):
-        return len(self._operations)
-
-    def add(self, operation):
-        """Add operation to be processed.
-
-        Args:
-            operation (BaseOperation): Operation that should be processed.
-        """
-        if not isinstance(
-            operation,
-            (CreateOperation, UpdateOperation, DeleteOperation)
-        ):
-            raise TypeError("Expected Operation object got {}".format(
-                str(type(operation))
-            ))
-
-        self._operations.append(operation)
-
-    def append(self, operation):
-        """Add operation to be processed.
-
-        Args:
-            operation (BaseOperation): Operation that should be processed.
-        """
-
-        self.add(operation)
-
-    def extend(self, operations):
-        """Add operations to be processed.
-
-        Args:
-            operations (List[BaseOperation]): Operations that should be
-                processed.
-        """
-
-        for operation in operations:
-            self.add(operation)
-
-    def remove(self, operation):
-        """Remove operation."""
-
-        self._operations.remove(operation)
-
-    def clear(self):
-        """Clear all registered operations."""
-
-        self._operations = []
-
-    def to_data(self):
-        return [
-            operation.to_data()
-            for operation in self._operations
-        ]
-
-    def commit(self):
-        """Commit session operations."""
-
-        operations, self._operations = self._operations, []
-        if not operations:
-            return
-
-        operations_by_project = collections.defaultdict(list)
-        for operation in operations:
-            operations_by_project[operation.project_name].append(operation)
-
-        for project_name, operations in operations_by_project.items():
-            operations_body = []
-            for operation in operations:
-                body = operation.to_server_operation()
-                if body is not None:
-                    operations_body.append(body)
-
-            self._con.send_batch_operations(
-                project_name, operations_body, can_fail=False
-            )
-
-    def create_entity(self, project_name, entity_type, data, nested_id=None):
-        """Fast access to 'CreateOperation'.
-
-        Args:
-            project_name (str): On which project the creation happens.
-            entity_type (str): Which entity type will be created.
-            data (Dicst[str, Any]): Entity data.
-            nested_id (str): Id of other operation from which is triggered
-                operation -> Operations can trigger suboperations but they
-                must be added to operations list after it's parent is added.
-
-        Returns:
-            CreateOperation: Object of update operation.
-        """
-
-        operation = CreateOperation(
-            project_name, entity_type, data, self
-        )
-
-        if nested_id:
-            self._nested_operations[nested_id].append(operation)
-        else:
-            self.add(operation)
-            if operation.id in self._nested_operations:
-                self.extend(self._nested_operations.pop(operation.id))
-
-        return operation
-
-    def update_entity(
-        self, project_name, entity_type, entity_id, update_data, nested_id=None
-    ):
-        """Fast access to 'UpdateOperation'.
-
-        Returns:
-            UpdateOperation: Object of update operation.
-        """
-
-        operation = UpdateOperation(
-            project_name, entity_type, entity_id, update_data, self
-        )
-        if nested_id:
-            self._nested_operations[nested_id].append(operation)
-        else:
-            self.add(operation)
-            if operation.id in self._nested_operations:
-                self.extend(self._nested_operations.pop(operation.id))
-        return operation
-
-    def delete_entity(
-        self, project_name, entity_type, entity_id, nested_id=None
-    ):
-        """Fast access to 'DeleteOperation'.
-
-        Returns:
-            DeleteOperation: Object of delete operation.
-        """
-
-        operation = DeleteOperation(
-            project_name, entity_type, entity_id, self
-        )
-        if nested_id:
-            self._nested_operations[nested_id].append(operation)
-        else:
-            self.add(operation)
-            if operation.id in self._nested_operations:
-                self.extend(self._nested_operations.pop(operation.id))
-        return operation
+import copy
+import collections
+import uuid
+from abc import ABCMeta, abstractmethod
+
+import six
+
+from ._api import get_server_api_connection
+from .utils import create_entity_id, REMOVED_VALUE
+
+
+def _create_or_convert_to_id(entity_id=None):
+    if entity_id is None:
+        return create_entity_id()
+
+    # Validate if can be converted to uuid
+    uuid.UUID(entity_id)
+    return entity_id
+
+
+def new_folder_entity(
+    name,
+    folder_type,
+    parent_id=None,
+    attribs=None,
+    data=None,
+    thumbnail_id=None,
+    entity_id=None
+):
+    """Create skeleton data of folder entity.
+
+    Args:
+        name (str): Is considered as unique identifier of folder in project.
+        folder_type (str): Type of folder.
+        parent_id (Optional[str]]): Id of parent folder.
+        attribs (Optional[Dict[str, Any]]): Explicitly set attributes
+            of folder.
+        data (Optional[Dict[str, Any]]): Custom folder data. Empty dictionary
+            is used if not passed.
+        thumbnail_id (Optional[str]): Id of thumbnail related to folder.
+        entity_id (Optional[str]): Predefined id of entity. New id is
+            created if not passed.
+
+    Returns:
+        Dict[str, Any]: Skeleton of folder entity.
+    """
+
+    if attribs is None:
+        attribs = {}
+
+    if data is None:
+        data = {}
+
+    if parent_id is not None:
+        parent_id = _create_or_convert_to_id(parent_id)
+
+    return {
+        "id": _create_or_convert_to_id(entity_id),
+        "name": name,
+        # This will be ignored
+        "folderType": folder_type,
+        "parentId": parent_id,
+        "data": data,
+        "attrib": attribs,
+        "thumbnailId": thumbnail_id
+    }
+
+
+def new_product_entity(
+    name,
+    product_type,
+    folder_id,
+    status=None,
+    attribs=None,
+    data=None,
+    entity_id=None
+):
+    """Create skeleton data of product entity.
+
+    Args:
+        name (str): Is considered as unique identifier of
+            product under folder.
+        product_type (str): Product type.
+        folder_id (str): Id of parent folder.
+        status (Optional[str]): Product status.
+        attribs (Optional[Dict[str, Any]]): Explicitly set attributes
+            of product.
+        data (Optional[Dict[str, Any]]): product entity data. Empty dictionary
+            is used if not passed.
+        entity_id (Optional[str]): Predefined id of entity. New id is
+            created if not passed.
+
+    Returns:
+        Dict[str, Any]: Skeleton of product entity.
+    """
+
+    if attribs is None:
+        attribs = {}
+
+    if data is None:
+        data = {}
+
+    output = {
+        "id": _create_or_convert_to_id(entity_id),
+        "name": name,
+        "productType": product_type,
+        "attrib": attribs,
+        "data": data,
+        "folderId": _create_or_convert_to_id(folder_id),
+    }
+    if status:
+        output["status"] = status
+    return output
+
+
+def new_version_entity(
+    version,
+    product_id,
+    task_id=None,
+    thumbnail_id=None,
+    author=None,
+    attribs=None,
+    data=None,
+    entity_id=None
+):
+    """Create skeleton data of version entity.
+
+    Args:
+        version (int): Is considered as unique identifier of version
+            under product.
+        product_id (str): Id of parent product.
+        task_id (Optional[str]]): Id of task under which product was created.
+        thumbnail_id (Optional[str]]): Thumbnail related to version.
+        author (Optional[str]]): Name of version author.
+        attribs (Optional[Dict[str, Any]]): Explicitly set attributes
+            of version.
+        data (Optional[Dict[str, Any]]): Version entity custom data.
+        entity_id (Optional[str]): Predefined id of entity. New id is
+            created if not passed.
+
+    Returns:
+        Dict[str, Any]: Skeleton of version entity.
+    """
+
+    if attribs is None:
+        attribs = {}
+
+    if data is None:
+        data = {}
+
+    if data is None:
+        data = {}
+
+    output = {
+        "id": _create_or_convert_to_id(entity_id),
+        "version": int(version),
+        "productId": _create_or_convert_to_id(product_id),
+        "attrib": attribs,
+        "data": data
+    }
+    if task_id:
+        output["taskId"] = task_id
+    if thumbnail_id:
+        output["thumbnailId"] = thumbnail_id
+    if author:
+        output["author"] = author
+    return output
+
+
+def new_hero_version_entity(
+    version,
+    product_id,
+    task_id=None,
+    thumbnail_id=None,
+    author=None,
+    attribs=None,
+    data=None,
+    entity_id=None
+):
+    """Create skeleton data of hero version entity.
+
+    Args:
+        version (int): Is considered as unique identifier of version
+            under product. Should be same as standard version if there is any.
+        product_id (str): Id of parent product.
+        task_id (Optional[str]): Id of task under which product was created.
+        thumbnail_id (Optional[str]): Thumbnail related to version.
+        author (Optional[str]): Name of version author.
+        attribs (Optional[Dict[str, Any]]): Explicitly set attributes
+            of version.
+        data (Optional[Dict[str, Any]]): Version entity data.
+        entity_id (Optional[str]): Predefined id of entity. New id is
+            created if not passed.
+
+    Returns:
+        Dict[str, Any]: Skeleton of version entity.
+    """
+
+    if attribs is None:
+        attribs = {}
+
+    if data is None:
+        data = {}
+
+    output = {
+        "id": _create_or_convert_to_id(entity_id),
+        "version": -abs(int(version)),
+        "productId": product_id,
+        "attrib": attribs,
+        "data": data
+    }
+    if task_id:
+        output["taskId"] = task_id
+    if thumbnail_id:
+        output["thumbnailId"] = thumbnail_id
+    if author:
+        output["author"] = author
+    return output
+
+
+def new_representation_entity(
+    name, version_id, attribs=None, data=None, entity_id=None
+):
+    """Create skeleton data of representation entity.
+
+    Args:
+        name (str): Representation name considered as unique identifier
+            of representation under version.
+        version_id (str): Id of parent version.
+        attribs (Optional[Dict[str, Any]]): Explicitly set attributes
+            of representation.
+        data (Optional[Dict[str, Any]]): Representation entity data.
+        entity_id (Optional[str]): Predefined id of entity. New id is created
+            if not passed.
+
+    Returns:
+        Dict[str, Any]: Skeleton of representation entity.
+    """
+
+    if attribs is None:
+        attribs = {}
+
+    if data is None:
+        data = {}
+
+    return {
+        "id": _create_or_convert_to_id(entity_id),
+        "versionId": _create_or_convert_to_id(version_id),
+        "name": name,
+        "data": data,
+        "attrib": attribs
+    }
+
+
+def new_workfile_info_doc(
+    filename, folder_id, task_name, files, data=None, entity_id=None
+):
+    """Create skeleton data of workfile info entity.
+
+    Workfile entity is at this moment used primarily for artist notes.
+
+    Args:
+        filename (str): Filename of workfile.
+        folder_id (str): Id of folder under which workfile live.
+        task_name (str): Task under which was workfile created.
+        files (List[str]): List of rootless filepaths related to workfile.
+        data (Optional[Dict[str, Any]]): Additional metadata.
+        entity_id (Optional[str]): Predefined id of entity. New id is created
+            if not passed.
+
+    Returns:
+        Dict[str, Any]: Skeleton of workfile info entity.
+    """
+
+    if not data:
+        data = {}
+
+    return {
+        "id": _create_or_convert_to_id(entity_id),
+        "parent": _create_or_convert_to_id(folder_id),
+        "task_name": task_name,
+        "filename": filename,
+        "data": data,
+        "files": files
+    }
+
+
+@six.add_metaclass(ABCMeta)
+class AbstractOperation(object):
+    """Base operation class.
+
+    Opration represent a call into database. The call can create, change or
+    remove data.
+
+    Args:
+        project_name (str): On which project operation will happen.
+        entity_type (str): Type of entity on which change happens.
+            e.g. 'folder', 'representation' etc.
+    """
+
+    def __init__(self, project_name, entity_type, session):
+        self._project_name = project_name
+        self._entity_type = entity_type
+        self._session = session
+        self._id = str(uuid.uuid4())
+
+    @property
+    def project_name(self):
+        return self._project_name
+
+    @property
+    def id(self):
+        """Identifier of operation."""
+
+        return self._id
+
+    @property
+    def entity_type(self):
+        return self._entity_type
+
+    @property
+    @abstractmethod
+    def operation_name(self):
+        """Stringified type of operation."""
+
+        pass
+
+    def to_data(self):
+        """Convert opration to data that can be converted to json or others.
+
+        Returns:
+            Dict[str, Any]: Description of operation.
+        """
+
+        return {
+            "id": self._id,
+            "entity_type": self.entity_type,
+            "project_name": self.project_name,
+            "operation": self.operation_name
+        }
+
+
+class CreateOperation(AbstractOperation):
+    """Opeartion to create an entity.
+
+    Args:
+        project_name (str): On which project operation will happen.
+        entity_type (str): Type of entity on which change happens.
+            e.g. 'folder', 'representation' etc.
+        data (Dict[str, Any]): Data of entity that will be created.
+    """
+
+    operation_name = "create"
+
+    def __init__(self, project_name, entity_type, data, session):
+        if not data:
+            data = {}
+        else:
+            data = copy.deepcopy(dict(data))
+
+        if "id" not in data:
+            data["id"] = create_entity_id()
+
+        self._data = data
+        super(CreateOperation, self).__init__(
+            project_name, entity_type, session
+        )
+
+    def __setitem__(self, key, value):
+        self.set_value(key, value)
+
+    def __getitem__(self, key):
+        return self.data[key]
+
+    def set_value(self, key, value):
+        self.data[key] = value
+
+    def get(self, key, *args, **kwargs):
+        return self.data.get(key, *args, **kwargs)
+
+    @property
+    def con(self):
+        return self.session.con
+
+    @property
+    def session(self):
+        return self._session
+
+    @property
+    def entity_id(self):
+        return self._data["id"]
+
+    @property
+    def data(self):
+        return self._data
+
+    def to_data(self):
+        output = super(CreateOperation, self).to_data()
+        output["data"] = copy.deepcopy(self.data)
+        return output
+
+    def to_server_operation(self):
+        return {
+            "id": self.id,
+            "type": "create",
+            "entityType": self.entity_type,
+            "entityId": self.entity_id,
+            "data": self._data
+        }
+
+
+class UpdateOperation(AbstractOperation):
+    """Operation to update an entity.
+
+    Args:
+        project_name (str): On which project operation will happen.
+        entity_type (str): Type of entity on which change happens.
+            e.g. 'folder', 'representation' etc.
+        entity_id (str): Identifier of an entity.
+        update_data (Dict[str, Any]): Key -> value changes that will be set in
+            database. If value is set to 'REMOVED_VALUE' the key will be
+            removed. Only first level of dictionary is checked (on purpose).
+    """
+
+    operation_name = "update"
+
+    def __init__(
+        self, project_name, entity_type, entity_id, update_data, session
+    ):
+        super(UpdateOperation, self).__init__(
+            project_name, entity_type, session
+        )
+
+        self._entity_id = entity_id
+        self._update_data = update_data
+
+    @property
+    def entity_id(self):
+        return self._entity_id
+
+    @property
+    def update_data(self):
+        return self._update_data
+
+    @property
+    def con(self):
+        return self.session.con
+
+    @property
+    def session(self):
+        return self._session
+
+    def to_data(self):
+        changes = {}
+        for key, value in self._update_data.items():
+            if value is REMOVED_VALUE:
+                value = None
+            changes[key] = value
+
+        output = super(UpdateOperation, self).to_data()
+        output.update({
+            "entity_id": self.entity_id,
+            "changes": changes
+        })
+        return output
+
+    def to_server_operation(self):
+        if not self._update_data:
+            return None
+
+        update_data = {}
+        for key, value in self._update_data.items():
+            if value is REMOVED_VALUE:
+                value = None
+            update_data[key] = value
+
+        return {
+            "id": self.id,
+            "type": "update",
+            "entityType": self.entity_type,
+            "entityId": self.entity_id,
+            "data": update_data
+        }
+
+
+class DeleteOperation(AbstractOperation):
+    """Opeartion to delete an entity.
+
+    Args:
+        project_name (str): On which project operation will happen.
+        entity_type (str): Type of entity on which change happens.
+            e.g. 'folder', 'representation' etc.
+        entity_id (str): Entity id that will be removed.
+    """
+
+    operation_name = "delete"
+
+    def __init__(self, project_name, entity_type, entity_id, session):
+        self._entity_id = entity_id
+
+        super(DeleteOperation, self).__init__(
+            project_name, entity_type, session
+        )
+
+    @property
+    def entity_id(self):
+        return self._entity_id
+
+    @property
+    def con(self):
+        return self.session.con
+
+    @property
+    def session(self):
+        return self._session
+
+    def to_data(self):
+        output = super(DeleteOperation, self).to_data()
+        output["entity_id"] = self.entity_id
+        return output
+
+    def to_server_operation(self):
+        return {
+            "id": self.id,
+            "type": self.operation_name,
+            "entityId": self.entity_id,
+            "entityType": self.entity_type,
+        }
+
+
+class OperationsSession(object):
+    """Session storing operations that should happen in an order.
+
+    At this moment does not handle anything special can be sonsidered as
+    stupid list of operations that will happen after each other. If creation
+    of same entity is there multiple times it's handled in any way and entity
+    values are not validated.
+
+    All operations must be related to single project.
+
+    Args:
+        project_name (str): Project name to which are operations related.
+    """
+
+    def __init__(self, con=None):
+        if con is None:
+            con = get_server_api_connection()
+        self._con = con
+        self._project_cache = {}
+        self._operations = []
+        self._nested_operations = collections.defaultdict(list)
+
+    @property
+    def con(self):
+        return self._con
+
+    def get_project(self, project_name):
+        if project_name not in self._project_cache:
+            self._project_cache[project_name] = self.con.get_project(
+                project_name)
+        return copy.deepcopy(self._project_cache[project_name])
+
+    def __len__(self):
+        return len(self._operations)
+
+    def add(self, operation):
+        """Add operation to be processed.
+
+        Args:
+            operation (BaseOperation): Operation that should be processed.
+        """
+        if not isinstance(
+            operation,
+            (CreateOperation, UpdateOperation, DeleteOperation)
+        ):
+            raise TypeError("Expected Operation object got {}".format(
+                str(type(operation))
+            ))
+
+        self._operations.append(operation)
+
+    def append(self, operation):
+        """Add operation to be processed.
+
+        Args:
+            operation (BaseOperation): Operation that should be processed.
+        """
+
+        self.add(operation)
+
+    def extend(self, operations):
+        """Add operations to be processed.
+
+        Args:
+            operations (List[BaseOperation]): Operations that should be
+                processed.
+        """
+
+        for operation in operations:
+            self.add(operation)
+
+    def remove(self, operation):
+        """Remove operation."""
+
+        self._operations.remove(operation)
+
+    def clear(self):
+        """Clear all registered operations."""
+
+        self._operations = []
+
+    def to_data(self):
+        return [
+            operation.to_data()
+            for operation in self._operations
+        ]
+
+    def commit(self):
+        """Commit session operations."""
+
+        operations, self._operations = self._operations, []
+        if not operations:
+            return
+
+        operations_by_project = collections.defaultdict(list)
+        for operation in operations:
+            operations_by_project[operation.project_name].append(operation)
+
+        for project_name, operations in operations_by_project.items():
+            operations_body = []
+            for operation in operations:
+                body = operation.to_server_operation()
+                if body is not None:
+                    operations_body.append(body)
+
+            self._con.send_batch_operations(
+                project_name, operations_body, can_fail=False
+            )
+
+    def create_entity(self, project_name, entity_type, data, nested_id=None):
+        """Fast access to 'CreateOperation'.
+
+        Args:
+            project_name (str): On which project the creation happens.
+            entity_type (str): Which entity type will be created.
+            data (Dicst[str, Any]): Entity data.
+            nested_id (str): Id of other operation from which is triggered
+                operation -> Operations can trigger suboperations but they
+                must be added to operations list after it's parent is added.
+
+        Returns:
+            CreateOperation: Object of update operation.
+        """
+
+        operation = CreateOperation(
+            project_name, entity_type, data, self
+        )
+
+        if nested_id:
+            self._nested_operations[nested_id].append(operation)
+        else:
+            self.add(operation)
+            if operation.id in self._nested_operations:
+                self.extend(self._nested_operations.pop(operation.id))
+
+        return operation
+
+    def update_entity(
+        self, project_name, entity_type, entity_id, update_data, nested_id=None
+    ):
+        """Fast access to 'UpdateOperation'.
+
+        Returns:
+            UpdateOperation: Object of update operation.
+        """
+
+        operation = UpdateOperation(
+            project_name, entity_type, entity_id, update_data, self
+        )
+        if nested_id:
+            self._nested_operations[nested_id].append(operation)
+        else:
+            self.add(operation)
+            if operation.id in self._nested_operations:
+                self.extend(self._nested_operations.pop(operation.id))
+        return operation
+
+    def delete_entity(
+        self, project_name, entity_type, entity_id, nested_id=None
+    ):
+        """Fast access to 'DeleteOperation'.
+
+        Returns:
+            DeleteOperation: Object of delete operation.
+        """
+
+        operation = DeleteOperation(
+            project_name, entity_type, entity_id, self
+        )
+        if nested_id:
+            self._nested_operations[nested_id].append(operation)
+        else:
+            self.add(operation)
+            if operation.id in self._nested_operations:
+                self.extend(self._nested_operations.pop(operation.id))
+        return operation
```

### Comparing `ayon-python-api-0.1.9/ayon_api/thumbnails.py` & `ayon-python-api-0.2.0/ayon_api/thumbnails.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-import os
-import time
-import collections
-
-import appdirs
-
-FileInfo = collections.namedtuple(
-    "FileInfo",
-    ("path", "size", "modification_time")
-)
-
-
-class ThumbnailCache:
-    """Cache of thumbnails on local storage.
-
-    Thumbnails are cached to appdirs to predefined directory. Each project has
-    own subfolder with thumbnails -> that's because each project has own
-    thumbnail id validation and file names are thumbnail ids with matching
-    extension. Extensions are predefined (.png and .jpeg).
-
-    Cache has cleanup mechanism which is triggered on initialized by default.
-
-    The cleanup has 2 levels:
-    1. soft cleanup which remove all files that are older then 'days_alive'
-    2. max size cleanup which remove all files until the thumbnails folder
-        contains less then 'max_filesize'
-        - this is time consuming so it's not triggered automatically
-
-    Args:
-        cleanup (bool): Trigger soft cleanup (Cleanup expired thumbnails).
-    """
-
-    # Lifetime of thumbnails (in seconds)
-    # - default 3 days
-    days_alive = 3 * 24 * 60 * 60
-    # Max size of thumbnail directory (in bytes)
-    # - default 2 Gb
-    max_filesize = 2 * 1024 * 1024 * 1024
-
-    def __init__(self, cleanup=True):
-        self._thumbnails_dir = None
-        if cleanup:
-            self.cleanup()
-
-    def get_thumbnails_dir(self):
-        """Root directory where thumbnails are stored.
-
-        Returns:
-            str: Path to thumbnails root.
-        """
-
-        if self._thumbnails_dir is None:
-            directory = appdirs.user_data_dir("ayon", "ynput")
-            self._thumbnails_dir = os.path.join(directory, "thumbnails")
-        return self._thumbnails_dir
-
-    thumbnails_dir = property(get_thumbnails_dir)
-
-    def get_thumbnails_dir_file_info(self):
-        """Get information about all files in thumbnails directory.
-
-        Returns:
-            List[FileInfo]: List of file information about all files.
-        """
-
-        thumbnails_dir = self.thumbnails_dir
-        files_info = []
-        if not os.path.exists(thumbnails_dir):
-            return files_info
-
-        for root, _, filenames in os.walk(thumbnails_dir):
-            for filename in filenames:
-                path = os.path.join(root, filename)
-                files_info.append(FileInfo(
-                    path, os.path.getsize(path), os.path.getmtime(path)
-                ))
-        return files_info
-
-    def get_thumbnails_dir_size(self, files_info=None):
-        """Got full size of thumbnail directory.
-
-        Args:
-            files_info (List[FileInfo]): Prepared file information about
-                files in thumbnail directory.
-
-        Returns:
-            int: File size of all files in thumbnail directory.
-        """
-
-        if files_info is None:
-            files_info = self.get_thumbnails_dir_file_info()
-
-        if not files_info:
-            return 0
-
-        return sum(
-            file_info.size
-            for file_info in files_info
-        )
-
-    def cleanup(self, check_max_size=False):
-        """Cleanup thumbnails directory.
-
-        Args:
-            check_max_size (bool): Also cleanup files to match max size of
-                thumbnails directory.
-        """
-
-        thumbnails_dir = self.get_thumbnails_dir()
-        # Skip if thumbnails dir does not exists yet
-        if not os.path.exists(thumbnails_dir):
-            return
-
-        self._soft_cleanup(thumbnails_dir)
-        if check_max_size:
-            self._max_size_cleanup(thumbnails_dir)
-
-    def _soft_cleanup(self, thumbnails_dir):
-        current_time = time.time()
-        for root, _, filenames in os.walk(thumbnails_dir):
-            for filename in filenames:
-                path = os.path.join(root, filename)
-                modification_time = os.path.getmtime(path)
-                if current_time - modification_time > self.days_alive:
-                    os.remove(path)
-
-    def _max_size_cleanup(self, thumbnails_dir):
-        files_info = self.get_thumbnails_dir_file_info()
-        size = self.get_thumbnails_dir_size(files_info)
-        if size < self.max_filesize:
-            return
-
-        sorted_file_info = collections.deque(
-            sorted(files_info, key=lambda item: item.modification_time)
-        )
-        diff = size - self.max_filesize
-        while diff > 0:
-            if not sorted_file_info:
-                break
-
-            file_info = sorted_file_info.popleft()
-            diff -= file_info.size
-            os.remove(file_info.path)
-
-    def get_thumbnail_filepath(self, project_name, thumbnail_id):
-        """Get thumbnail by thumbnail id.
-
-        Args:
-            project_name (str): Name of project.
-            thumbnail_id (str): Thumbnail id.
-
-        Returns:
-            Union[str, None]: Path to thumbnail image or None if thumbnail
-                is not cached yet.
-        """
-
-        if not thumbnail_id:
-            return None
-
-        for ext in (
-            ".png",
-            ".jpeg",
-        ):
-            filepath = os.path.join(
-                self.thumbnails_dir, project_name, thumbnail_id + ext
-            )
-            if os.path.exists(filepath):
-                return filepath
-        return None
-
-    def get_project_dir(self, project_name):
-        """Path to root directory for specific project.
-
-        Args:
-            project_name (str): Name of project for which root directory path
-                should be returned.
-
-        Returns:
-            str: Path to root of project's thumbnails.
-        """
-
-        return os.path.join(self.thumbnails_dir, project_name)
-
-    def make_sure_project_dir_exists(self, project_name):
-        project_dir = self.get_project_dir(project_name)
-        if not os.path.exists(project_dir):
-            os.makedirs(project_dir)
-        return project_dir
-
-    def store_thumbnail(self, project_name, thumbnail_id, content, mime_type):
-        """Store thumbnail to cache folder.
-
-        Args:
-            project_name (str): Project where the thumbnail belong to.
-            thumbnail_id (str): Id of thumbnail.
-            content (bytes): Byte content of thumbnail file.
-            mime_data (str): Type of content.
-
-        Returns:
-            str: Path to cached thumbnail image file.
-        """
-
-        if mime_type == "image/png":
-            ext = ".png"
-        elif mime_type == "image/jpeg":
-            ext = ".jpeg"
-        else:
-            raise ValueError(
-                "Unknown mime type for thumbnail \"{}\"".format(mime_type))
-
-        project_dir = self.make_sure_project_dir_exists(project_name)
-        thumbnail_path = os.path.join(project_dir, thumbnail_id + ext)
-        with open(thumbnail_path, "wb") as stream:
-            stream.write(content)
-
-        current_time = time.time()
-        os.utime(thumbnail_path, (current_time, current_time))
-
-        return thumbnail_path
+import os
+import time
+import collections
+
+import appdirs
+
+FileInfo = collections.namedtuple(
+    "FileInfo",
+    ("path", "size", "modification_time")
+)
+
+
+class ThumbnailCache:
+    """Cache of thumbnails on local storage.
+
+    Thumbnails are cached to appdirs to predefined directory. Each project has
+    own subfolder with thumbnails -> that's because each project has own
+    thumbnail id validation and file names are thumbnail ids with matching
+    extension. Extensions are predefined (.png and .jpeg).
+
+    Cache has cleanup mechanism which is triggered on initialized by default.
+
+    The cleanup has 2 levels:
+    1. soft cleanup which remove all files that are older then 'days_alive'
+    2. max size cleanup which remove all files until the thumbnails folder
+        contains less then 'max_filesize'
+        - this is time consuming so it's not triggered automatically
+
+    Args:
+        cleanup (bool): Trigger soft cleanup (Cleanup expired thumbnails).
+    """
+
+    # Lifetime of thumbnails (in seconds)
+    # - default 3 days
+    days_alive = 3 * 24 * 60 * 60
+    # Max size of thumbnail directory (in bytes)
+    # - default 2 Gb
+    max_filesize = 2 * 1024 * 1024 * 1024
+
+    def __init__(self, cleanup=True):
+        self._thumbnails_dir = None
+        if cleanup:
+            self.cleanup()
+
+    def get_thumbnails_dir(self):
+        """Root directory where thumbnails are stored.
+
+        Returns:
+            str: Path to thumbnails root.
+        """
+
+        if self._thumbnails_dir is None:
+            directory = appdirs.user_data_dir("ayon", "ynput")
+            self._thumbnails_dir = os.path.join(directory, "thumbnails")
+        return self._thumbnails_dir
+
+    thumbnails_dir = property(get_thumbnails_dir)
+
+    def get_thumbnails_dir_file_info(self):
+        """Get information about all files in thumbnails directory.
+
+        Returns:
+            List[FileInfo]: List of file information about all files.
+        """
+
+        thumbnails_dir = self.thumbnails_dir
+        files_info = []
+        if not os.path.exists(thumbnails_dir):
+            return files_info
+
+        for root, _, filenames in os.walk(thumbnails_dir):
+            for filename in filenames:
+                path = os.path.join(root, filename)
+                files_info.append(FileInfo(
+                    path, os.path.getsize(path), os.path.getmtime(path)
+                ))
+        return files_info
+
+    def get_thumbnails_dir_size(self, files_info=None):
+        """Got full size of thumbnail directory.
+
+        Args:
+            files_info (List[FileInfo]): Prepared file information about
+                files in thumbnail directory.
+
+        Returns:
+            int: File size of all files in thumbnail directory.
+        """
+
+        if files_info is None:
+            files_info = self.get_thumbnails_dir_file_info()
+
+        if not files_info:
+            return 0
+
+        return sum(
+            file_info.size
+            for file_info in files_info
+        )
+
+    def cleanup(self, check_max_size=False):
+        """Cleanup thumbnails directory.
+
+        Args:
+            check_max_size (bool): Also cleanup files to match max size of
+                thumbnails directory.
+        """
+
+        thumbnails_dir = self.get_thumbnails_dir()
+        # Skip if thumbnails dir does not exists yet
+        if not os.path.exists(thumbnails_dir):
+            return
+
+        self._soft_cleanup(thumbnails_dir)
+        if check_max_size:
+            self._max_size_cleanup(thumbnails_dir)
+
+    def _soft_cleanup(self, thumbnails_dir):
+        current_time = time.time()
+        for root, _, filenames in os.walk(thumbnails_dir):
+            for filename in filenames:
+                path = os.path.join(root, filename)
+                modification_time = os.path.getmtime(path)
+                if current_time - modification_time > self.days_alive:
+                    os.remove(path)
+
+    def _max_size_cleanup(self, thumbnails_dir):
+        files_info = self.get_thumbnails_dir_file_info()
+        size = self.get_thumbnails_dir_size(files_info)
+        if size < self.max_filesize:
+            return
+
+        sorted_file_info = collections.deque(
+            sorted(files_info, key=lambda item: item.modification_time)
+        )
+        diff = size - self.max_filesize
+        while diff > 0:
+            if not sorted_file_info:
+                break
+
+            file_info = sorted_file_info.popleft()
+            diff -= file_info.size
+            os.remove(file_info.path)
+
+    def get_thumbnail_filepath(self, project_name, thumbnail_id):
+        """Get thumbnail by thumbnail id.
+
+        Args:
+            project_name (str): Name of project.
+            thumbnail_id (str): Thumbnail id.
+
+        Returns:
+            Union[str, None]: Path to thumbnail image or None if thumbnail
+                is not cached yet.
+        """
+
+        if not thumbnail_id:
+            return None
+
+        for ext in (
+            ".png",
+            ".jpeg",
+        ):
+            filepath = os.path.join(
+                self.thumbnails_dir, project_name, thumbnail_id + ext
+            )
+            if os.path.exists(filepath):
+                return filepath
+        return None
+
+    def get_project_dir(self, project_name):
+        """Path to root directory for specific project.
+
+        Args:
+            project_name (str): Name of project for which root directory path
+                should be returned.
+
+        Returns:
+            str: Path to root of project's thumbnails.
+        """
+
+        return os.path.join(self.thumbnails_dir, project_name)
+
+    def make_sure_project_dir_exists(self, project_name):
+        project_dir = self.get_project_dir(project_name)
+        if not os.path.exists(project_dir):
+            os.makedirs(project_dir)
+        return project_dir
+
+    def store_thumbnail(self, project_name, thumbnail_id, content, mime_type):
+        """Store thumbnail to cache folder.
+
+        Args:
+            project_name (str): Project where the thumbnail belong to.
+            thumbnail_id (str): Id of thumbnail.
+            content (bytes): Byte content of thumbnail file.
+            mime_data (str): Type of content.
+
+        Returns:
+            str: Path to cached thumbnail image file.
+        """
+
+        if mime_type == "image/png":
+            ext = ".png"
+        elif mime_type == "image/jpeg":
+            ext = ".jpeg"
+        else:
+            raise ValueError(
+                "Unknown mime type for thumbnail \"{}\"".format(mime_type))
+
+        project_dir = self.make_sure_project_dir_exists(project_name)
+        thumbnail_path = os.path.join(project_dir, thumbnail_id + ext)
+        with open(thumbnail_path, "wb") as stream:
+            stream.write(content)
+
+        current_time = time.time()
+        os.utime(thumbnail_path, (current_time, current_time))
+
+        return thumbnail_path
```

### Comparing `ayon-python-api-0.1.9/ayon_python_api.egg-info/PKG-INFO` & `ayon-python-api-0.2.0/ayon_python_api.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,80 @@
-Metadata-Version: 2.1
-Name: ayon-python-api
-Version: 0.1.9
-Summary: AYON Python API
-Home-page: https://github.com/ynput/ayon-python-api
-Author: ynput.io
-Author-email: info@ynput.io
-License: Apache License (2.0)
-Description: # AYON server API
-        Python client for connection server. Client must be (at least for some time) Python 2 compatible because will be used in DCC that are "older".
-        
-        Client should support connection to server with raw REST functions and prepared functionality for work with entities. Must not contain only functionality that can be used with core server functionality.
-        
-        
-        ## TODOs
-        - Current implementation contains prepared functions for entity queries which is not using full potential of OpenPype server but is MongoDB compatible.
-            - only functions related to v4 should stay at that place and v3 compatible functions should be moved
-        - Missing settings getter
-        - Missing CRUD operations for entities (Only read is possible)
-        - More clear what is difference in `ServerAPIBase` and `ServerAPI`
-            - `ServerAPI` was added primarily for desktop app which handle login and logout in a different way so the class should be maybe removed and `ServerAPIBase` should be renamed to `ServerAPI`
-            - find more suitable names of classes
-            - find more suitable name of objects (right now is used `connection` or `conn`)
-        - Add folder and task changes to operations
-          - Entity hub should use operations to update folders and tasks 
-Keywords: AYON,ynput,OpenPype,vfx
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: ayon-python-api
+Version: 0.2.0
+Summary: AYON Python API
+Home-page: https://github.com/ynput/ayon-python-api
+Author: ynput.io
+Author-email: info@ynput.io
+License: Apache License (2.0)
+Keywords: AYON,ynput,OpenPype,vfx
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AYON server API
+Python client for connection server. Client must be (at least for some time) Python 2 compatible because will be used in DCC that are "older".
+
+AYON Python api should support connection to server with raw REST functions and prepared functionality for work with entities. Must not contain only functionality that can be used with core server functionality.
+
+Module support singleton connection which is using `AYON_SERVER_URL` and `AYON_API_KEY` environment variables as source for connection. The singleton connection is using `ServerAPI` object. There can be created multiple connection to different server at one time, for that purpose use `ServerAPIBase` object.
+
+## Install
+AYON python api is available on PyPi:
+
+    pip install ayon-python-api
+
+For development purposes you may follow [build](#build-wheel) guide to build and install custom wheels.
+
+
+## Cloning the repository
+Repository does not have submodules or special cases. Clone is simple as:
+
+    git clone git@github.com:ynput/ayon-python-api.git
+
+
+## Build wheel
+For wheel build is required a `wheel` module from PyPi:
+
+    pip install wheel
+
+Open terminal and change directory to ayon-python-api repository and build wheel:
+
+    cd <REPOSITORY ROOT>/ayon-python-api
+    python setup.py sdist bdist_wheel   
+    
+
+Once finished a wheel should be created in `./dist/ayon_python_api-<VERSION>-py3-none-any`.
+
+---
+
+### Wheel installation
+The wheel file can be used to install using pip:
+
+    pip install <REPOSITORY ROOT>/dist/ayon_python_api-<VERSION>-py3-none-any
+
+If pip complain that `ayon-python-api` is already installed just uninstall existing one first:
+    
+    pip uninstall ayon-python-api
+
+
+## TODOs
+- Find more suitable name of `ServerAPI` objects (right now is used `con` or `connection`)
+- Add all available CRUD operation on entities using REST
+- Add folder and task changes to operations
+- Enhance entity hub
+  - Missing docstrings in EntityHub -> especially entity arguments are missing
+  - Better order of arguments for entity classes
+    - Move entity hub to first place
+    - Skip those which are invalid for the entity and fake it for base or remove it from base
+  - Entity hub should use operations session to do changes
+  - Entity hub could also handle 'subset', 'version' and 'representation' entities
+  - Missing 'statuses' on project
+  - Missing 'status' on folders
+  - Missing assignees on tasks
+  - Pass docstrings and arguments definitions from `ServerAPI` methods to global functions
+- Split `ServerAPI` into smaller chunks (somehow), the class has 4k+ lines of code
+- Add .pyi stub for ServerAPI 
+- Missing websockets connection
```

### Comparing `ayon-python-api-0.1.9/ayon_python_api.egg-info/SOURCES.txt` & `ayon-python-api-0.2.0/ayon_python_api.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 ayon_api/__init__.py
+ayon_api/_api.py
 ayon_api/constants.py
 ayon_api/entity_hub.py
 ayon_api/events.py
 ayon_api/exceptions.py
 ayon_api/graphql.py
 ayon_api/graphql_queries.py
 ayon_api/operations.py
-ayon_api/server.py
 ayon_api/server_api.py
 ayon_api/thumbnails.py
 ayon_api/utils.py
 ayon_api/version.py
 ayon_python_api.egg-info/PKG-INFO
 ayon_python_api.egg-info/SOURCES.txt
 ayon_python_api.egg-info/dependency_links.txt
```

### Comparing `ayon-python-api-0.1.9/setup.py` & `ayon-python-api-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-import os
-from setuptools import setup
-
-REPO_ROOT = os.path.dirname(os.path.abspath(__file__))
-README_PATH = os.path.join(REPO_ROOT, "README.md")
-VERSION_PATH = os.path.join(REPO_ROOT, "ayon_api", "version.py")
-_version_content = {}
-exec(open(VERSION_PATH).read(), _version_content)
-
-setup(
-    name="ayon-python-api",
-    version=_version_content["__version__"],
-    py_modules=["ayon_api"],
-    packages=["ayon_api"],
-    author="ynput.io",
-    author_email="info@ynput.io",
-    license="Apache License (2.0)",
-    description="AYON Python API",
-    long_description=open(README_PATH).read(),
-    long_description_content_type="text/markdown",
-    url="https://github.com/ynput/ayon-python-api",
-    include_package_data=True,
-    # https://pypi.org/classifiers/
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 3",
-    ],
-    install_requires=[
-        "requests >= 2.27.1",
-        "six >= 1.15",
-        "Unidecode >= 1.3.6",
-        "appdirs >=1, <2",
-    ],
-    keywords=["AYON", "ynput", "OpenPype", "vfx"],
+# -*- coding: utf-8 -*-
+
+import os
+from setuptools import setup
+
+REPO_ROOT = os.path.dirname(os.path.abspath(__file__))
+README_PATH = os.path.join(REPO_ROOT, "README.md")
+VERSION_PATH = os.path.join(REPO_ROOT, "ayon_api", "version.py")
+_version_content = {}
+exec(open(VERSION_PATH).read(), _version_content)
+
+setup(
+    name="ayon-python-api",
+    version=_version_content["__version__"],
+    py_modules=["ayon_api"],
+    packages=["ayon_api"],
+    author="ynput.io",
+    author_email="info@ynput.io",
+    license="Apache License (2.0)",
+    description="AYON Python API",
+    long_description=open(README_PATH, encoding="utf-8").read(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/ynput/ayon-python-api",
+    include_package_data=True,
+    # https://pypi.org/classifiers/
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 2",
+        "Programming Language :: Python :: 3",
+    ],
+    install_requires=[
+        "requests >= 2.27.1",
+        "six >= 1.15",
+        "Unidecode >= 1.2.0",
+        "appdirs >=1, <2",
+    ],
+    keywords=["AYON", "ynput", "OpenPype", "vfx"],
 )
```

