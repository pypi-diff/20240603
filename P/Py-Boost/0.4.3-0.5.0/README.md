# Comparing `tmp/py_boost-0.4.3.tar.gz` & `tmp/py_boost-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_boost-0.4.3.tar", max compression
+gzip compressed data, was "py_boost-0.5.0.tar", max compression
```

## Comparing `py_boost-0.4.3.tar` & `py_boost-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0    11361 2023-05-27 15:22:20.177818 py_boost-0.4.3/LICENSE
--rw-r--r--   0        0        0     3636 2023-05-27 15:22:20.177818 py_boost-0.4.3/README.md
--rw-r--r--   0        0        0     1301 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/callbacks/__init__.py
--rw-r--r--   0        0        0     8542 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/callbacks/callback.py
--rw-r--r--   0        0        0      234 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/cv/__init__.py
--rw-r--r--   0        0        0     9356 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/cv/adaptive_es.py
--rw-r--r--   0        0        0     4199 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/cv/base.py
--rw-r--r--   0        0        0     7012 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/cv/cluster_tree.py
--rw-r--r--   0        0        0      120 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/gpu/__init__.py
--rw-r--r--   0        0        0    27174 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/gpu/base.py
--rw-r--r--   0        0        0    13160 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/gpu/boosting.py
--rw-r--r--   0        0        0      457 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/gpu/losses/__init__.py
--rw-r--r--   0        0        0     6266 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/gpu/losses/losses.py
--rw-r--r--   0        0        0     9368 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/gpu/losses/metrics.py
--rw-r--r--   0        0        0     3783 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/gpu/losses/multiclass_metrics.py
--rw-r--r--   0        0        0     4692 2023-05-27 15:23:53.285422 py_boost-0.4.3/py_boost/gpu/sketch_boost.py
--rw-r--r--   0        0        0    26445 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/gpu/tree.py
--rw-r--r--   0        0        0    28118 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/gpu/utils.py
--rw-r--r--   0        0        0       52 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/multioutput/__init__.py
--rw-r--r--   0        0        0     7955 2023-05-27 15:23:32.072603 py_boost-0.4.3/py_boost/multioutput/sketching.py
--rw-r--r--   0        0        0     2362 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/multioutput/target_splitter.py
--rw-r--r--   0        0        0       29 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/quantization/__init__.py
--rw-r--r--   0        0        0     3028 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/quantization/base.py
--rw-r--r--   0        0        0     4061 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/quantization/utils.py
--rw-r--r--   0        0        0       50 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/sampling/__init__.py
--rw-r--r--   0        0        0     6275 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/sampling/bagging.py
--rw-r--r--   0        0        0       35 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/utils/__init__.py
--rw-r--r--   0        0        0     5823 2023-05-27 15:22:20.177818 py_boost-0.4.3/py_boost/utils/logging.py
--rw-r--r--   0        0        0    10338 2023-05-27 15:22:20.181818 py_boost-0.4.3/py_boost/utils/tl_wrapper.py
--rw-r--r--   0        0        0     1247 2023-05-27 15:24:09.422043 py_boost-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     4983 1970-01-01 00:00:00.000000 py_boost-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11562 2024-05-27 15:11:09.000000 py_boost-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4192 2024-06-03 13:27:43.000000 py_boost-0.5.0/README.md
+-rw-r--r--   0        0        0     1530 2024-06-03 08:34:21.000000 py_boost-0.5.0/py_boost/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/callbacks/__init__.py
+-rw-r--r--   0        0        0     8832 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/callbacks/callback.py
+-rw-r--r--   0        0        0      247 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/cv/__init__.py
+-rw-r--r--   0        0        0     9687 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/cv/adaptive_es.py
+-rw-r--r--   0        0        0     4366 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/cv/base.py
+-rw-r--r--   0        0        0     7210 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/cv/cluster_tree.py
+-rw-r--r--   0        0        0      125 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/gpu/__init__.py
+-rw-r--r--   0        0        0    28339 2024-06-03 04:09:30.000000 py_boost-0.5.0/py_boost/gpu/base.py
+-rw-r--r--   0        0        0    13870 2024-06-03 04:18:21.000000 py_boost-0.5.0/py_boost/gpu/boosting.py
+-rw-r--r--   0        0        0      488 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/gpu/losses/__init__.py
+-rw-r--r--   0        0        0     6505 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/gpu/losses/losses.py
+-rw-r--r--   0        0        0     9709 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/gpu/losses/metrics.py
+-rw-r--r--   0        0        0     3921 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/gpu/losses/multiclass_metrics.py
+-rw-r--r--   0        0        0     3114 2024-06-03 03:59:05.000000 py_boost-0.5.0/py_boost/gpu/serialization.py
+-rw-r--r--   0        0        0     4812 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/gpu/sketch_boost.py
+-rw-r--r--   0        0        0    27026 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/gpu/tree.py
+-rw-r--r--   0        0        0    29801 2024-06-03 04:25:04.000000 py_boost-0.5.0/py_boost/gpu/utils.py
+-rw-r--r--   0        0        0       53 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/multioutput/__init__.py
+-rw-r--r--   0        0        0     8247 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/multioutput/sketching.py
+-rw-r--r--   0        0        0     2460 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/multioutput/target_splitter.py
+-rw-r--r--   0        0        0       30 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/quantization/__init__.py
+-rw-r--r--   0        0        0     3181 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/quantization/base.py
+-rw-r--r--   0        0        0     4358 2024-06-01 15:20:17.000000 py_boost-0.5.0/py_boost/quantization/utils.py
+-rw-r--r--   0        0        0       51 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/sampling/__init__.py
+-rw-r--r--   0        0        0     6502 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/sampling/bagging.py
+-rw-r--r--   0        0        0       36 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/utils/__init__.py
+-rw-r--r--   0        0        0     6004 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/utils/logging.py
+-rw-r--r--   0        0        0     7685 2024-06-03 12:24:15.000000 py_boost-0.5.0/py_boost/utils/onnx_wrapper.py
+-rw-r--r--   0        0        0    10338 2024-05-27 15:11:09.000000 py_boost-0.5.0/py_boost/utils/tl_wrapper.py
+-rw-r--r--   0        0        0     1338 2024-06-03 13:54:04.000000 py_boost-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5553 1970-01-01 00:00:00.000000 py_boost-0.5.0/PKG-INFO
```

### Comparing `py_boost-0.4.3/LICENSE` & `py_boost-0.5.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

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
-   Copyright 2021 Vakhrusev Anton, Iosipoi Leonid
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
+   Copyright 2021 Vakhrusev Anton, Iosipoi Leonid
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

### Comparing `py_boost-0.4.3/README.md` & `py_boost-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,70 @@
-# Py-boost: a research tool for exploring GBDTs
-
-Modern gradient boosting toolkits are very complex and are written in low-level programming languages. As a result,
-
-* It is hard to customize them to suit one’s needs 
-* New ideas and methods are not easy to implement
-* It is difficult to understand how they work
-
-Py-boost is a Python-based gradient boosting library which aims at overcoming the aforementioned problems. 
-
-**Authors**: [Anton Vakhrushev](https://kaggle.com/btbpanda), [Leonid Iosipoi](http://iosipoi.com/), [Sergey Kupriyanov](https://www.linkedin.com/in/sergeykupriyanov).
-
-
-## Py-boost Key Features
-
-**Simple**. Py-boost is a simplified gradient boosting library, but it supports all main features and hyperparameters available in other implementations.
-
-**Fast with GPU**. Despite the fact that Py-boost is written in Python, it works only on GPU and uses Python GPU libraries such as `CuPy` and `Numba`.
-
-**Efficient inference**. Since v0.4 Py-Boost is able to perform the efficient inference of tree ensembles on GPU. Moreover, ones your model is trained on GPU, it could be converted to perform the inference on CPU only machine via converting to the [treelite](https://treelite.readthedocs.io/) format with build-in wrapper (limitation - model should be trained with `target_splitter='Single'`, which is the default). 
-
-**Easy to customize**. Py-boost can be easily customized even if one is not familiar with GPU programming (just replace np with cp).  What can be customized? Almost everything via custom callbacks. Examples: Row/Col sampling strategy, Training control, Losses/metrics, Multioutput handling strategy, Anything via custom callbacks
-
-
-## SketchBoost [paper](https://openreview.net/forum?id=WSxarC8t-T)
-
-**Multioutput training**. Current state-of-atr boosting toolkits provide very limited support of multioutput training. And even if this option is available, training time for such tasks as multiclass/multilabel classification and multitask regression is quite slow because of the training complexity that scales linearly with the number of outputs. To overcome the existing limitations we create **SketchBoost** algorithm that uses approximate tree structure search. As we show in [paper](https://openreview.net/forum?id=WSxarC8t-T) that strategy at least does not lead to performance decrease and often is able to improve the accuracy
-
-**SketchBoost**. You can try our sketching strategies by using `SketchBoost` class or if you want you can implement your own and pass to the `GradientBoosting` constructor as `multioutput_sketch` parameter. For the details please see [Tutorial_2_Advanced_multioutput](https://github.com/AILab-MLTools/Py-Boost/blob/master/tutorials/Tutorial_2_Advanced_multioutput.ipynb)
-
-
-## Installation
-
-Before installing py-boost via pip you should have cupy installed. You can use:
-
-`pip install -U cupy-cuda110 py-boost`
-
-**Note**: replace with your cuda version! For the details see [this guide](https://docs.cupy.dev/en/stable/install.html)
-
-
-## Quick tour
-
-Py-boost is easy to use since it has similar to scikit-learn interface. For usage example please see:
-
-* [Tutorial_1_Basics](https://github.com/AILab-MLTools/Py-Boost/blob/master/tutorials/Tutorial_1_Basics.ipynb) for simple usage examples
-* [Tutorial_2_Advanced_multioutput](https://github.com/AILab-MLTools/Py-Boost/blob/master/tutorials/Tutorial_2_Advanced_multioutput.ipynb) for advanced multioutput features
-* [Tutorial_3_Custom_features](https://github.com/AILab-MLTools/Py-Boost/blob/master/tutorials/Tutorial_3_Custom_features.ipynb) for examples of customization
-
-More examples are coming soon
+# Py-boost: a research tool for exploring GBDTs
+
+Modern gradient boosting toolkits are very complex and are written in low-level programming languages. As a result,
+
+* It is hard to customize them to suit one’s needs
+* New ideas and methods are not easy to implement
+* It is difficult to understand how they work
+
+Py-boost is a Python-based gradient boosting library which aims at overcoming the aforementioned problems.
+
+**Authors**: [Anton Vakhrushev](https://kaggle.com/btbpanda), [Leonid Iosipoi](http://iosipoi.com/)
+, [Sergey Kupriyanov](https://www.linkedin.com/in/sergeykupriyanov).
+
+## Py-boost Key Features
+
+**Simple**. Py-boost is a simplified gradient boosting library, but it supports all main features and hyperparameters
+available in other implementations.
+
+**Fast with GPU**. Despite the fact that Py-boost is written in Python, it works only on GPU and uses Python GPU
+libraries such as `CuPy` and `Numba`.
+
+**Efficient inference**. Since v0.4 Py-Boost is able to perform the efficient inference of tree ensembles on GPU.
+Moreover, ones your model is trained on GPU, it could be converted to perform the inference on CPU only machine via
+converting to the [treelite](https://treelite.readthedocs.io/) format with build-in wrapper (limitation - model should
+be trained with `target_splitter='Single'`, which is the default).
+
+**ONNX compatible** Since v0.5 Py-Boost is compatible with ONNX format that allows more options the CPU inference and
+model deployment.
+
+**Easy to customize**. Py-boost can be easily customized even if one is not familiar with GPU programming (just replace
+np with cp). What can be customized? Almost everything via custom callbacks. Examples: Row/Col sampling strategy,
+Training control, Losses/metrics, Multioutput handling strategy, Anything via custom callbacks
+
+## SketchBoost [paper](https://openreview.net/forum?id=WSxarC8t-T)
+
+**Multioutput training**. Current state-of-atr boosting toolkits provide very limited support of multioutput training.
+And even if this option is available, training time for such tasks as multiclass/multilabel classification and multitask
+regression is quite slow because of the training complexity that scales linearly with the number of outputs. To overcome
+the existing limitations we create **SketchBoost** algorithm that uses approximate tree structure search. As we show
+in [paper](https://openreview.net/forum?id=WSxarC8t-T) that strategy at least does not lead to performance decrease and
+often is able to improve the accuracy
+
+**SketchBoost**. You can try our sketching strategies by using `SketchBoost` class or if you want you can implement your
+own and pass to the `GradientBoosting` constructor as `multioutput_sketch` parameter. For the details please
+see [Tutorial_2_Advanced_multioutput](https://github.com/AILab-MLTools/Py-Boost/blob/master/tutorials/Tutorial_2_Advanced_multioutput.ipynb)
+
+## Installation
+
+Before installing py-boost via pip you should have cupy installed. You can use:
+
+`pip install -U cupy-cuda110 py-boost`
+
+**Note**: replace with your cuda version! For the details see [this guide](https://docs.cupy.dev/en/stable/install.html)
+
+## Quick tour
+
+Py-boost is easy to use since it has similar to scikit-learn interface. For usage example please see:
+
+* [Tutorial_1_Basics](https://github.com/sb-ai-lab/Py-Boost/blob/master/tutorials/Tutorial_1_Basics.ipynb) for simple
+  usage examples
+* [Tutorial_2_Advanced_multioutput](https://github.com/sb-ai-lab/Py-Boost/blob/master/tutorials/Tutorial_2_Advanced_multioutput.ipynb)
+  for advanced multioutput features
+* [Tutorial_3_Custom_features](https://github.com/sb-ai-lab/Py-Boost/blob/master/tutorials/Tutorial_3_Custom_features.ipynb)
+  for examples of customization
+* [Tutorial_4_Handle_null_targets](https://github.com/sb-ai-lab/Py-Boost/blob/master/tutorials/Tutorial_4_Handle_null_targets.ipynb)
+  for the case when multioutput target contains NaNs
+* [Tutorial_5_ONNX_inference](https://github.com/sb-ai-lab/Py-Boost/blob/master/tutorials/Tutorial_5_ONNX_inference.ipynb)
+  examples of parsing and inference on CPU with ONNX
+
+More examples are coming soon
```

### Comparing `py_boost-0.4.3/py_boost/callbacks/callback.py` & `py_boost-0.5.0/py_boost/callbacks/callback.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,290 +1,290 @@
-"""Default callbacks"""
-import logging
-from ..utils.logging import verbosity_to_loglevel, set_stdout_level
-
-logger = logging.getLogger(__name__)
-
-
-class Callback:
-    """Abstract class for callback. All Callback methods define the actions, should be done between training stages
-    There are 4 methods, that could be redefined:
-        - before_train - outputs None
-        - before_iteration - outputs None
-        - after_train - outputs None
-        - after_iteration - outputs bool - if training should be stopped after iteration
-
-    Methods received build_info - the state dict, that could be accessed and modifier
-
-    Basic build info structure:
-
-    build_info = {
-            'data': {
-                'train': {
-                    'features_cpu': np.ndarray - raw feature matrix,
-                    'features_gpu': cp.ndarray - uint8 quantized feature matrix on GPU,
-                    'target': y - cp.ndarray - processed target variable on GPU,
-                    'sample_weight': cp.ndarray - processed sample_weight on GPU or None,
-                    'ensemble': cp.ndarray - current model prediction (with no postprocessing,
-                        ex. before sigmoid for logloss) on GPU,
-                    'grad': cp.ndarray of gradients on GPU, before first iteration - None,
-                    'hess': cp.ndarray of hessians on GPU, before first iteration - None,
-
-                    'last_tree': {
-                        'nodes': cp.ndarray - nodes indices of the last trained tree,
-                        'preds': cp.ndarray - predictions of the last trained tree,
-                    }
-
-                },
-                'valid': {
-                    'features_cpu' the same as train, but list, each element corresponds each validation sample,
-                    'features_gpu': ...,
-                    'target': ...,
-                    'sample_weight': ...,
-                    'ensemble': ...,
-
-                    'last_tree': {
-                        'nodes': ...,
-                        'preds': ...,
-                    }
-
-                }
-            },
-            'borders': list of np.ndarray - list or quantization borders,
-            'model': GradientBoosting - model, that is trained,
-            'mempool': cp.cuda.MemoryPool - memory pool used for train, could be used to clean memory to prevent OOM,
-            'builder': DepthwiseTreeBuilder - the instance of tree builder, contains training params,
-
-            'num_iter': int, current number of iteration,
-            'iter_scores': list of float - list of metric values for all validation sets for the last iteration,
-        }
-
-    """
-
-    def before_train(self, build_info):
-        """Actions to be made before train starts
-
-        Args:
-            build_info: dict
-
-        Returns:
-
-        """
-        return
-
-    def before_iteration(self, build_info):
-        """Actions to be made before each iteration starts
-
-        Args:
-            build_info: dict
-
-        Returns:
-
-        """
-        return
-
-    def after_iteration(self, build_info):
-        """Actions to be made after each iteration finishes
-
-        Args:
-            build_info: dict
-
-        Returns:
-            bool, if train process should be terminated
-        """
-        return False
-
-    def after_train(self, build_info):
-        """Actions to be made before train finishes
-
-        Args:
-            build_info:
-
-        Returns:
-
-        """
-        return
-
-
-class CallbackPipeline:
-    """Sequential pipeline of callbacks"""
-
-    def __init__(self, *callbacks):
-        self.callbacks = callbacks
-
-    def after_iteration(self, build_info):
-        stop = False
-
-        for callback in self.callbacks:
-            stop = stop or callback.after_iteration(build_info)
-
-        return stop
-
-    def after_train(self, build_info):
-
-        for callback in self.callbacks:
-            callback.after_train(build_info)
-
-    def before_train(self, build_info):
-
-        for callback in self.callbacks:
-            callback.before_train(build_info)
-
-    def before_iteration(self, build_info):
-
-        for callback in self.callbacks:
-            callback.before_iteration(build_info)
-
-
-class EvalHistory(Callback):
-    """Callback for history evaluation"""
-
-    def __init__(self, history, verbose=0):
-
-        self.history = history
-        self.verbose = verbose
-        self.metric = None
-        self.postprocess_fn = None
-        self.ntrees = None
-
-    def before_train(self, build_info):
-        """Init params and logger
-
-        Args:
-            build_info: dict
-
-        Returns:
-
-        """
-        self.metric = build_info['model'].metric
-        self.postprocess_fn = build_info['model'].loss.postprocess_output
-        self.ntrees = build_info['model'].ntrees
-
-        self.set_verbosity_level(int(self.verbose > 0) * 1)
-
-        msg = 'GDBT train starts. Max iter {0}, early stopping rounds {1}'.format(
-            build_info['model'].ntrees, build_info['model'].es)
-
-        logger.info(msg)
-
-    def after_iteration(self, build_info):
-        """Save the iteration results and output log
-
-        Args:
-            build_info: dict
-
-        Returns:
-
-        """
-        valid = build_info['data']['valid']
-        y_val, val_ens, w_val = valid['target'], valid['ensemble'], valid['sample_weight']
-
-        num_iter = build_info['num_iter']
-
-        msg = 'Iter {0}; '.format(num_iter)
-
-        if self.metric is None:
-            return
-
-        alias = self.metric.alias
-
-        if len(y_val) > 0:
-            val_metric = [float(self.metric(y, self.postprocess_fn(x), w)) for (y, x, w) in zip(y_val, val_ens, w_val)]
-            self.history.append(val_metric)
-
-            msg += ' '.join(['Sample {0}, {1} = {2}; '.format(n, alias, x) for (n, x) in enumerate(val_metric)])
-
-            build_info['iter_score'] = val_metric
-
-        if ((num_iter % self.verbose) == 0) or (num_iter == (self.ntrees - 1)):
-            logger.info(msg)
-
-    @staticmethod
-    def set_verbosity_level(verbose):
-        """Verbosity level setter.
-
-        Args:
-            verbose: Controls the verbosity: the higher, the more messages.
-                <1  : messages are not displayed;
-                >=1 : the computation process for layers is displayed;
-                >=2 : the information about folds processing is also displayed;
-                >=3 : the hyperparameters optimization process is also displayed;
-                >=4 : the training process for every algorithm is displayed;
-        """
-        level = verbosity_to_loglevel(verbose)
-        set_stdout_level(level)
-
-        logger.info(f"Stdout logging level is {logging._levelToName[level]}.")
-
-
-class EarlyStopping(Callback):
-    """Callback for early stopping"""
-
-    def __init__(self, num_rounds=100):
-
-        self.num_rounds = num_rounds
-        self.best_round = 1
-        self.no_upd_rounds = 0
-        self.best_score = None
-        self.metric = None
-
-    def before_train(self, build_info):
-        """Init params
-
-        Args:
-            build_info: dict
-
-        Returns:
-
-        """
-        self.metric = build_info['model'].metric
-
-    def after_iteration(self, build_info):
-        """Check early stopping condition and update the state
-
-        Args:
-            build_info: dict
-
-        Returns:
-            bool, if early stopping condition was met
-        """
-        if ('iter_score' not in build_info) or (self.num_rounds == 0):
-            return False
-
-        num_iter = build_info['num_iter']
-        # if multiple valid sets passed - use the last one
-        score = build_info['iter_score'][-1]
-
-        if num_iter == 0:
-            self.best_score = score
-            return False
-
-        if self.metric.compare(score, self.best_score):
-            self.best_score = score
-            self.best_round = num_iter + 1
-            self.no_upd_rounds = 0
-            return False
-
-        self.no_upd_rounds += 1
-
-        stop = self.no_upd_rounds >= self.num_rounds
-
-        if stop:
-            msg = 'Early stopping at iter {0}, best iter {1}, best_score {2}'.format(
-                num_iter + 1, self.best_round, self.best_score)
-            logger.info(msg)
-
-        return stop
-
-    def after_train(self, build_info):
-        """Prune the model to the best iteration
-
-        Args:
-            build_info: dict
-
-        Returns:
-
-        """
-        if self.best_score is not None:
-            model = build_info['model']
-            model.models = model.models[:self.best_round]
-            model.best_round = self.best_round
+"""Default callbacks"""
+import logging
+from ..utils.logging import verbosity_to_loglevel, set_stdout_level
+
+logger = logging.getLogger(__name__)
+
+
+class Callback:
+    """Abstract class for callback. All Callback methods define the actions, should be done between training stages
+    There are 4 methods, that could be redefined:
+        - before_train - outputs None
+        - before_iteration - outputs None
+        - after_train - outputs None
+        - after_iteration - outputs bool - if training should be stopped after iteration
+
+    Methods received build_info - the state dict, that could be accessed and modifier
+
+    Basic build info structure:
+
+    build_info = {
+            'data': {
+                'train': {
+                    'features_cpu': np.ndarray - raw feature matrix,
+                    'features_gpu': cp.ndarray - uint8 quantized feature matrix on GPU,
+                    'target': y - cp.ndarray - processed target variable on GPU,
+                    'sample_weight': cp.ndarray - processed sample_weight on GPU or None,
+                    'ensemble': cp.ndarray - current model prediction (with no postprocessing,
+                        ex. before sigmoid for logloss) on GPU,
+                    'grad': cp.ndarray of gradients on GPU, before first iteration - None,
+                    'hess': cp.ndarray of hessians on GPU, before first iteration - None,
+
+                    'last_tree': {
+                        'nodes': cp.ndarray - nodes indices of the last trained tree,
+                        'preds': cp.ndarray - predictions of the last trained tree,
+                    }
+
+                },
+                'valid': {
+                    'features_cpu' the same as train, but list, each element corresponds each validation sample,
+                    'features_gpu': ...,
+                    'target': ...,
+                    'sample_weight': ...,
+                    'ensemble': ...,
+
+                    'last_tree': {
+                        'nodes': ...,
+                        'preds': ...,
+                    }
+
+                }
+            },
+            'borders': list of np.ndarray - list or quantization borders,
+            'model': GradientBoosting - model, that is trained,
+            'mempool': cp.cuda.MemoryPool - memory pool used for train, could be used to clean memory to prevent OOM,
+            'builder': DepthwiseTreeBuilder - the instance of tree builder, contains training params,
+
+            'num_iter': int, current number of iteration,
+            'iter_scores': list of float - list of metric values for all validation sets for the last iteration,
+        }
+
+    """
+
+    def before_train(self, build_info):
+        """Actions to be made before train starts
+
+        Args:
+            build_info: dict
+
+        Returns:
+
+        """
+        return
+
+    def before_iteration(self, build_info):
+        """Actions to be made before each iteration starts
+
+        Args:
+            build_info: dict
+
+        Returns:
+
+        """
+        return
+
+    def after_iteration(self, build_info):
+        """Actions to be made after each iteration finishes
+
+        Args:
+            build_info: dict
+
+        Returns:
+            bool, if train process should be terminated
+        """
+        return False
+
+    def after_train(self, build_info):
+        """Actions to be made before train finishes
+
+        Args:
+            build_info:
+
+        Returns:
+
+        """
+        return
+
+
+class CallbackPipeline:
+    """Sequential pipeline of callbacks"""
+
+    def __init__(self, *callbacks):
+        self.callbacks = callbacks
+
+    def after_iteration(self, build_info):
+        stop = False
+
+        for callback in self.callbacks:
+            stop = stop or callback.after_iteration(build_info)
+
+        return stop
+
+    def after_train(self, build_info):
+
+        for callback in self.callbacks:
+            callback.after_train(build_info)
+
+    def before_train(self, build_info):
+
+        for callback in self.callbacks:
+            callback.before_train(build_info)
+
+    def before_iteration(self, build_info):
+
+        for callback in self.callbacks:
+            callback.before_iteration(build_info)
+
+
+class EvalHistory(Callback):
+    """Callback for history evaluation"""
+
+    def __init__(self, history, verbose=0):
+
+        self.history = history
+        self.verbose = verbose
+        self.metric = None
+        self.postprocess_fn = None
+        self.ntrees = None
+
+    def before_train(self, build_info):
+        """Init params and logger
+
+        Args:
+            build_info: dict
+
+        Returns:
+
+        """
+        self.metric = build_info['model'].metric
+        self.postprocess_fn = build_info['model'].loss.postprocess_output
+        self.ntrees = build_info['model'].ntrees
+
+        self.set_verbosity_level(int(self.verbose > 0) * 1)
+
+        msg = 'GDBT train starts. Max iter {0}, early stopping rounds {1}'.format(
+            build_info['model'].ntrees, build_info['model'].es)
+
+        logger.info(msg)
+
+    def after_iteration(self, build_info):
+        """Save the iteration results and output log
+
+        Args:
+            build_info: dict
+
+        Returns:
+
+        """
+        valid = build_info['data']['valid']
+        y_val, val_ens, w_val = valid['target'], valid['ensemble'], valid['sample_weight']
+
+        num_iter = build_info['num_iter']
+
+        msg = 'Iter {0}; '.format(num_iter)
+
+        if self.metric is None:
+            return
+
+        alias = self.metric.alias
+
+        if len(y_val) > 0:
+            val_metric = [float(self.metric(y, self.postprocess_fn(x), w)) for (y, x, w) in zip(y_val, val_ens, w_val)]
+            self.history.append(val_metric)
+
+            msg += ' '.join(['Sample {0}, {1} = {2}; '.format(n, alias, x) for (n, x) in enumerate(val_metric)])
+
+            build_info['iter_score'] = val_metric
+
+        if ((num_iter % self.verbose) == 0) or (num_iter == (self.ntrees - 1)):
+            logger.info(msg)
+
+    @staticmethod
+    def set_verbosity_level(verbose):
+        """Verbosity level setter.
+
+        Args:
+            verbose: Controls the verbosity: the higher, the more messages.
+                <1  : messages are not displayed;
+                >=1 : the computation process for layers is displayed;
+                >=2 : the information about folds processing is also displayed;
+                >=3 : the hyperparameters optimization process is also displayed;
+                >=4 : the training process for every algorithm is displayed;
+        """
+        level = verbosity_to_loglevel(verbose)
+        set_stdout_level(level)
+
+        logger.info(f"Stdout logging level is {logging._levelToName[level]}.")
+
+
+class EarlyStopping(Callback):
+    """Callback for early stopping"""
+
+    def __init__(self, num_rounds=100):
+
+        self.num_rounds = num_rounds
+        self.best_round = 1
+        self.no_upd_rounds = 0
+        self.best_score = None
+        self.metric = None
+
+    def before_train(self, build_info):
+        """Init params
+
+        Args:
+            build_info: dict
+
+        Returns:
+
+        """
+        self.metric = build_info['model'].metric
+
+    def after_iteration(self, build_info):
+        """Check early stopping condition and update the state
+
+        Args:
+            build_info: dict
+
+        Returns:
+            bool, if early stopping condition was met
+        """
+        if ('iter_score' not in build_info) or (self.num_rounds == 0):
+            return False
+
+        num_iter = build_info['num_iter']
+        # if multiple valid sets passed - use the last one
+        score = build_info['iter_score'][-1]
+
+        if num_iter == 0:
+            self.best_score = score
+            return False
+
+        if self.metric.compare(score, self.best_score):
+            self.best_score = score
+            self.best_round = num_iter + 1
+            self.no_upd_rounds = 0
+            return False
+
+        self.no_upd_rounds += 1
+
+        stop = self.no_upd_rounds >= self.num_rounds
+
+        if stop:
+            msg = 'Early stopping at iter {0}, best iter {1}, best_score {2}'.format(
+                num_iter + 1, self.best_round, self.best_score)
+            logger.info(msg)
+
+        return stop
+
+    def after_train(self, build_info):
+        """Prune the model to the best iteration
+
+        Args:
+            build_info: dict
+
+        Returns:
+
+        """
+        if self.best_score is not None:
+            model = build_info['model']
+            model.models = model.models[:self.best_round]
+            model.best_round = self.best_round
```

### Comparing `py_boost-0.4.3/py_boost/cv/adaptive_es.py` & `py_boost-0.5.0/py_boost/cv/adaptive_es.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,331 +1,331 @@
-"""Adaptive early stopping"""
-
-import numpy as np
-try:
-    import cupy as cp
-except Exception:
-    pass
-from copy import deepcopy
-from numba import njit
-
-from ..gpu.losses import MSELoss, CrossEntropyLoss, BCELoss, loss_alias
-from ..gpu.utils import validate_input
-
-from .base import CrossValidation
-
-
-def check_input(y_true, sample_weight):
-    if len(y_true.shape) == 1:
-        y_true = y_true[:, np.newaxis]
-
-    y_true = y_true[np.newaxis, :, :]
-
-    if sample_weight is not None and len(sample_weight.shape) == 1:
-        sample_weight = sample_weight[:, np.newaxis]
-
-    return y_true, sample_weight
-
-
-def bce_scorer(y_true, y_pred, sample_weight=None):
-    """
-
-    Args:
-        y_true: (nobj, nout)
-        y_pred: (niter, nobj, nout)
-        sample_weight: (nobj, 1)
-
-    Returns:
-
-    """
-    y_true, sample_weight = check_input(y_true, sample_weight)
-
-    path = -np.log(y_true * y_pred + (1 - y_true) * (1 - y_pred))
-    path = path.sum(axis=-1).T
-
-    if sample_weight is not None:
-        path *= sample_weight
-
-    return path
-
-
-def mse_scorer(y_true, y_pred, sample_weight=None):
-    """
-
-    Args:
-        y_true: (nobj, nout)
-        y_pred: (niter, nobj, nout)
-        sample_weight: (nobj, 1)
-
-    Returns:
-
-    """
-    y_true, sample_weight = check_input(y_true, sample_weight)
-
-    path = (y_true - y_pred) ** 2
-    path = path.sum(axis=-1).T
-
-    if sample_weight is not None:
-        path *= sample_weight
-
-    return path
-
-
-def cent_scorer(y_true, y_pred, sample_weight=None):
-    """
-
-    Args:
-        y_true: (nobj, nout)
-        y_pred: (niter, nobj, nout)
-        sample_weight: (nobj, 1)
-
-    Returns:
-
-    """
-    y_true, sample_weight = check_input(y_true, sample_weight)
-
-    path = -np.log(np.take_along_axis(y_pred, y_true, axis=2)[..., 0].T)
-
-    if sample_weight is not None:
-        path *= sample_weight
-
-    return path
-
-
-@njit
-def select_preds(arr, leaves, order):
-    """Select corresponding to cluster prediction
-
-    Args:
-        arr: np.ndarray, predictions
-        leaves: np.ndarray, clusters
-        order: np.ndarray, maps cluster label with position in prediction array
-
-    Returns:
-        np.ndarray, pruned prediction
-    """
-    res = np.empty(arr.shape[1:], dtype=arr.dtype)
-
-    for i in range(leaves.shape[0]):
-        res[i] = arr[order[leaves[i]], i, :]
-
-    return res
-
-
-class AdaptiveESCV(CrossValidation):
-    """
-    Cross validation wrapper with built-in adaptive early stopping
-    """
-
-    def __init__(self, base_learner, cluster, iters_to_fit, metric=None, random_state=42, batch_size=10000):
-        super().__init__(deepcopy(base_learner), random_state)
-        self._base_learner.params['es'] = 0
-        self.cluster = cluster
-        self.iters_to_fit = iters_to_fit
-        self.metric = metric
-        self.batch_size = batch_size
-
-        self.best_split = None
-        self.best_trees = None
-        self.best_oof_trees = None
-
-    def get_es_metric(self):
-
-        if self.metric:
-            return self.metric
-
-        loss = self._base_learner.params['loss']
-        if type(loss) is str:
-            loss = loss_alias[loss]
-
-        if type(loss) is MSELoss:
-            return mse_scorer
-
-        if type(loss) is BCELoss:
-            return bce_scorer
-
-        if type(loss) is CrossEntropyLoss:
-            return cent_scorer
-
-        raise ValueError('Unknown loss func. Please specify metric manually')
-
-    def fit_predict(self, X, y, sample_weight=None, cv=5, stratify=False, random_state=42):
-        """
-
-        Args:
-            X:
-            y:
-            sample_weight:
-            cv:
-            stratify:
-            random_state:
-
-        Returns:
-
-        """
-        assert self.models is None, 'Is already trained'
-
-        self.models = []
-
-        X, y, sample_weight, eval_sets = validate_input(X, y, sample_weight, {})
-        self._base_learner._infer_params()
-        X_enc, max_bin, borders, eval_enc = self._base_learner.quantize(X, eval_sets)
-
-        # create validation
-        cv_iter = self.get_cv_iter(cv, stratify, random_state)
-
-        # fit and free memory
-        mempool = cp.cuda.MemoryPool()
-
-        oof_pred, folds = self._fit_predict(mempool, X, X_enc, y, sample_weight, max_bin, borders, cv_iter)
-        self.fit_cluster_tree(X, X_enc, y, sample_weight, max_bin, borders, folds)
-        self.search_for_best_cluster(X, y, sample_weight, folds)
-
-        # create out of fold pruned prediction
-
-        for f in range(folds.max() + 1):
-            idx = np.arange(X_enc.shape[0])[folds == f]
-            X_test = X[idx]
-            pred = self._get_stages([self.models[f]], self.best_oof_trees[f], X_test, batch_size=self.batch_size)
-            oof_pred[idx] = self._prune_preds(self.best_oof_trees[f], X_test, pred, batch_size=self.batch_size)
-
-        return oof_pred
-
-    def fit_cluster_tree(self, X, X_enc, y, sample_weight, max_bin, borders, folds):
-        """Fit cluster tree
-
-        Args:
-            X:
-            X_enc:
-            y:
-            sample_weight:
-            max_bin:
-            borders:
-            folds:
-
-        Returns:
-
-        """
-        paths = np.zeros((X_enc.shape[0], len(self.iters_to_fit)), dtype=np.float32)
-        scorer = self.get_es_metric()
-
-        for f in range(folds.max() + 1):
-            idx = np.arange(X_enc.shape[0])[folds == f]
-            val_pred = self.models[f].predict_staged(X[idx], iterations=self.iters_to_fit)
-            paths[idx] = scorer(y[idx], val_pred, None if sample_weight is None else sample_weight[idx])
-
-        self.cluster.fit_quantized(X_enc, paths, max_bin, borders)
-        self.cluster.to_cpu()
-
-    def search_for_best_cluster(self, X, y, sample_weight, folds):
-        """Search for the best cluster tree
-
-        Args:
-            X:
-            y:
-            sample_weight:
-            folds:
-
-        Returns:
-
-        """
-        # predict cluster trees
-        cl_ = self.cluster.predict(X)
-        # zero clustering is a simple early stopping
-        clusters = np.zeros((cl_.shape[0], cl_.shape[1] + 1), dtype=np.uint32)
-        clusters[:, 1:] = cl_
-
-        scorer = self.get_es_metric()
-        n_cand = clusters.shape[1]
-        clust_per_split = clusters.max(axis=0) + 1
-        nfolds = folds.max() + 1
-        max_clust = clust_per_split.max()
-        iter_num = self._base_learner.params['ntrees']
-        batch_size = 1000
-
-        folds_stats = np.zeros((nfolds, n_cand, max_clust, iter_num), dtype=np.float32)
-
-        # calculate oof errors
-        for f in range(nfolds):
-            idx = np.arange(X.shape[0])[folds == f]
-            X_test, y_test, cl_test = X[idx], y[idx], clusters[idx]
-
-            for i in range(0, X_test.shape[0], batch_size):
-
-                val_pred = self.models[f].predict_staged(X_test[i:i + batch_size])
-                err = scorer(y_test[i:i + batch_size], val_pred,
-                             None if sample_weight is None else sample_weight[i:i + batch_size])
-
-                for j in range(n_cand):
-                    np.add.at(folds_stats[f, j], (cl_test[i:i + batch_size, j],), err)
-
-        # select best by oof
-        stats = folds_stats.sum(axis=0)  # shape (nsplits, max_clust, niters)
-        oof_stats = stats[np.newaxis, ...] - folds_stats  # shape (nfolds, nsplits, max_clust, niters)
-
-        best_iters = oof_stats.argmin(axis=-1)  # shape (nfolds, nsplits, max_clust)
-        best_errs = np.take_along_axis(folds_stats, best_iters[..., np.newaxis], axis=3)[..., 0].sum(
-            axis=0)  # shape  (nsplits, max_clust)
-        self.best_split = best_errs.sum(axis=1).argmin()  # scalar
-        best_oof_trees = best_iters[:, self.best_split]  # shape (nfolds, max_clust)
-        self.best_oof_trees = best_oof_trees[:, :clust_per_split[self.best_split]]
-
-        # select best in total
-        best_trees = stats[self.best_split].argmin(axis=-1)  # shape (max_clust, )
-        self.best_trees = best_trees[:clust_per_split[self.best_split]]
-
-    def _get_stages(self, models, iters, X, batch_size=100000):
-        """
-
-        Args:
-            models:
-            iters:
-            X:
-            batch_size:
-
-        Returns:
-
-        """
-        sorted_iters = np.sort(np.unique(iters))
-        pred = models[0].predict_staged(X, iterations=sorted_iters, batch_size=batch_size)
-
-        for i in range(1, len(models)):
-            pred += models[i].predict_staged(X, iterations=sorted_iters, batch_size=batch_size)
-
-        pred /= len(models)
-
-        return pred
-
-    def _prune_preds(self, iters, X, pred, batch_size=100000):
-        """
-
-        Args:
-            iters:
-            X:
-            pred:
-            batch_size:
-
-        Returns:
-
-        """
-        if self.best_split == 0:
-            cluster = np.zeros((X.shape[0],), dtype=np.uint32)
-        else:
-            cluster = self.cluster.predict(X, iterations=[self.best_split - 1], batch_size=batch_size)[:, 0]
-
-        sorted_iters = np.sort(np.unique(iters))
-        order = np.searchsorted(sorted_iters, iters)
-
-        return select_preds(pred, cluster, order)
-
-    def predict(self, X, batch_size=100000):
-        """
-
-        Args:
-            X:
-            batch_size:
-
-        Returns:
-
-        """
-        pred = self._get_stages(self.models, self.best_trees, X, batch_size=batch_size)
-        return self._prune_preds(self.best_trees, X, pred, batch_size=batch_size)
+"""Adaptive early stopping"""
+
+import numpy as np
+try:
+    import cupy as cp
+except Exception:
+    pass
+from copy import deepcopy
+from numba import njit
+
+from ..gpu.losses import MSELoss, CrossEntropyLoss, BCELoss, loss_alias
+from ..gpu.utils import validate_input
+
+from .base import CrossValidation
+
+
+def check_input(y_true, sample_weight):
+    if len(y_true.shape) == 1:
+        y_true = y_true[:, np.newaxis]
+
+    y_true = y_true[np.newaxis, :, :]
+
+    if sample_weight is not None and len(sample_weight.shape) == 1:
+        sample_weight = sample_weight[:, np.newaxis]
+
+    return y_true, sample_weight
+
+
+def bce_scorer(y_true, y_pred, sample_weight=None):
+    """
+
+    Args:
+        y_true: (nobj, nout)
+        y_pred: (niter, nobj, nout)
+        sample_weight: (nobj, 1)
+
+    Returns:
+
+    """
+    y_true, sample_weight = check_input(y_true, sample_weight)
+
+    path = -np.log(y_true * y_pred + (1 - y_true) * (1 - y_pred))
+    path = path.sum(axis=-1).T
+
+    if sample_weight is not None:
+        path *= sample_weight
+
+    return path
+
+
+def mse_scorer(y_true, y_pred, sample_weight=None):
+    """
+
+    Args:
+        y_true: (nobj, nout)
+        y_pred: (niter, nobj, nout)
+        sample_weight: (nobj, 1)
+
+    Returns:
+
+    """
+    y_true, sample_weight = check_input(y_true, sample_weight)
+
+    path = (y_true - y_pred) ** 2
+    path = path.sum(axis=-1).T
+
+    if sample_weight is not None:
+        path *= sample_weight
+
+    return path
+
+
+def cent_scorer(y_true, y_pred, sample_weight=None):
+    """
+
+    Args:
+        y_true: (nobj, nout)
+        y_pred: (niter, nobj, nout)
+        sample_weight: (nobj, 1)
+
+    Returns:
+
+    """
+    y_true, sample_weight = check_input(y_true, sample_weight)
+
+    path = -np.log(np.take_along_axis(y_pred, y_true, axis=2)[..., 0].T)
+
+    if sample_weight is not None:
+        path *= sample_weight
+
+    return path
+
+
+@njit
+def select_preds(arr, leaves, order):
+    """Select corresponding to cluster prediction
+
+    Args:
+        arr: np.ndarray, predictions
+        leaves: np.ndarray, clusters
+        order: np.ndarray, maps cluster label with position in prediction array
+
+    Returns:
+        np.ndarray, pruned prediction
+    """
+    res = np.empty(arr.shape[1:], dtype=arr.dtype)
+
+    for i in range(leaves.shape[0]):
+        res[i] = arr[order[leaves[i]], i, :]
+
+    return res
+
+
+class AdaptiveESCV(CrossValidation):
+    """
+    Cross validation wrapper with built-in adaptive early stopping
+    """
+
+    def __init__(self, base_learner, cluster, iters_to_fit, metric=None, random_state=42, batch_size=10000):
+        super().__init__(deepcopy(base_learner), random_state)
+        self._base_learner.params['es'] = 0
+        self.cluster = cluster
+        self.iters_to_fit = iters_to_fit
+        self.metric = metric
+        self.batch_size = batch_size
+
+        self.best_split = None
+        self.best_trees = None
+        self.best_oof_trees = None
+
+    def get_es_metric(self):
+
+        if self.metric:
+            return self.metric
+
+        loss = self._base_learner.params['loss']
+        if type(loss) is str:
+            loss = loss_alias[loss]
+
+        if type(loss) is MSELoss:
+            return mse_scorer
+
+        if type(loss) is BCELoss:
+            return bce_scorer
+
+        if type(loss) is CrossEntropyLoss:
+            return cent_scorer
+
+        raise ValueError('Unknown loss func. Please specify metric manually')
+
+    def fit_predict(self, X, y, sample_weight=None, cv=5, stratify=False, random_state=42):
+        """
+
+        Args:
+            X:
+            y:
+            sample_weight:
+            cv:
+            stratify:
+            random_state:
+
+        Returns:
+
+        """
+        assert self.models is None, 'Is already trained'
+
+        self.models = []
+
+        X, y, sample_weight, eval_sets = validate_input(X, y, sample_weight, {})
+        self._base_learner._infer_params()
+        X_enc, max_bin, borders, eval_enc = self._base_learner.quantize(X, eval_sets)
+
+        # create validation
+        cv_iter = self.get_cv_iter(cv, stratify, random_state)
+
+        # fit and free memory
+        mempool = cp.cuda.MemoryPool()
+
+        oof_pred, folds = self._fit_predict(mempool, X, X_enc, y, sample_weight, max_bin, borders, cv_iter)
+        self.fit_cluster_tree(X, X_enc, y, sample_weight, max_bin, borders, folds)
+        self.search_for_best_cluster(X, y, sample_weight, folds)
+
+        # create out of fold pruned prediction
+
+        for f in range(folds.max() + 1):
+            idx = np.arange(X_enc.shape[0])[folds == f]
+            X_test = X[idx]
+            pred = self._get_stages([self.models[f]], self.best_oof_trees[f], X_test, batch_size=self.batch_size)
+            oof_pred[idx] = self._prune_preds(self.best_oof_trees[f], X_test, pred, batch_size=self.batch_size)
+
+        return oof_pred
+
+    def fit_cluster_tree(self, X, X_enc, y, sample_weight, max_bin, borders, folds):
+        """Fit cluster tree
+
+        Args:
+            X:
+            X_enc:
+            y:
+            sample_weight:
+            max_bin:
+            borders:
+            folds:
+
+        Returns:
+
+        """
+        paths = np.zeros((X_enc.shape[0], len(self.iters_to_fit)), dtype=np.float32)
+        scorer = self.get_es_metric()
+
+        for f in range(folds.max() + 1):
+            idx = np.arange(X_enc.shape[0])[folds == f]
+            val_pred = self.models[f].predict_staged(X[idx], iterations=self.iters_to_fit)
+            paths[idx] = scorer(y[idx], val_pred, None if sample_weight is None else sample_weight[idx])
+
+        self.cluster.fit_quantized(X_enc, paths, max_bin, borders)
+        self.cluster.to_cpu()
+
+    def search_for_best_cluster(self, X, y, sample_weight, folds):
+        """Search for the best cluster tree
+
+        Args:
+            X:
+            y:
+            sample_weight:
+            folds:
+
+        Returns:
+
+        """
+        # predict cluster trees
+        cl_ = self.cluster.predict(X)
+        # zero clustering is a simple early stopping
+        clusters = np.zeros((cl_.shape[0], cl_.shape[1] + 1), dtype=np.uint32)
+        clusters[:, 1:] = cl_
+
+        scorer = self.get_es_metric()
+        n_cand = clusters.shape[1]
+        clust_per_split = clusters.max(axis=0) + 1
+        nfolds = folds.max() + 1
+        max_clust = clust_per_split.max()
+        iter_num = self._base_learner.params['ntrees']
+        batch_size = 1000
+
+        folds_stats = np.zeros((nfolds, n_cand, max_clust, iter_num), dtype=np.float32)
+
+        # calculate oof errors
+        for f in range(nfolds):
+            idx = np.arange(X.shape[0])[folds == f]
+            X_test, y_test, cl_test = X[idx], y[idx], clusters[idx]
+
+            for i in range(0, X_test.shape[0], batch_size):
+
+                val_pred = self.models[f].predict_staged(X_test[i:i + batch_size])
+                err = scorer(y_test[i:i + batch_size], val_pred,
+                             None if sample_weight is None else sample_weight[i:i + batch_size])
+
+                for j in range(n_cand):
+                    np.add.at(folds_stats[f, j], (cl_test[i:i + batch_size, j],), err)
+
+        # select best by oof
+        stats = folds_stats.sum(axis=0)  # shape (nsplits, max_clust, niters)
+        oof_stats = stats[np.newaxis, ...] - folds_stats  # shape (nfolds, nsplits, max_clust, niters)
+
+        best_iters = oof_stats.argmin(axis=-1)  # shape (nfolds, nsplits, max_clust)
+        best_errs = np.take_along_axis(folds_stats, best_iters[..., np.newaxis], axis=3)[..., 0].sum(
+            axis=0)  # shape  (nsplits, max_clust)
+        self.best_split = best_errs.sum(axis=1).argmin()  # scalar
+        best_oof_trees = best_iters[:, self.best_split]  # shape (nfolds, max_clust)
+        self.best_oof_trees = best_oof_trees[:, :clust_per_split[self.best_split]]
+
+        # select best in total
+        best_trees = stats[self.best_split].argmin(axis=-1)  # shape (max_clust, )
+        self.best_trees = best_trees[:clust_per_split[self.best_split]]
+
+    def _get_stages(self, models, iters, X, batch_size=100000):
+        """
+
+        Args:
+            models:
+            iters:
+            X:
+            batch_size:
+
+        Returns:
+
+        """
+        sorted_iters = np.sort(np.unique(iters))
+        pred = models[0].predict_staged(X, iterations=sorted_iters, batch_size=batch_size)
+
+        for i in range(1, len(models)):
+            pred += models[i].predict_staged(X, iterations=sorted_iters, batch_size=batch_size)
+
+        pred /= len(models)
+
+        return pred
+
+    def _prune_preds(self, iters, X, pred, batch_size=100000):
+        """
+
+        Args:
+            iters:
+            X:
+            pred:
+            batch_size:
+
+        Returns:
+
+        """
+        if self.best_split == 0:
+            cluster = np.zeros((X.shape[0],), dtype=np.uint32)
+        else:
+            cluster = self.cluster.predict(X, iterations=[self.best_split - 1], batch_size=batch_size)[:, 0]
+
+        sorted_iters = np.sort(np.unique(iters))
+        order = np.searchsorted(sorted_iters, iters)
+
+        return select_preds(pred, cluster, order)
+
+    def predict(self, X, batch_size=100000):
+        """
+
+        Args:
+            X:
+            batch_size:
+
+        Returns:
+
+        """
+        pred = self._get_stages(self.models, self.best_trees, X, batch_size=batch_size)
+        return self._prune_preds(self.best_trees, X, pred, batch_size=batch_size)
```

### Comparing `py_boost-0.4.3/py_boost/cv/base.py` & `py_boost-0.5.0/py_boost/cv/base.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-"""Gradient Boosting with built-in cross validation"""
-
-import numpy as np
-try:
-    import cupy as cp
-except Exception:
-    pass
-from copy import deepcopy
-
-from sklearn.model_selection import KFold, StratifiedKFold
-from ..gpu.utils import validate_input
-
-
-class CustomFolds:
-    """
-    Class to imitate sklearn cv for custom folds
-    """
-
-    def __init__(self, folds):
-        self.folds = folds
-
-    def split(self, *args, **kwargs):
-        nfolds = int(self.folds.max() + 1)
-        idx = np.arange(len(self.folds))
-
-        splits = []
-
-        for i in range(nfolds):
-            splits.append((idx[self.folds != i], idx[self.folds == i]))
-
-        return splits
-
-
-class CrossValidation:
-    """
-    Cross validation wrapper for gradient boosting
-    """
-
-    def __init__(self, base_learner, random_state=42):
-        """
-
-        Args:
-            base_learner:
-            random_state:
-        """
-        self._base_learner = base_learner
-        self.random_state = random_state
-        self.models = None
-
-    def _fit_predict(self, mempool, X, X_enc, y, sample_weight, max_bin, borders, cv_iter):
-
-        oof_pred = None
-        folds = np.zeros(X.shape[0], dtype=np.int32)
-
-        with cp.cuda.using_allocator(allocator=mempool.malloc):
-
-            for n, (f0, f1) in enumerate(cv_iter.split(X, y)):
-
-                # split data
-
-                X_tr, X_enc_tr, y_tr, = X[f0], X_enc[f0], y[f0]
-
-                sample_weight_tr = None
-                if sample_weight is not None:
-                    sample_weight_tr = sample_weight[f0]
-
-                eval_sets = [{
-
-                    'X': X[f1],
-                    'y': y[f1],
-                    'sample_weight': None if sample_weight is None else sample_weight[f1]
-
-                }]
-
-                eval_enc = [X_enc[f1]]
-
-                # fit model
-                model = deepcopy(self._base_learner)
-                model._infer_params()
-                builder, build_info = model._create_build_info(mempool, X_tr, X_enc_tr, y_tr, sample_weight_tr,
-                                                               max_bin, borders, eval_sets, eval_enc)
-                model._fit(builder, build_info)
-
-                # predict
-
-                val_pred = model.predict(eval_sets[0]['X'])
-                model.to_cpu()
-
-                if oof_pred is None:
-                    oof_pred = np.zeros((X.shape[0], val_pred.shape[1]), dtype=np.float32)
-
-                oof_pred[f1] = val_pred
-                folds[f1] = n
-                self.models.append(model)
-
-                mempool.free_all_blocks()
-
-        return oof_pred, folds
-
-    def get_cv_iter(self, cv, stratify, random_state):
-
-        if type(cv) in [int, float]:
-            cv = int(cv)
-            if stratify:
-                folds = StratifiedKFold(cv, shuffle=True, random_state=random_state)
-            else:
-                folds = KFold(cv, shuffle=True)
-
-        else:
-            folds = CustomFolds(cv)
-
-        return folds
-
-    def fit_predict(self, X, y, sample_weight=None, cv=5, stratify=False, random_state=42):
-        """
-
-        Args:
-            X:
-            y:
-            sample_weight:
-            cv:
-            stratify:
-            random_state:
-
-        Returns:
-
-        """
-        assert self.models is None, 'Is already trained'
-
-        self.models = []
-
-        X, y, sample_weight, eval_sets = validate_input(X, y, sample_weight, {})
-        self._base_learner._infer_params()
-        X_enc, max_bin, borders, eval_enc = self._base_learner.quantize(X, eval_sets)
-
-        # create validation
-        cv_iter = self.get_cv_iter(cv, stratify, random_state)
-
-        # fit and free memory
-        mempool = cp.cuda.MemoryPool()
-
-        oof_pred, folds = self._fit_predict(mempool, X, X_enc, y, sample_weight, max_bin, borders, cv_iter)
-
-        return oof_pred
-
-    def predict(self, X):
-        """
-
-        Args:
-            X:
-
-        Returns:
-
-        """
-        res = None
-
-        for model in self.models:
-
-            pred = model.predict(X)
-            if res is None:
-                res = pred
-            else:
-                res += pred
-
-        res /= len(self.models)
-
-        return res
+"""Gradient Boosting with built-in cross validation"""
+
+import numpy as np
+try:
+    import cupy as cp
+except Exception:
+    pass
+from copy import deepcopy
+
+from sklearn.model_selection import KFold, StratifiedKFold
+from ..gpu.utils import validate_input
+
+
+class CustomFolds:
+    """
+    Class to imitate sklearn cv for custom folds
+    """
+
+    def __init__(self, folds):
+        self.folds = folds
+
+    def split(self, *args, **kwargs):
+        nfolds = int(self.folds.max() + 1)
+        idx = np.arange(len(self.folds))
+
+        splits = []
+
+        for i in range(nfolds):
+            splits.append((idx[self.folds != i], idx[self.folds == i]))
+
+        return splits
+
+
+class CrossValidation:
+    """
+    Cross validation wrapper for gradient boosting
+    """
+
+    def __init__(self, base_learner, random_state=42):
+        """
+
+        Args:
+            base_learner:
+            random_state:
+        """
+        self._base_learner = base_learner
+        self.random_state = random_state
+        self.models = None
+
+    def _fit_predict(self, mempool, X, X_enc, y, sample_weight, max_bin, borders, cv_iter):
+
+        oof_pred = None
+        folds = np.zeros(X.shape[0], dtype=np.int32)
+
+        with cp.cuda.using_allocator(allocator=mempool.malloc):
+
+            for n, (f0, f1) in enumerate(cv_iter.split(X, y)):
+
+                # split data
+
+                X_tr, X_enc_tr, y_tr, = X[f0], X_enc[f0], y[f0]
+
+                sample_weight_tr = None
+                if sample_weight is not None:
+                    sample_weight_tr = sample_weight[f0]
+
+                eval_sets = [{
+
+                    'X': X[f1],
+                    'y': y[f1],
+                    'sample_weight': None if sample_weight is None else sample_weight[f1]
+
+                }]
+
+                eval_enc = [X_enc[f1]]
+
+                # fit model
+                model = deepcopy(self._base_learner)
+                model._infer_params()
+                builder, build_info = model._create_build_info(mempool, X_tr, X_enc_tr, y_tr, sample_weight_tr,
+                                                               max_bin, borders, eval_sets, eval_enc)
+                model._fit(builder, build_info)
+
+                # predict
+
+                val_pred = model.predict(eval_sets[0]['X'])
+                model.to_cpu()
+
+                if oof_pred is None:
+                    oof_pred = np.zeros((X.shape[0], val_pred.shape[1]), dtype=np.float32)
+
+                oof_pred[f1] = val_pred
+                folds[f1] = n
+                self.models.append(model)
+
+                mempool.free_all_blocks()
+
+        return oof_pred, folds
+
+    def get_cv_iter(self, cv, stratify, random_state):
+
+        if type(cv) in [int, float]:
+            cv = int(cv)
+            if stratify:
+                folds = StratifiedKFold(cv, shuffle=True, random_state=random_state)
+            else:
+                folds = KFold(cv, shuffle=True)
+
+        else:
+            folds = CustomFolds(cv)
+
+        return folds
+
+    def fit_predict(self, X, y, sample_weight=None, cv=5, stratify=False, random_state=42):
+        """
+
+        Args:
+            X:
+            y:
+            sample_weight:
+            cv:
+            stratify:
+            random_state:
+
+        Returns:
+
+        """
+        assert self.models is None, 'Is already trained'
+
+        self.models = []
+
+        X, y, sample_weight, eval_sets = validate_input(X, y, sample_weight, {})
+        self._base_learner._infer_params()
+        X_enc, max_bin, borders, eval_enc = self._base_learner.quantize(X, eval_sets)
+
+        # create validation
+        cv_iter = self.get_cv_iter(cv, stratify, random_state)
+
+        # fit and free memory
+        mempool = cp.cuda.MemoryPool()
+
+        oof_pred, folds = self._fit_predict(mempool, X, X_enc, y, sample_weight, max_bin, borders, cv_iter)
+
+        return oof_pred
+
+    def predict(self, X):
+        """
+
+        Args:
+            X:
+
+        Returns:
+
+        """
+        res = None
+
+        for model in self.models:
+
+            pred = model.predict(X)
+            if res is None:
+                res = pred
+            else:
+                res += pred
+
+        res /= len(self.models)
+
+        return res
```

### Comparing `py_boost-0.4.3/py_boost/cv/cluster_tree.py` & `py_boost-0.5.0/py_boost/cv/cluster_tree.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,198 +1,198 @@
-from ..gpu.utils import *
-from ..gpu.tree import *
-from ..gpu.base import Ensemble
-
-from ..quantization.base import QuantileQuantizer
-
-
-def cluster_grow_tree(tree, group, arr, grad, hess, row_indexer, col_indexer, params):
-    """Graw tree for advanced pruning
-
-    Args:
-        tree:
-        group:
-        arr:
-        grad:
-        hess:
-        row_indexer:
-        col_indexer:
-        params:
-
-    Returns:
-
-    """
-    # create gh
-    gh = cp.concatenate((grad, hess), axis=1)
-    out_indexer = cp.arange(gh.shape[1], dtype=cp.uint64)
-
-    # init nodes with single zero node
-    unique_nodes = np.zeros(1, dtype=np.int32)
-    # count unique nodes in active rows
-    nodes_count = cp.ones(1, dtype=cp.uint64) * row_indexer.shape[0]
-    # nodes for all rows
-    nodes = cp.zeros(arr.shape[0], dtype=cp.int32)
-    # index of node in unique array
-    node_indexes = nodes
-    prev_hist, small_index, big_index = [None] * 3
-
-    for niter in range(params['max_depth']):
-
-        nnodes = len(unique_nodes)
-        gh_hist = histogram(arr, gh, node_indexes,
-                            col_indexer=col_indexer,
-                            row_indexer=row_indexer,
-                            out_indexer=out_indexer,
-                            nnodes=nnodes,
-                            max_bins=params['max_bin'],
-                            prev_hist=prev_hist,
-                            small_index=small_index,
-                            big_index=big_index)
-
-        # assume hess is the last output
-
-        hist, counts = gh_hist[:-1], gh_hist[-1]
-        total = hist[..., :1, -1:]
-        curr = total.min(axis=0)
-        gain = cp.zeros(hist.shape[1:] + (2,), dtype=cp.float32)
-
-        # NAN to left
-        gain[..., 0] = curr - hist.min(axis=0) - (total - hist).min(axis=0)
-        gain[..., 0] *= cp.minimum(counts, counts[..., -1:] - counts) >= params['min_data_in_leaf']
-
-        # NAN to right
-        gain[..., 1] = curr - (hist - hist[..., :1]).min(axis=0) - (total - hist + hist[..., :1]).min(axis=0)
-        gain[..., 1] *= cp.minimum(counts - counts[..., :1:], counts[..., -1:] - counts + counts[..., :1]) >= params[
-            'min_data_in_leaf']
-
-        best_feat, best_gain, best_split, best_nan_left = get_best_split(gain, col_indexer)
-
-        # move to CPU and apply min_gain_to_split condition
-        unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left, is_valid_node = \
-            get_cpu_splitters(unique_nodes, best_feat, best_gain, best_split, best_nan_left,
-                              params['min_gain_to_split'])
-        # if all nodes are not valid to split - exit
-        if len(unique_nodes) == 0:
-            break
-        # write node info to the Tree
-        tree.set_nodes(group, unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left)
-        # get args back on gpu
-        split_args, unique_nodes = get_gpu_splitters(unique_nodes, new_nodes_id,
-                                                     best_feat, best_split, best_nan_left)
-
-        # perform split for train set
-        nodes, node_indexes = make_split(nodes, arr, *split_args, return_pos=True)
-
-        # update info for the next step
-        if niter < (params['max_depth'] - 1):
-            # update counts
-            nodes_count = cp.zeros((unique_nodes.shape[0] + 1,), dtype=np.uint64)
-            nodes_count.scatter_add(node_indexes[row_indexer], 1)
-            nodes_count = nodes_count[:-1]
-
-            cpu_counts = nodes_count.get()
-
-            # remove unused rows from indexer
-            if cpu_counts.sum() < row_indexer.shape[0]:
-                row_indexer = row_indexer[isin(nodes, split_args[1].ravel(), index=row_indexer)]
-
-            # save histogram for the subs trick
-            prev_hist, small_index, big_index = get_prev_hist(cpu_counts,
-                                                              gh_hist, cp.asarray(is_valid_node))
-
-    return nodes
-
-
-class ClusterTreeBuilder:
-    """Tree builder for early stopping clusters"""
-
-    def __init__(self, borders,
-                 **tree_params
-                 ):
-        """
-
-        Args:
-            borders: list of np.ndarray, actual split borders for quantized features
-            **tree_params: other tree building parameters
-        """
-        self.borders = borders
-
-        self.params = {**{
-
-            'max_bin': 256,
-            'max_depth': 6,
-            'min_data_in_leaf': 10,
-            'min_gain_to_split': 0
-
-        }, **tree_params}
-
-    def build_tree(self, X, y):
-        """Build tree
-
-        Args:
-            X: cp.ndarray, quantized feature matrix
-            y: cp.ndarray, loss path matrix
-
-
-        Returns:
-            tree, Tree, constructed tree
-        """
-
-        col_indexer = cp.arange(X.shape[1], dtype=cp.uint64)
-        row_indexer = cp.arange(X.shape[0], dtype=cp.uint64)
-        max_nodes = int((2 ** np.arange(self.params['max_depth'] + 1)).sum())
-        tree = Tree(max_nodes, y.shape[1], 1)
-        # grow single group of the tree and get nodes index
-        cluster_grow_tree(tree, 0, X, y, cp.ones((y.shape[0], 1), dtype=cp.float32),
-                          row_indexer, col_indexer, self.params)
-
-        tree.set_borders(self.borders)
-        tree.set_leaves()
-        tree.set_node_values(np.zeros((max_nodes, 1), dtype=np.float32), np.zeros((1,), dtype=np.uint64))
-
-        return tree
-
-
-class ClusterCandidates(Ensemble):
-    """
-    Ensemble of cluster candidates
-    """
-
-    def __init__(self, depth_range=range(1, 7), min_data_in_leaf=100, debug=False):
-        super().__init__()
-
-        self._debug = debug
-        self.depth_range = depth_range
-        self.min_data_in_leaf = min_data_in_leaf
-        self.max_clust = 2 ** max(depth_range)
-
-    def fit(self, X, y):
-        X, y, sample_weight, eval_sets = validate_input(X, y, None, [])
-        mempool = cp.cuda.MemoryPool()
-        with cp.cuda.using_allocator(allocator=mempool.malloc):
-            # TODO: move quantizer to the Ensemble
-            quantizer = QuantileQuantizer(sample=self.quant_sample, max_bin=self.max_bin)
-            X_enc, max_bin, borders, eval_enc = self.quantize(X, eval_sets)
-
-            self.fit_quantized(X_enc, y, max_bin, borders)
-        mempool.free_all_blocks()
-
-        return self
-
-    def fit_quantized(self, X_enc, y, max_bin, borders):
-        y = cp.array(y, order='C', dtype=cp.float32)
-        X_cp = pad_and_move(X_enc)
-        self.models = []
-
-        for d in self.depth_range:
-            builder = ClusterTreeBuilder(borders, max_depth=d, min_data_in_leaf=self.min_data_in_leaf, max_bin=max_bin)
-
-            tree = builder.build_tree(X_cp, y)
-            tree.reformat(nfeats=X_cp.shape[1], debug=self._debug)
-            self.models.append(tree)
-
-        self.base_score = np.zeros((1,), dtype=np.float32)
-
-        return self
-
-    def predict(self, X, iterations=None, batch_size=100000):
-        return self.predict_leaves(X, iterations=iterations, batch_size=batch_size)[..., 0].T
+from ..gpu.utils import *
+from ..gpu.tree import *
+from ..gpu.base import Ensemble
+
+from ..quantization.base import QuantileQuantizer
+
+
+def cluster_grow_tree(tree, group, arr, grad, hess, row_indexer, col_indexer, params):
+    """Graw tree for advanced pruning
+
+    Args:
+        tree:
+        group:
+        arr:
+        grad:
+        hess:
+        row_indexer:
+        col_indexer:
+        params:
+
+    Returns:
+
+    """
+    # create gh
+    gh = cp.concatenate((grad, hess), axis=1)
+    out_indexer = cp.arange(gh.shape[1], dtype=cp.uint64)
+
+    # init nodes with single zero node
+    unique_nodes = np.zeros(1, dtype=np.int32)
+    # count unique nodes in active rows
+    nodes_count = cp.ones(1, dtype=cp.uint64) * row_indexer.shape[0]
+    # nodes for all rows
+    nodes = cp.zeros(arr.shape[0], dtype=cp.int32)
+    # index of node in unique array
+    node_indexes = nodes
+    prev_hist, small_index, big_index = [None] * 3
+
+    for niter in range(params['max_depth']):
+
+        nnodes = len(unique_nodes)
+        gh_hist = histogram(arr, gh, node_indexes,
+                            col_indexer=col_indexer,
+                            row_indexer=row_indexer,
+                            out_indexer=out_indexer,
+                            nnodes=nnodes,
+                            max_bins=params['max_bin'],
+                            prev_hist=prev_hist,
+                            small_index=small_index,
+                            big_index=big_index)
+
+        # assume hess is the last output
+
+        hist, counts = gh_hist[:-1], gh_hist[-1]
+        total = hist[..., :1, -1:]
+        curr = total.min(axis=0)
+        gain = cp.zeros(hist.shape[1:] + (2,), dtype=cp.float32)
+
+        # NAN to left
+        gain[..., 0] = curr - hist.min(axis=0) - (total - hist).min(axis=0)
+        gain[..., 0] *= cp.minimum(counts, counts[..., -1:] - counts) >= params['min_data_in_leaf']
+
+        # NAN to right
+        gain[..., 1] = curr - (hist - hist[..., :1]).min(axis=0) - (total - hist + hist[..., :1]).min(axis=0)
+        gain[..., 1] *= cp.minimum(counts - counts[..., :1:], counts[..., -1:] - counts + counts[..., :1]) >= params[
+            'min_data_in_leaf']
+
+        best_feat, best_gain, best_split, best_nan_left = get_best_split(gain, col_indexer)
+
+        # move to CPU and apply min_gain_to_split condition
+        unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left, is_valid_node = \
+            get_cpu_splitters(unique_nodes, best_feat, best_gain, best_split, best_nan_left,
+                              params['min_gain_to_split'])
+        # if all nodes are not valid to split - exit
+        if len(unique_nodes) == 0:
+            break
+        # write node info to the Tree
+        tree.set_nodes(group, unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left)
+        # get args back on gpu
+        split_args, unique_nodes = get_gpu_splitters(unique_nodes, new_nodes_id,
+                                                     best_feat, best_split, best_nan_left)
+
+        # perform split for train set
+        nodes, node_indexes = make_split(nodes, arr, *split_args, return_pos=True)
+
+        # update info for the next step
+        if niter < (params['max_depth'] - 1):
+            # update counts
+            nodes_count = cp.zeros((unique_nodes.shape[0] + 1,), dtype=np.uint64)
+            nodes_count.scatter_add(node_indexes[row_indexer], 1)
+            nodes_count = nodes_count[:-1]
+
+            cpu_counts = nodes_count.get()
+
+            # remove unused rows from indexer
+            if cpu_counts.sum() < row_indexer.shape[0]:
+                row_indexer = row_indexer[isin(nodes, split_args[1].ravel(), index=row_indexer)]
+
+            # save histogram for the subs trick
+            prev_hist, small_index, big_index = get_prev_hist(cpu_counts,
+                                                              gh_hist, cp.asarray(is_valid_node))
+
+    return nodes
+
+
+class ClusterTreeBuilder:
+    """Tree builder for early stopping clusters"""
+
+    def __init__(self, borders,
+                 **tree_params
+                 ):
+        """
+
+        Args:
+            borders: list of np.ndarray, actual split borders for quantized features
+            **tree_params: other tree building parameters
+        """
+        self.borders = borders
+
+        self.params = {**{
+
+            'max_bin': 256,
+            'max_depth': 6,
+            'min_data_in_leaf': 10,
+            'min_gain_to_split': 0
+
+        }, **tree_params}
+
+    def build_tree(self, X, y):
+        """Build tree
+
+        Args:
+            X: cp.ndarray, quantized feature matrix
+            y: cp.ndarray, loss path matrix
+
+
+        Returns:
+            tree, Tree, constructed tree
+        """
+
+        col_indexer = cp.arange(X.shape[1], dtype=cp.uint64)
+        row_indexer = cp.arange(X.shape[0], dtype=cp.uint64)
+        max_nodes = int((2 ** np.arange(self.params['max_depth'] + 1)).sum())
+        tree = Tree(max_nodes, y.shape[1], 1)
+        # grow single group of the tree and get nodes index
+        cluster_grow_tree(tree, 0, X, y, cp.ones((y.shape[0], 1), dtype=cp.float32),
+                          row_indexer, col_indexer, self.params)
+
+        tree.set_borders(self.borders)
+        tree.set_leaves()
+        tree.set_node_values(np.zeros((max_nodes, 1), dtype=np.float32), np.zeros((1,), dtype=np.uint64))
+
+        return tree
+
+
+class ClusterCandidates(Ensemble):
+    """
+    Ensemble of cluster candidates
+    """
+
+    def __init__(self, depth_range=range(1, 7), min_data_in_leaf=100, debug=False):
+        super().__init__()
+
+        self._debug = debug
+        self.depth_range = depth_range
+        self.min_data_in_leaf = min_data_in_leaf
+        self.max_clust = 2 ** max(depth_range)
+
+    def fit(self, X, y):
+        X, y, sample_weight, eval_sets = validate_input(X, y, None, [])
+        mempool = cp.cuda.MemoryPool()
+        with cp.cuda.using_allocator(allocator=mempool.malloc):
+            # TODO: move quantizer to the Ensemble
+            quantizer = QuantileQuantizer(sample=self.quant_sample, max_bin=self.max_bin)
+            X_enc, max_bin, borders, eval_enc = self.quantize(X, eval_sets)
+
+            self.fit_quantized(X_enc, y, max_bin, borders)
+        mempool.free_all_blocks()
+
+        return self
+
+    def fit_quantized(self, X_enc, y, max_bin, borders):
+        y = cp.array(y, order='C', dtype=cp.float32)
+        X_cp = pad_and_move(X_enc)
+        self.models = []
+
+        for d in self.depth_range:
+            builder = ClusterTreeBuilder(borders, max_depth=d, min_data_in_leaf=self.min_data_in_leaf, max_bin=max_bin)
+
+            tree = builder.build_tree(X_cp, y)
+            tree.reformat(nfeats=X_cp.shape[1], debug=self._debug)
+            self.models.append(tree)
+
+        self.base_score = np.zeros((1,), dtype=np.float32)
+
+        return self
+
+    def predict(self, X, iterations=None, batch_size=100000):
+        return self.predict_leaves(X, iterations=iterations, batch_size=batch_size)[..., 0].T
```

### Comparing `py_boost-0.4.3/py_boost/gpu/base.py` & `py_boost-0.5.0/py_boost/gpu/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,640 +1,669 @@
-"""Abstracts for the tree ensembles"""
-import warnings
-
-try:
-    import cupy as cp
-except Exception:
-    pass
-import numpy as np
-
-from .utils import pinned_array
-from ..quantization.base import QuantileQuantizer, UniformQuantizer, UniquantQuantizer
-
-
-class Ensemble:
-    """
-    Abstract class for tree ensembles.
-    Contains prediction, importance and data transfer methods
-    """
-
-    @staticmethod
-    def _default_postprocess_fn(x):
-        return x
-
-    def __init__(self):
-        """Initialize ensemble"""
-        self.models = None
-        self.nfeats = None
-        self.postprocess_fn = self._default_postprocess_fn
-        self.base_score = None
-        self._on_device = False
-
-        self.quantization = 'Quantile'
-        self.quant_sample = 200000
-        self.max_bin = 256
-        self.min_data_in_bin = 3
-        self.seed = 42
-
-    def to_device(self):
-        """Move trained ensemble data to current GPU device
-
-        Returns:
-
-        """
-        if not self._on_device:
-            for tree in self.models:
-                tree.to_device()
-            self.base_score = cp.asarray(self.base_score)
-
-            self._on_device = True
-
-    def to_cpu(self):
-        """Move trained ensemble data to CPU memory
-
-        Returns:
-
-        """
-        if self._on_device:
-            for tree in self.models:
-                tree.to_cpu()
-            self.base_score = self.base_score.get()
-
-            self._on_device = False
-
-    def __getstate__(self):
-        """Get state dict on CPU for picking
-
-        Returns:
-
-        """
-        self.to_cpu()
-        return self.__dict__
-
-    def quantize(self, X, eval_set):
-        """Fit and quantize all sets
-
-        Args:
-            X: np.ndarray, train features
-            eval_set: list of np.ndarrays, validation features
-
-        Returns:
-
-        """
-        quantizer = self.quantization
-
-        if type(quantizer) is str:
-
-            params = {'sample': self.quant_sample, 'max_bin': self.max_bin, 'min_data_in_bin': self.min_data_in_bin,
-                      'random_state': self.seed}
-
-            if self.quantization == 'Quantile':
-                quantizer = QuantileQuantizer(**params)
-            elif self.quantization == 'Uniform':
-                quantizer = UniformQuantizer(**params)
-            elif self.quantization == 'Uniquant':
-                quantizer = UniquantQuantizer(**params)
-            else:
-                raise ValueError('Unknown quantizer')
-
-        X_enc = quantizer.fit_transform(X)
-        eval_enc = [quantizer.transform(x['X']) for x in eval_set]
-
-        return X_enc, quantizer.get_max_bin(), quantizer.get_borders(), eval_enc
-
-    def _predict_deprecated(self, X, batch_size=100000):
-        """(DEPRECATED) Make prediction for the feature matrix X
-
-        Args:
-            X: 2d np.ndarray of features
-            batch_size: int, inner batch splitting size to avoid OOM
-
-        Returns:
-            prediction, 2d np.ndarray of float32, shape (n_data, n_outputs)
-        """
-        self.to_device()
-        prediction = pinned_array(np.empty((X.shape[0], self.base_score.shape[0]), dtype=np.float32))
-
-        n_streams = 2
-        map_streams = [cp.cuda.Stream(non_blocking=False) for _ in range(n_streams)]
-
-        stop_events = []
-
-        for k, i in enumerate(range(0, X.shape[0], batch_size)):
-            with map_streams[k % n_streams] as st:
-                x_batch = X[i: i + batch_size].astype(np.float32)
-                gpu_batch = cp.empty(x_batch.shape, x_batch.dtype)
-                x_batch = pinned_array(x_batch)
-                gpu_batch.set(x_batch, stream=st)
-
-                result = cp.zeros((x_batch.shape[0], self.base_score.shape[0]), dtype=np.float32)
-                result[:] = self.base_score
-                for n, tree in enumerate(self.models):
-                    result += tree._predict_deprecated(gpu_batch)
-
-                self.postprocess_fn(result).get(stream=st, out=prediction[i: i + x_batch.shape[0]])
-
-                stop_event = st.record()
-                stop_events.append(stop_event)
-
-        curr_stream = cp.cuda.get_current_stream()
-        for stop_event in stop_events:
-            curr_stream.wait_event(stop_event)
-        curr_stream.synchronize()
-        return prediction
-
-    def _predict_leaves_deprecated(self, X, iterations=None, batch_size=100000):
-        """(DEPRECATED) Predict tree leaf indices for the feature matrix X
-
-        Args:
-            X: 2d np.ndarray of features
-            iterations: list of int or None. If list of ints is passed, prediction will be made only
-            for given iterations, otherwise - for all iterations
-            batch_size: int, inner batch splitting size to avoid OOM
-
-        Returns:
-            prediction, 2d np.ndarray of uint32, shape (n_iterations, n_data, n_groups).
-            For n_groups explanation check Tree class
-        """
-        if iterations is None:
-            iterations = list(range(len(self.models)))
-
-        self.to_device()
-
-        check_grp = np.unique([x.ngroups for x in self.models])
-        if check_grp.shape[0] > 1:
-            raise ValueError('Different number of groups in trees')
-
-        ngroups = check_grp[0]
-        leaves = pinned_array(np.empty((len(iterations), X.shape[0], ngroups), dtype=np.int32))
-
-        map_streams = [cp.cuda.Stream(non_blocking=False) for _ in range(2)]
-
-        stop_events = []
-
-        for k, i in enumerate(range(0, X.shape[0], batch_size)):
-            with map_streams[k % 2] as st:
-                x_batch = X[i: i + batch_size].astype(np.float32)
-                gpu_batch = cp.empty(x_batch.shape, x_batch.dtype)
-                x_batch = pinned_array(x_batch)
-                gpu_batch.set(x_batch, stream=st)
-
-                for j, n in enumerate(iterations):
-                    self.models[n]._predict_leaf_deprecated(gpu_batch).get(stream=st, out=leaves[j, i: i + x_batch.shape[0]])
-
-                stop_event = st.record()
-                stop_events.append(stop_event)
-
-        curr_stream = cp.cuda.get_current_stream()
-        for stop_event in stop_events:
-            curr_stream.wait_event(stop_event)
-        curr_stream.synchronize()
-        return leaves
-
-    def _predict_staged_deprecated(self, X, iterations=None, batch_size=100000):
-        """(DEPRECATED) Make prediction from different stages for the feature matrix X
-
-        Args:
-            X: 2d np.ndarray of features
-            iterations: list of int or None. If list of ints is passed, prediction will be made only
-            for given iterations, otherwise - for all iterations
-            batch_size: int, inner batch splitting size to avoid OOM
-
-        Returns:
-            prediction, 2d np.ndarray of float32, shape (n_iterations, n_data, n_out)
-        """
-
-        # Iteration list validation
-        if iterations is None:
-            iterations = list(range(len(self.models)))
-            
-        self.to_device()
-        prediction = pinned_array(np.empty((len(iterations), X.shape[0], self.base_score.shape[0]), dtype=np.float32))
-
-        map_streams = [cp.cuda.Stream(non_blocking=False) for _ in range(2)]
-
-        stop_events = []
-
-        for k, i in enumerate(range(0, X.shape[0], batch_size)):
-            with map_streams[k % 2] as st:
-                x_batch = X[i: i + batch_size].astype(np.float32)
-                gpu_batch = cp.empty(x_batch.shape, x_batch.dtype)
-                x_batch = pinned_array(x_batch)
-                gpu_batch.set(x_batch, stream=st)
-
-                result = cp.zeros((x_batch.shape[0], self.base_score.shape[0]), dtype=np.float32)
-                result[:] = self.base_score
-
-                next_out = 0
-                for n, tree in enumerate(self.models):
-                    result += tree._predict_deprecated(gpu_batch)
-                    if n == iterations[next_out]:
-                        self.postprocess_fn(result).get(
-                            stream=st, out=prediction[next_out, i: i + x_batch.shape[0]]
-                        )
-
-                        next_out += 1
-                        if next_out >= len(iterations):
-                            break
-
-                stop_event = st.record()
-                stop_events.append(stop_event)
-
-        curr_stream = cp.cuda.get_current_stream()
-        for stop_event in stop_events:
-            curr_stream.wait_event(stop_event)
-        curr_stream.synchronize()
-        return prediction
-
-    def _get_feature_importance_deprecated(self, imp_type='split'):
-        """(DEPRECATED) Get feature importance
-
-        Args:
-            imp_type: str, importance type, 'split' or 'gain'
-
-        Returns:
-
-        """
-        self.to_cpu()
-
-        assert imp_type in ['gain', 'split'], "Importance type should be 'gain' or 'split'"
-        importance = np.zeros(self.nfeats, dtype=np.float32)
-
-        for tree in self.models:
-            sl = tree.feats >= 0
-            acc_val = 1 if imp_type == 'split' else tree.gains[sl]
-            np.add.at(importance, tree.feats[sl], acc_val)
-
-        return importance
-
-    def get_feature_importance(self, imp_type='split'):
-        """Get feature importance
-
-        Args:
-            imp_type: str, importance type, 'split' or 'gain'
-
-        Returns:
-            importance: np.ndarray 1d of float32, shape (n_features)
-        """
-        assert imp_type in ['gain', 'split'], "Importance type should be 'gain' or 'split'"
-            
-        importance = np.zeros(self.nfeats, dtype=np.float32)
-
-        for tree in self.models:
-            if imp_type == 'split':
-                if type(tree.feature_importance_split) is not np.ndarray:
-                    importance += tree.feature_importance_split.get()
-                else:
-                    importance += tree.feature_importance_split
-            else:
-                if type(tree.feature_importance_gain) is not np.ndarray:
-                    importance += tree.feature_importance_gain.get()
-                else:
-                    importance += tree.feature_importance_gain
-
-        return importance
-
-    def predict_leaves(self, X, iterations=None, batch_size=100_000):
-        """Predict tree leaf indices for the feature matrix X
-
-        Args:
-            X: 2d np.ndarray of float32, array of features
-            iterations: list of int or None. If list of ints is passed, prediction will be made only
-                for given iterations, otherwise - for all iterations
-            batch_size: int, inner batch splitting size to avoid OOM
-
-        Returns:
-            prediction, np.ndarray 2d of int32, shape (n_iterations, n_data, n_groups).
-            For n_groups explanation check Tree class
-        """
-        assert batch_size > 0, 'Batch size must be a positive integer'
-        
-        if iterations is None:
-            iterations = np.arange(len(self.models))
-        else:
-            iterations = np.array(iterations, dtype=np.int64)
-            
-        assert len(iterations) > 0, 'Iterations are empty sequence'
-        assert (max(iterations) < len(self.models)) and (min(iterations) >= 0), 'Invalid stage numbers'
-        assert len(np.unique(iterations)) == len(iterations), 'Duplicate values in stages are not allowed'
-
-        check_grp = np.unique([x.ngroups for x in self.models])
-        assert len(check_grp) == 1, 'Different number of groups in trees'
-        
-        ngroups = check_grp[0]
-
-        self.to_device()
-        # special case handle, if X is already on device or size of X <= batch_size
-        if type(X) is cp.ndarray or X.shape[0] <= batch_size:
-            is_on_gpu = True
-            if type(X) is not cp.ndarray:
-                is_on_gpu = False
-                X = cp.array(X, order='C', dtype=cp.float32)
-            if not (X.flags['C_CONTIGUOUS'] or X.flags['F_CONTIGUOUS']):
-                warnings.warn("X is not 'C_CONTIGUOUS' or 'F_CONTIGUOUS', contiguous copy of array will be created."
-                              "To reduce inference time, make sure X is contiguous beforehand")
-                X = cp.ascontiguousarray(X)
-            gpu_pred = cp.empty((len(iterations), X.shape[0], ngroups), dtype=np.int32)
-
-            for j, n in enumerate(iterations):
-                self.models[n].predict_leaf(X, gpu_pred[j])
-
-            cp.cuda.get_current_stream().synchronize()
-            if is_on_gpu:
-                return gpu_pred
-            return gpu_pred.get()
-
-        n_streams = 2  # don't change
-        map_streams = [cp.cuda.Stream() for _ in range(n_streams)]
-
-        # result allocation
-        cpu_leaves_full = np.empty((len(iterations), X.shape[0], ngroups), dtype=np.int32)
-        cpu_leaves = [pinned_array(np.empty((len(iterations), batch_size, ngroups), dtype=np.int32)) for _ in range(n_streams)]
-        gpu_leaves = [cp.empty((len(iterations), batch_size, ngroups), dtype=cp.int32) for _ in range(n_streams)]
-
-        # batch allocation
-        cpu_batch = [pinned_array(np.empty(X[0:batch_size].shape, dtype=np.float32)) for _ in range(n_streams)]
-        gpu_batch = [cp.empty(X[0:batch_size].shape, dtype=cp.float32) for _ in range(n_streams)]
-
-        cpu_batch_free_event = [None, None]
-        gpu_batch_free_event = [None, None]
-        cpu_out_ready_event = [None, None]
-        last_batch_size = 0
-        last_n_stream = 0
-        for k, i in enumerate(range(0, X.shape[0], batch_size)):
-            nst = k % n_streams
-            with map_streams[nst] as stream:
-                real_batch_len = batch_size if i + batch_size <= X.shape[0] else X.shape[0] - i
-
-                # if cpu_batch is available, copy X batch to pinned memory on H
-                if k >= 2:
-                    cpu_batch_free_event[nst].synchronize()
-                cpu_batch[nst][:real_batch_len] = X[i:i + real_batch_len].astype(np.float32)
-
-                # copy X batch from pinned memory to D
-                if k >= 2:
-                    gpu_batch_free_event[nst].synchronize()
-                gpu_batch[nst][:real_batch_len].set(cpu_batch[nst][:real_batch_len])
-                cpu_batch_free_event[nst] = stream.record(cp.cuda.Event(block=True))
-
-                # when gpu_leaves is available and cpu_out is ready, proceed to the prediction
-                if k >= 2:
-                    cpu_out_ready_event[nst].synchronize()
-                for j, n in enumerate(iterations):
-                    self.models[n].predict_leaf(gpu_batch[nst][:real_batch_len], gpu_leaves[nst][j][:real_batch_len])
-                gpu_batch_free_event[nst] = stream.record(cp.cuda.Event(block=True))
-
-                # copy prediction from pinned memory to pageable memory on H (from previous iteration)
-                if k >= 2:
-                    for j, n in enumerate(iterations):
-                        cpu_leaves_full[j][i - 2 * batch_size: i - batch_size] = cpu_leaves[nst][j][:batch_size]
-
-                # copy predictions from device to pinned memory on H
-                gpu_leaves[nst][:real_batch_len].get(out=cpu_leaves[nst][:real_batch_len])
-                cpu_out_ready_event[nst] = stream.record(cp.cuda.Event(block=True))
-
-                last_batch_size = real_batch_len
-                last_n_stream = nst
-
-        with map_streams[1 - last_n_stream]:
-            cpu_out_ready_event[1 - last_n_stream].synchronize()
-            for j, n in enumerate(iterations):
-                cpu_leaves_full[j][X.shape[0] - (batch_size + last_batch_size): X.shape[0] - last_batch_size] = \
-                    cpu_leaves[1 - last_n_stream][j][:batch_size]
-        with map_streams[last_n_stream]:
-            cpu_out_ready_event[last_n_stream].synchronize()
-            for j, n in enumerate(iterations):
-                cpu_leaves_full[j][X.shape[0] - last_batch_size:] = cpu_leaves[last_n_stream][j][:last_batch_size]
-
-        return cpu_leaves_full
-
-    def predict(self, X, batch_size=100_000):
-        """Make prediction for the feature matrix X
-
-        Args:
-            X: np.ndarray 2d of float32, array of features
-            batch_size: int, inner batch splitting size to avoid OOM
-
-        Returns:
-            prediction: np.ndarray 2d of float32, shape (n_data, n_outputs)
-        """
-        assert batch_size > 0, 'Batch size must be a positive integer'
-        
-        ngroups = max((x.ngroups for x in self.models))
-        n_out = self.base_score.shape[0]
-
-        self.to_device()
-        # special case handle, if X is already on device or size of X <= batch_size
-        if type(X) is cp.ndarray or X.shape[0] <= batch_size:
-            is_on_gpu = True
-            if type(X) is not cp.ndarray:
-                is_on_gpu = False
-                X = cp.array(X, order='C', dtype=cp.float32)
-            if not(X.flags['C_CONTIGUOUS'] or X.flags['F_CONTIGUOUS']):
-                warnings.warn("X is not 'C_CONTIGUOUS' or 'F_CONTIGUOUS', contiguous copy of array will be created."
-                              "To reduce inference time, make sure X is contiguous beforehand")
-                X = cp.ascontiguousarray(X)
-
-            gpu_pred = cp.empty((X.shape[0], n_out), dtype=cp.float32)
-            gpu_pred_leaves = cp.empty((X.shape[0], ngroups), dtype=cp.int32)
-
-            gpu_pred[:] = self.base_score
-
-            for tree in self.models:
-                tree.predict(X, gpu_pred, gpu_pred_leaves)
-
-            cp.cuda.get_current_stream().synchronize()
-            pred = self.postprocess_fn(gpu_pred)
-            if is_on_gpu:
-                return pred
-            return pred.get()
-
-        # cuda stream allocation
-        n_streams = 2  # don't change
-        map_streams = [cp.cuda.Stream() for _ in range(n_streams)]
-
-        # result allocation
-        cpu_pred_full = np.empty((X.shape[0], n_out), dtype=np.float32)
-        cpu_pred = [pinned_array(np.empty((batch_size, n_out), dtype=np.float32)) for _ in range(n_streams)]
-        gpu_pred = [cp.empty((batch_size, n_out), dtype=cp.float32) for _ in range(n_streams)]
-
-        # temp buffer for leaves
-        gpu_pred_leaves = [cp.empty((batch_size, ngroups), dtype=cp.int32) for _ in range(n_streams)]
-
-        # batch allocation
-        cpu_batch = [pinned_array(np.empty(X[0:batch_size].shape, dtype=np.float32)) for _ in range(n_streams)]
-        gpu_batch = [cp.empty(X[0:batch_size].shape, dtype=cp.float32) for _ in range(n_streams)]
-
-        cpu_batch_free_event = [None, None]
-        gpu_batch_free_event = [None, None]
-        cpu_out_ready_event = [None, None]
-        last_batch_size = 0
-        last_n_stream = 0
-        for k, i in enumerate(range(0, X.shape[0], batch_size)):
-            nst = k % n_streams
-            with map_streams[nst] as stream:
-                real_batch_len = batch_size if i + batch_size <= X.shape[0] else X.shape[0] - i
-
-                # if cpu_batch is available, copy X batch to pinned memory on H
-                if k >= 2:
-                    cpu_batch_free_event[nst].synchronize()
-                cpu_batch[nst][:real_batch_len] = X[i:i + real_batch_len].astype(cp.float32)
-
-                # copy X batch from pinned memory to D
-                if k >= 2:
-                    gpu_batch_free_event[nst].synchronize()
-                gpu_batch[nst][:real_batch_len].set(cpu_batch[nst][:real_batch_len])
-                cpu_batch_free_event[nst] = stream.record(cp.cuda.Event(block=True))
-
-                # when gpu_pred is available and cpu_out is ready, proceed to the prediction
-                if k >= 2:
-                    cpu_out_ready_event[nst].synchronize()
-                gpu_pred[nst][:] = self.base_score
-                for tree in self.models:
-                    tree.predict(gpu_batch[nst][:real_batch_len], gpu_pred[nst][:real_batch_len],
-                                 gpu_pred_leaves[nst][:real_batch_len])
-                gpu_batch_free_event[nst] = stream.record(cp.cuda.Event(block=True))
-
-                # copy prediction from pinned memory to pageable memory on H (from previous iteration)
-                if k >= 2:
-                    cpu_pred_full[i - 2 * batch_size: i - batch_size] = cpu_pred[nst][:batch_size]
-
-                # copy predictions from device to pinned memory on H
-                self.postprocess_fn(gpu_pred[nst][:real_batch_len]).get(out=cpu_pred[nst][:real_batch_len])
-                cpu_out_ready_event[nst] = stream.record(cp.cuda.Event(block=True))
-
-                last_batch_size = real_batch_len
-                last_n_stream = nst
-
-        # waiting for sync of last two batches
-        with map_streams[1 - last_n_stream]:
-            cpu_out_ready_event[1 - last_n_stream].synchronize()
-            cpu_pred_full[X.shape[0] - (batch_size + last_batch_size): X.shape[0] - last_batch_size] = \
-                cpu_pred[1 - last_n_stream][:batch_size]
-        with map_streams[last_n_stream]:
-            cpu_out_ready_event[last_n_stream].synchronize()
-            cpu_pred_full[X.shape[0] - last_batch_size:] = cpu_pred[last_n_stream][:last_batch_size]
-
-        return cpu_pred_full
-
-    def predict_staged(self, X, iterations=None, batch_size=100_000):
-        """Make prediction from different stages for the feature matrix X
-
-        Args:
-            X: 2d np.ndarray of float32, array of features
-            iterations: list of int or None. If list of ints is passed, prediction will be made only
-                for given iterations, otherwise - for all iterations
-            batch_size: int, inner batch splitting size to avoid OOM
-
-        Returns:
-            prediction, np.ndarray 2d of float32, shape (n_iterations, n_data, n_out)
-        """
-        assert batch_size > 0, 'Batch size must be a positive integer'
-        
-        if iterations is None:
-            iterations = np.arange(len(self.models))
-        else:
-            iterations = np.array(iterations, dtype=np.int64)
-            
-        assert len(iterations) > 0, 'Iterations are empty sequence'
-        assert (max(iterations) < len(self.models)) and (min(iterations) >= 0), 'Invalid stage numbers'
-        assert len(np.unique(iterations)) == len(iterations), 'Duplicate values in stages are not allowed'
-        
-        ngroups = max((x.ngroups for x in self.models))
-        n_out = self.base_score.shape[0]
-
-        self.to_device()
-        # special case handle, if X is already on device or size of X <= batch_size
-        if type(X) is cp.ndarray or X.shape[0] <= batch_size:
-            is_on_gpu = True
-            if type(X) is not cp.ndarray:
-                is_on_gpu = False
-                X = cp.array(X, order='C', dtype=cp.float32)
-                pred_full = np.empty((len(iterations), X.shape[0], n_out), dtype=cp.float32)
-            else:
-                pred_full = cp.empty((len(iterations), X.shape[0], n_out), dtype=cp.float32)
-            if not (X.flags['C_CONTIGUOUS'] or X.flags['F_CONTIGUOUS']):
-                warnings.warn("X is not 'C_CONTIGUOUS' or 'F_CONTIGUOUS', contiguous copy of array will be created."
-                              "To reduce inference time, make sure X is contiguous beforehand")
-                X = cp.ascontiguousarray(X)
-
-            gpu_pred = cp.empty((X.shape[0], n_out), dtype=cp.float32)
-            gpu_pred_leaves = cp.empty((X.shape[0], ngroups), dtype=cp.int32)
-
-            gpu_pred[:] = self.base_score
-            next_out = 0
-            for n, tree in enumerate(self.models):
-                tree.predict(X, gpu_pred, gpu_pred_leaves)
-                if n == iterations[next_out]:
-                    if is_on_gpu:
-                        pred_full[next_out] = self.postprocess_fn(gpu_pred)
-                    else:
-                        self.postprocess_fn(gpu_pred).get(out=pred_full[next_out])
-                    next_out += 1
-                    if next_out >= len(iterations):
-                        cp.cuda.get_current_stream().synchronize()
-                        return pred_full
-
-        n_streams = 2  # don't change
-        map_streams = [cp.cuda.Stream() for _ in range(n_streams)]
-
-        # result allocation
-        cpu_pred_full = np.empty((len(iterations), X.shape[0], n_out), dtype=np.float32)
-        cpu_pred = [pinned_array(np.empty((len(iterations), batch_size, n_out), dtype=np.float32)) for _ in range(n_streams)]
-        gpu_pred = [cp.empty((batch_size, n_out), dtype=cp.float32) for _ in range(n_streams)]
-
-        # temp buffer for leaves
-        gpu_pred_leaves = [cp.empty((batch_size, ngroups), dtype=cp.int32) for _ in range(n_streams)]
-
-        # batch allocation
-        cpu_batch = [pinned_array(np.empty(X[0:batch_size].shape, dtype=np.float32)) for _ in range(n_streams)]
-        gpu_batch = [cp.empty(X[0:batch_size].shape, dtype=np.float32) for _ in range(n_streams)]
-
-        cpu_batch_free_event = [None, None]
-        cpu_out_ready_event = [None, None]
-        last_batch_size = 0
-        last_n_stream = 0
-        for k, i in enumerate(range(0, X.shape[0], batch_size)):
-            nst = k % n_streams
-            with map_streams[nst] as stream:
-                real_batch_len = batch_size if i + batch_size <= X.shape[0] else X.shape[0] - i
-
-                # if cpu_batch is available, copy X batch to pinned memory on H
-                if k >= 2:
-                    cpu_batch_free_event[nst].synchronize()
-                cpu_batch[nst][:real_batch_len] = X[i:i + real_batch_len].astype(np.float32)
-
-                # copy X batch from pinned memory to D
-                if k >= 2:
-                    cpu_out_ready_event[nst].synchronize()
-                gpu_batch[nst][:real_batch_len].set(cpu_batch[nst][:real_batch_len])
-                cpu_batch_free_event[nst] = stream.record(cp.cuda.Event(block=True))
-                gpu_pred[nst][:] = self.base_score
-
-                # copy prediction from pinned memory to pageable memory on H (from previous iteration)
-                if k >= 2:
-                    cpu_pred_full[:, i - 2 * batch_size: i - batch_size] = cpu_pred[nst][:, :batch_size]
-
-                i_next = 0
-                for i_tree, tree in enumerate(self.models):
-                    tree.predict(gpu_batch[nst][:real_batch_len], gpu_pred[nst][:real_batch_len],
-                                 gpu_pred_leaves[nst][:real_batch_len])
-                    if iterations[i_next] == i_tree:
-                        self.postprocess_fn(gpu_pred[nst][:real_batch_len]).get(out=cpu_pred[nst][i_next][:real_batch_len])
-                        i_next += 1
-                        if i_next >= len(iterations):
-                            break
-                cpu_out_ready_event[nst] = stream.record(cp.cuda.Event(block=True))
-
-                last_batch_size = real_batch_len
-                last_n_stream = nst
-
-        # waiting for sync of last two batches
-        with map_streams[1 - last_n_stream]:
-            cpu_out_ready_event[1 - last_n_stream].synchronize()
-            cpu_pred_full[:, X.shape[0] - (batch_size + last_batch_size): X.shape[0] - last_batch_size] =\
-                cpu_pred[1 - last_n_stream][:, :batch_size]
-        with map_streams[last_n_stream]:
-            cpu_out_ready_event[last_n_stream].synchronize()
-            cpu_pred_full[:, X.shape[0] - last_batch_size:] = cpu_pred[last_n_stream][:, :last_batch_size]
-
-        return cpu_pred_full
+"""Abstracts for the tree ensembles"""
+import warnings
+
+try:
+    import cupy as cp
+except Exception:
+    pass
+import numpy as np
+
+from .serialization import dump, load
+from .utils import pinned_array
+from ..quantization.base import QuantileQuantizer, UniformQuantizer, UniquantQuantizer
+
+
+class Ensemble:
+    """
+    Abstract class for tree ensembles.
+    Contains prediction, importance and data transfer methods
+    """
+
+    @staticmethod
+    def _default_postprocess_fn(x):
+        return x
+
+    def __init__(self):
+        """Initialize ensemble"""
+        self.models = None
+        self.nfeats = None
+        self.postprocess_fn = self._default_postprocess_fn
+        self.base_score = None
+        self._on_device = False
+
+        self.quantization = 'Quantile'
+        self.quant_sample = 200000
+        self.max_bin = 256
+        self.min_data_in_bin = 3
+        self.seed = 42
+
+    def to_device(self):
+        """Move trained ensemble data to current GPU device
+
+        Returns:
+
+        """
+        if not self._on_device:
+            for tree in self.models:
+                tree.to_device()
+            self.base_score = cp.asarray(self.base_score)
+
+            self._on_device = True
+
+    def to_cpu(self):
+        """Move trained ensemble data to CPU memory
+
+        Returns:
+
+        """
+        if self._on_device:
+            for tree in self.models:
+                tree.to_cpu()
+            self.base_score = self.base_score.get()
+
+            self._on_device = False
+
+    def __getstate__(self):
+        """Get state dict on CPU for picking
+
+        Returns:
+
+        """
+        self.to_cpu()
+        return self.__dict__
+
+    def quantize(self, X, eval_set):
+        """Fit and quantize all sets
+
+        Args:
+            X: np.ndarray, train features
+            eval_set: list of np.ndarrays, validation features
+
+        Returns:
+
+        """
+        quantizer = self.quantization
+
+        if type(quantizer) is str:
+
+            params = {'sample': self.quant_sample, 'max_bin': self.max_bin, 'min_data_in_bin': self.min_data_in_bin,
+                      'random_state': self.seed}
+
+            if self.quantization == 'Quantile':
+                quantizer = QuantileQuantizer(**params)
+            elif self.quantization == 'Uniform':
+                quantizer = UniformQuantizer(**params)
+            elif self.quantization == 'Uniquant':
+                quantizer = UniquantQuantizer(**params)
+            else:
+                raise ValueError('Unknown quantizer')
+
+        X_enc = quantizer.fit_transform(X)
+        eval_enc = [quantizer.transform(x['X']) for x in eval_set]
+
+        return X_enc, quantizer.get_max_bin(), quantizer.get_borders(), eval_enc
+
+    def _predict_deprecated(self, X, batch_size=100000):
+        """(DEPRECATED) Make prediction for the feature matrix X
+
+        Args:
+            X: 2d np.ndarray of features
+            batch_size: int, inner batch splitting size to avoid OOM
+
+        Returns:
+            prediction, 2d np.ndarray of float32, shape (n_data, n_outputs)
+        """
+        self.to_device()
+        prediction = pinned_array(np.empty((X.shape[0], self.base_score.shape[0]), dtype=np.float32))
+
+        n_streams = 2
+        map_streams = [cp.cuda.Stream(non_blocking=False) for _ in range(n_streams)]
+
+        stop_events = []
+
+        for k, i in enumerate(range(0, X.shape[0], batch_size)):
+            with map_streams[k % n_streams] as st:
+                x_batch = X[i: i + batch_size].astype(np.float32)
+                gpu_batch = cp.empty(x_batch.shape, x_batch.dtype)
+                x_batch = pinned_array(x_batch)
+                gpu_batch.set(x_batch, stream=st)
+
+                result = cp.zeros((x_batch.shape[0], self.base_score.shape[0]), dtype=np.float32)
+                result[:] = self.base_score
+                for n, tree in enumerate(self.models):
+                    result += tree._predict_deprecated(gpu_batch)
+
+                self.postprocess_fn(result).get(stream=st, out=prediction[i: i + x_batch.shape[0]])
+
+                stop_event = st.record()
+                stop_events.append(stop_event)
+
+        curr_stream = cp.cuda.get_current_stream()
+        for stop_event in stop_events:
+            curr_stream.wait_event(stop_event)
+        curr_stream.synchronize()
+        return prediction
+
+    def _predict_leaves_deprecated(self, X, iterations=None, batch_size=100000):
+        """(DEPRECATED) Predict tree leaf indices for the feature matrix X
+
+        Args:
+            X: 2d np.ndarray of features
+            iterations: list of int or None. If list of ints is passed, prediction will be made only
+            for given iterations, otherwise - for all iterations
+            batch_size: int, inner batch splitting size to avoid OOM
+
+        Returns:
+            prediction, 2d np.ndarray of uint32, shape (n_iterations, n_data, n_groups).
+            For n_groups explanation check Tree class
+        """
+        if iterations is None:
+            iterations = list(range(len(self.models)))
+
+        self.to_device()
+
+        check_grp = np.unique([x.ngroups for x in self.models])
+        if check_grp.shape[0] > 1:
+            raise ValueError('Different number of groups in trees')
+
+        ngroups = check_grp[0]
+        leaves = pinned_array(np.empty((len(iterations), X.shape[0], ngroups), dtype=np.int32))
+
+        map_streams = [cp.cuda.Stream(non_blocking=False) for _ in range(2)]
+
+        stop_events = []
+
+        for k, i in enumerate(range(0, X.shape[0], batch_size)):
+            with map_streams[k % 2] as st:
+                x_batch = X[i: i + batch_size].astype(np.float32)
+                gpu_batch = cp.empty(x_batch.shape, x_batch.dtype)
+                x_batch = pinned_array(x_batch)
+                gpu_batch.set(x_batch, stream=st)
+
+                for j, n in enumerate(iterations):
+                    self.models[n]._predict_leaf_deprecated(gpu_batch).get(stream=st,
+                                                                           out=leaves[j, i: i + x_batch.shape[0]])
+
+                stop_event = st.record()
+                stop_events.append(stop_event)
+
+        curr_stream = cp.cuda.get_current_stream()
+        for stop_event in stop_events:
+            curr_stream.wait_event(stop_event)
+        curr_stream.synchronize()
+        return leaves
+
+    def _predict_staged_deprecated(self, X, iterations=None, batch_size=100000):
+        """(DEPRECATED) Make prediction from different stages for the feature matrix X
+
+        Args:
+            X: 2d np.ndarray of features
+            iterations: list of int or None. If list of ints is passed, prediction will be made only
+            for given iterations, otherwise - for all iterations
+            batch_size: int, inner batch splitting size to avoid OOM
+
+        Returns:
+            prediction, 2d np.ndarray of float32, shape (n_iterations, n_data, n_out)
+        """
+
+        # Iteration list validation
+        if iterations is None:
+            iterations = list(range(len(self.models)))
+
+        self.to_device()
+        prediction = pinned_array(np.empty((len(iterations), X.shape[0], self.base_score.shape[0]), dtype=np.float32))
+
+        map_streams = [cp.cuda.Stream(non_blocking=False) for _ in range(2)]
+
+        stop_events = []
+
+        for k, i in enumerate(range(0, X.shape[0], batch_size)):
+            with map_streams[k % 2] as st:
+                x_batch = X[i: i + batch_size].astype(np.float32)
+                gpu_batch = cp.empty(x_batch.shape, x_batch.dtype)
+                x_batch = pinned_array(x_batch)
+                gpu_batch.set(x_batch, stream=st)
+
+                result = cp.zeros((x_batch.shape[0], self.base_score.shape[0]), dtype=np.float32)
+                result[:] = self.base_score
+
+                next_out = 0
+                for n, tree in enumerate(self.models):
+                    result += tree._predict_deprecated(gpu_batch)
+                    if n == iterations[next_out]:
+                        self.postprocess_fn(result).get(
+                            stream=st, out=prediction[next_out, i: i + x_batch.shape[0]]
+                        )
+
+                        next_out += 1
+                        if next_out >= len(iterations):
+                            break
+
+                stop_event = st.record()
+                stop_events.append(stop_event)
+
+        curr_stream = cp.cuda.get_current_stream()
+        for stop_event in stop_events:
+            curr_stream.wait_event(stop_event)
+        curr_stream.synchronize()
+        return prediction
+
+    def _get_feature_importance_deprecated(self, imp_type='split'):
+        """(DEPRECATED) Get feature importance
+
+        Args:
+            imp_type: str, importance type, 'split' or 'gain'
+
+        Returns:
+
+        """
+        self.to_cpu()
+
+        assert imp_type in ['gain', 'split'], "Importance type should be 'gain' or 'split'"
+        importance = np.zeros(self.nfeats, dtype=np.float32)
+
+        for tree in self.models:
+            sl = tree.feats >= 0
+            acc_val = 1 if imp_type == 'split' else tree.gains[sl]
+            np.add.at(importance, tree.feats[sl], acc_val)
+
+        return importance
+
+    def get_feature_importance(self, imp_type='split'):
+        """Get feature importance
+
+        Args:
+            imp_type: str, importance type, 'split' or 'gain'
+
+        Returns:
+            importance: np.ndarray 1d of float32, shape (n_features)
+        """
+        assert imp_type in ['gain', 'split'], "Importance type should be 'gain' or 'split'"
+
+        importance = np.zeros(self.nfeats, dtype=np.float32)
+
+        for tree in self.models:
+            if imp_type == 'split':
+                if type(tree.feature_importance_split) is not np.ndarray:
+                    importance += tree.feature_importance_split.get()
+                else:
+                    importance += tree.feature_importance_split
+            else:
+                if type(tree.feature_importance_gain) is not np.ndarray:
+                    importance += tree.feature_importance_gain.get()
+                else:
+                    importance += tree.feature_importance_gain
+
+        return importance
+
+    def predict_leaves(self, X, iterations=None, batch_size=100_000):
+        """Predict tree leaf indices for the feature matrix X
+
+        Args:
+            X: 2d np.ndarray of float32, array of features
+            iterations: list of int or None. If list of ints is passed, prediction will be made only
+                for given iterations, otherwise - for all iterations
+            batch_size: int, inner batch splitting size to avoid OOM
+
+        Returns:
+            prediction, np.ndarray 2d of int32, shape (n_iterations, n_data, n_groups).
+            For n_groups explanation check Tree class
+        """
+        assert batch_size > 0, 'Batch size must be a positive integer'
+
+        if iterations is None:
+            iterations = np.arange(len(self.models))
+        else:
+            iterations = np.array(iterations, dtype=np.int64)
+
+        assert len(iterations) > 0, 'Iterations are empty sequence'
+        assert (max(iterations) < len(self.models)) and (min(iterations) >= 0), 'Invalid stage numbers'
+        assert len(np.unique(iterations)) == len(iterations), 'Duplicate values in stages are not allowed'
+
+        check_grp = np.unique([x.ngroups for x in self.models])
+        assert len(check_grp) == 1, 'Different number of groups in trees'
+
+        ngroups = check_grp[0]
+
+        self.to_device()
+        # special case handle, if X is already on device or size of X <= batch_size
+        if type(X) is cp.ndarray or X.shape[0] <= batch_size:
+            is_on_gpu = True
+            if type(X) is not cp.ndarray:
+                is_on_gpu = False
+                X = cp.array(X, order='C', dtype=cp.float32)
+            if not (X.flags['C_CONTIGUOUS'] or X.flags['F_CONTIGUOUS']):
+                warnings.warn("X is not 'C_CONTIGUOUS' or 'F_CONTIGUOUS', contiguous copy of array will be created."
+                              "To reduce inference time, make sure X is contiguous beforehand")
+                X = cp.ascontiguousarray(X)
+            gpu_pred = cp.empty((len(iterations), X.shape[0], ngroups), dtype=np.int32)
+
+            for j, n in enumerate(iterations):
+                self.models[n].predict_leaf(X, gpu_pred[j])
+
+            cp.cuda.get_current_stream().synchronize()
+            if is_on_gpu:
+                return gpu_pred
+            return gpu_pred.get()
+
+        n_streams = 2  # don't change
+        map_streams = [cp.cuda.Stream() for _ in range(n_streams)]
+
+        # result allocation
+        cpu_leaves_full = np.empty((len(iterations), X.shape[0], ngroups), dtype=np.int32)
+        cpu_leaves = [pinned_array(np.empty((len(iterations), batch_size, ngroups), dtype=np.int32)) for _ in
+                      range(n_streams)]
+        gpu_leaves = [cp.empty((len(iterations), batch_size, ngroups), dtype=cp.int32) for _ in range(n_streams)]
+
+        # batch allocation
+        cpu_batch = [pinned_array(np.empty(X[0:batch_size].shape, dtype=np.float32)) for _ in range(n_streams)]
+        gpu_batch = [cp.empty(X[0:batch_size].shape, dtype=cp.float32) for _ in range(n_streams)]
+
+        cpu_batch_free_event = [None, None]
+        gpu_batch_free_event = [None, None]
+        cpu_out_ready_event = [None, None]
+        last_batch_size = 0
+        last_n_stream = 0
+        for k, i in enumerate(range(0, X.shape[0], batch_size)):
+            nst = k % n_streams
+            with map_streams[nst] as stream:
+                real_batch_len = batch_size if i + batch_size <= X.shape[0] else X.shape[0] - i
+
+                # if cpu_batch is available, copy X batch to pinned memory on H
+                if k >= 2:
+                    cpu_batch_free_event[nst].synchronize()
+                cpu_batch[nst][:real_batch_len] = X[i:i + real_batch_len].astype(np.float32)
+
+                # copy X batch from pinned memory to D
+                if k >= 2:
+                    gpu_batch_free_event[nst].synchronize()
+                gpu_batch[nst][:real_batch_len].set(cpu_batch[nst][:real_batch_len])
+                cpu_batch_free_event[nst] = stream.record(cp.cuda.Event(block=True))
+
+                # when gpu_leaves is available and cpu_out is ready, proceed to the prediction
+                if k >= 2:
+                    cpu_out_ready_event[nst].synchronize()
+                for j, n in enumerate(iterations):
+                    self.models[n].predict_leaf(gpu_batch[nst][:real_batch_len], gpu_leaves[nst][j][:real_batch_len])
+                gpu_batch_free_event[nst] = stream.record(cp.cuda.Event(block=True))
+
+                # copy prediction from pinned memory to pageable memory on H (from previous iteration)
+                if k >= 2:
+                    for j, n in enumerate(iterations):
+                        cpu_leaves_full[j][i - 2 * batch_size: i - batch_size] = cpu_leaves[nst][j][:batch_size]
+
+                # copy predictions from device to pinned memory on H
+                gpu_leaves[nst][:real_batch_len].get(out=cpu_leaves[nst][:real_batch_len])
+                cpu_out_ready_event[nst] = stream.record(cp.cuda.Event(block=True))
+
+                last_batch_size = real_batch_len
+                last_n_stream = nst
+
+        with map_streams[1 - last_n_stream]:
+            cpu_out_ready_event[1 - last_n_stream].synchronize()
+            for j, n in enumerate(iterations):
+                cpu_leaves_full[j][X.shape[0] - (batch_size + last_batch_size): X.shape[0] - last_batch_size] = \
+                    cpu_leaves[1 - last_n_stream][j][:batch_size]
+        with map_streams[last_n_stream]:
+            cpu_out_ready_event[last_n_stream].synchronize()
+            for j, n in enumerate(iterations):
+                cpu_leaves_full[j][X.shape[0] - last_batch_size:] = cpu_leaves[last_n_stream][j][:last_batch_size]
+
+        return cpu_leaves_full
+
+    def predict(self, X, batch_size=100_000):
+        """Make prediction for the feature matrix X
+
+        Args:
+            X: np.ndarray 2d of float32, array of features
+            batch_size: int, inner batch splitting size to avoid OOM
+
+        Returns:
+            prediction: np.ndarray 2d of float32, shape (n_data, n_outputs)
+        """
+        assert batch_size > 0, 'Batch size must be a positive integer'
+
+        ngroups = max((x.ngroups for x in self.models))
+        n_out = self.base_score.shape[0]
+
+        self.to_device()
+        # special case handle, if X is already on device or size of X <= batch_size
+        if type(X) is cp.ndarray or X.shape[0] <= batch_size:
+            is_on_gpu = True
+            if type(X) is not cp.ndarray:
+                is_on_gpu = False
+                X = cp.array(X, order='C', dtype=cp.float32)
+            if not (X.flags['C_CONTIGUOUS'] or X.flags['F_CONTIGUOUS']):
+                warnings.warn("X is not 'C_CONTIGUOUS' or 'F_CONTIGUOUS', contiguous copy of array will be created."
+                              "To reduce inference time, make sure X is contiguous beforehand")
+                X = cp.ascontiguousarray(X)
+
+            gpu_pred = cp.empty((X.shape[0], n_out), dtype=cp.float32)
+            gpu_pred_leaves = cp.empty((X.shape[0], ngroups), dtype=cp.int32)
+
+            gpu_pred[:] = self.base_score
+
+            for tree in self.models:
+                tree.predict(X, gpu_pred, gpu_pred_leaves)
+
+            cp.cuda.get_current_stream().synchronize()
+            pred = self.postprocess_fn(gpu_pred)
+            if is_on_gpu:
+                return pred
+            return pred.get()
+
+        # cuda stream allocation
+        n_streams = 2  # don't change
+        map_streams = [cp.cuda.Stream() for _ in range(n_streams)]
+
+        # result allocation
+        cpu_pred_full = np.empty((X.shape[0], n_out), dtype=np.float32)
+        cpu_pred = [pinned_array(np.empty((batch_size, n_out), dtype=np.float32)) for _ in range(n_streams)]
+        gpu_pred = [cp.empty((batch_size, n_out), dtype=cp.float32) for _ in range(n_streams)]
+
+        # temp buffer for leaves
+        gpu_pred_leaves = [cp.empty((batch_size, ngroups), dtype=cp.int32) for _ in range(n_streams)]
+
+        # batch allocation
+        cpu_batch = [pinned_array(np.empty(X[0:batch_size].shape, dtype=np.float32)) for _ in range(n_streams)]
+        gpu_batch = [cp.empty(X[0:batch_size].shape, dtype=cp.float32) for _ in range(n_streams)]
+
+        cpu_batch_free_event = [None, None]
+        gpu_batch_free_event = [None, None]
+        cpu_out_ready_event = [None, None]
+        last_batch_size = 0
+        last_n_stream = 0
+        for k, i in enumerate(range(0, X.shape[0], batch_size)):
+            nst = k % n_streams
+            with map_streams[nst] as stream:
+                real_batch_len = batch_size if i + batch_size <= X.shape[0] else X.shape[0] - i
+
+                # if cpu_batch is available, copy X batch to pinned memory on H
+                if k >= 2:
+                    cpu_batch_free_event[nst].synchronize()
+                cpu_batch[nst][:real_batch_len] = X[i:i + real_batch_len].astype(cp.float32)
+
+                # copy X batch from pinned memory to D
+                if k >= 2:
+                    gpu_batch_free_event[nst].synchronize()
+                gpu_batch[nst][:real_batch_len].set(cpu_batch[nst][:real_batch_len])
+                cpu_batch_free_event[nst] = stream.record(cp.cuda.Event(block=True))
+
+                # when gpu_pred is available and cpu_out is ready, proceed to the prediction
+                if k >= 2:
+                    cpu_out_ready_event[nst].synchronize()
+                gpu_pred[nst][:] = self.base_score
+                for tree in self.models:
+                    tree.predict(gpu_batch[nst][:real_batch_len], gpu_pred[nst][:real_batch_len],
+                                 gpu_pred_leaves[nst][:real_batch_len])
+                gpu_batch_free_event[nst] = stream.record(cp.cuda.Event(block=True))
+
+                # copy prediction from pinned memory to pageable memory on H (from previous iteration)
+                if k >= 2:
+                    cpu_pred_full[i - 2 * batch_size: i - batch_size] = cpu_pred[nst][:batch_size]
+
+                # copy predictions from device to pinned memory on H
+                self.postprocess_fn(gpu_pred[nst][:real_batch_len]).get(out=cpu_pred[nst][:real_batch_len])
+                cpu_out_ready_event[nst] = stream.record(cp.cuda.Event(block=True))
+
+                last_batch_size = real_batch_len
+                last_n_stream = nst
+
+        # waiting for sync of last two batches
+        with map_streams[1 - last_n_stream]:
+            cpu_out_ready_event[1 - last_n_stream].synchronize()
+            cpu_pred_full[X.shape[0] - (batch_size + last_batch_size): X.shape[0] - last_batch_size] = \
+                cpu_pred[1 - last_n_stream][:batch_size]
+        with map_streams[last_n_stream]:
+            cpu_out_ready_event[last_n_stream].synchronize()
+            cpu_pred_full[X.shape[0] - last_batch_size:] = cpu_pred[last_n_stream][:last_batch_size]
+
+        return cpu_pred_full
+
+    def predict_staged(self, X, iterations=None, batch_size=100_000):
+        """Make prediction from different stages for the feature matrix X
+
+        Args:
+            X: 2d np.ndarray of float32, array of features
+            iterations: list of int or None. If list of ints is passed, prediction will be made only
+                for given iterations, otherwise - for all iterations
+            batch_size: int, inner batch splitting size to avoid OOM
+
+        Returns:
+            prediction, np.ndarray 2d of float32, shape (n_iterations, n_data, n_out)
+        """
+        assert batch_size > 0, 'Batch size must be a positive integer'
+
+        if iterations is None:
+            iterations = np.arange(len(self.models))
+        else:
+            iterations = np.array(iterations, dtype=np.int64)
+
+        assert len(iterations) > 0, 'Iterations are empty sequence'
+        assert (max(iterations) < len(self.models)) and (min(iterations) >= 0), 'Invalid stage numbers'
+        assert len(np.unique(iterations)) == len(iterations), 'Duplicate values in stages are not allowed'
+
+        ngroups = max((x.ngroups for x in self.models))
+        n_out = self.base_score.shape[0]
+
+        self.to_device()
+        # special case handle, if X is already on device or size of X <= batch_size
+        if type(X) is cp.ndarray or X.shape[0] <= batch_size:
+            is_on_gpu = True
+            if type(X) is not cp.ndarray:
+                is_on_gpu = False
+                X = cp.array(X, order='C', dtype=cp.float32)
+                pred_full = np.empty((len(iterations), X.shape[0], n_out), dtype=cp.float32)
+            else:
+                pred_full = cp.empty((len(iterations), X.shape[0], n_out), dtype=cp.float32)
+            if not (X.flags['C_CONTIGUOUS'] or X.flags['F_CONTIGUOUS']):
+                warnings.warn("X is not 'C_CONTIGUOUS' or 'F_CONTIGUOUS', contiguous copy of array will be created."
+                              "To reduce inference time, make sure X is contiguous beforehand")
+                X = cp.ascontiguousarray(X)
+
+            gpu_pred = cp.empty((X.shape[0], n_out), dtype=cp.float32)
+            gpu_pred_leaves = cp.empty((X.shape[0], ngroups), dtype=cp.int32)
+
+            gpu_pred[:] = self.base_score
+            next_out = 0
+            for n, tree in enumerate(self.models):
+                tree.predict(X, gpu_pred, gpu_pred_leaves)
+                if n == iterations[next_out]:
+                    if is_on_gpu:
+                        pred_full[next_out] = self.postprocess_fn(gpu_pred)
+                    else:
+                        self.postprocess_fn(gpu_pred).get(out=pred_full[next_out])
+                    next_out += 1
+                    if next_out >= len(iterations):
+                        cp.cuda.get_current_stream().synchronize()
+                        return pred_full
+
+        n_streams = 2  # don't change
+        map_streams = [cp.cuda.Stream() for _ in range(n_streams)]
+
+        # result allocation
+        cpu_pred_full = np.empty((len(iterations), X.shape[0], n_out), dtype=np.float32)
+        cpu_pred = [pinned_array(np.empty((len(iterations), batch_size, n_out), dtype=np.float32)) for _ in
+                    range(n_streams)]
+        gpu_pred = [cp.empty((batch_size, n_out), dtype=cp.float32) for _ in range(n_streams)]
+
+        # temp buffer for leaves
+        gpu_pred_leaves = [cp.empty((batch_size, ngroups), dtype=cp.int32) for _ in range(n_streams)]
+
+        # batch allocation
+        cpu_batch = [pinned_array(np.empty(X[0:batch_size].shape, dtype=np.float32)) for _ in range(n_streams)]
+        gpu_batch = [cp.empty(X[0:batch_size].shape, dtype=np.float32) for _ in range(n_streams)]
+
+        cpu_batch_free_event = [None, None]
+        cpu_out_ready_event = [None, None]
+        last_batch_size = 0
+        last_n_stream = 0
+        for k, i in enumerate(range(0, X.shape[0], batch_size)):
+            nst = k % n_streams
+            with map_streams[nst] as stream:
+                real_batch_len = batch_size if i + batch_size <= X.shape[0] else X.shape[0] - i
+
+                # if cpu_batch is available, copy X batch to pinned memory on H
+                if k >= 2:
+                    cpu_batch_free_event[nst].synchronize()
+                cpu_batch[nst][:real_batch_len] = X[i:i + real_batch_len].astype(np.float32)
+
+                # copy X batch from pinned memory to D
+                if k >= 2:
+                    cpu_out_ready_event[nst].synchronize()
+                gpu_batch[nst][:real_batch_len].set(cpu_batch[nst][:real_batch_len])
+                cpu_batch_free_event[nst] = stream.record(cp.cuda.Event(block=True))
+                gpu_pred[nst][:] = self.base_score
+
+                # copy prediction from pinned memory to pageable memory on H (from previous iteration)
+                if k >= 2:
+                    cpu_pred_full[:, i - 2 * batch_size: i - batch_size] = cpu_pred[nst][:, :batch_size]
+
+                i_next = 0
+                for i_tree, tree in enumerate(self.models):
+                    tree.predict(gpu_batch[nst][:real_batch_len], gpu_pred[nst][:real_batch_len],
+                                 gpu_pred_leaves[nst][:real_batch_len])
+                    if iterations[i_next] == i_tree:
+                        self.postprocess_fn(gpu_pred[nst][:real_batch_len]).get(
+                            out=cpu_pred[nst][i_next][:real_batch_len])
+                        i_next += 1
+                        if i_next >= len(iterations):
+                            break
+                cpu_out_ready_event[nst] = stream.record(cp.cuda.Event(block=True))
+
+                last_batch_size = real_batch_len
+                last_n_stream = nst
+
+        # waiting for sync of last two batches
+        with map_streams[1 - last_n_stream]:
+            cpu_out_ready_event[1 - last_n_stream].synchronize()
+            cpu_pred_full[:, X.shape[0] - (batch_size + last_batch_size): X.shape[0] - last_batch_size] = \
+                cpu_pred[1 - last_n_stream][:, :batch_size]
+        with map_streams[last_n_stream]:
+            cpu_out_ready_event[last_n_stream].synchronize()
+            cpu_pred_full[:, X.shape[0] - last_batch_size:] = cpu_pred[last_n_stream][:, :last_batch_size]
+
+        return cpu_pred_full
+
+    def dump(self, file):
+        """Dump model data to json
+
+        Args:
+            file: str, file path
+
+        Returns:
+
+        """
+        dump(self, file)
+        return
+
+    def load(self, file):
+        """Load model data from json
+
+        Args:
+            file: str, file path
+
+        Returns:
+            Py-Boost Ensemble
+        """
+        load(self, file)
+        return self
```

### Comparing `py_boost-0.4.3/py_boost/gpu/boosting.py` & `py_boost-0.5.0/py_boost/gpu/boosting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,353 +1,370 @@
-"""Gradient boosting builder"""
-
-try:
-    import cupy as cp
-except Exception:
-    pass
-from .base import Ensemble
-from .losses import loss_alias
-from .tree import DepthwiseTreeBuilder
-from .utils import pad_and_move, validate_input
-from ..callbacks.callback import EarlyStopping, EvalHistory, CallbackPipeline
-from ..multioutput.sketching import GradSketch
-from ..sampling.bagging import BaseSampler
-from ..multioutput.target_splitter import SingleSplitter, OneVsAllSplitter
-
-
-class GradientBoosting(Ensemble):
-    """Basic Gradient Boosting on depthwise trees"""
-
-    def __init__(self, loss,
-                 metric=None,
-                 ntrees=100,
-                 lr=0.05,
-                 min_gain_to_split=0,
-                 lambda_l2=1,
-                 gd_steps=1,
-
-                 max_depth=6,
-                 min_data_in_leaf=10,
-                 colsample=1.,
-                 subsample=1.,
-                 target_splitter='Single',
-                 multioutput_sketch=None,
-                 use_hess=True,
-
-                 quantization='Quantile',
-                 quant_sample=2000000,
-                 max_bin=256,
-                 min_data_in_bin=3,
-
-                 es=100,
-                 seed=42,
-                 verbose=10,
-                 callbacks=None,
-
-                 debug=False
-                 ):
-        """
-
-        Args:
-            loss: str or Loss, loss function
-            metric: None or str or Metric, metric
-            ntrees: int, maximum number of trees
-            lr: float, learning rate
-            min_gain_to_split: float >=0, minimal gain to split
-            lambda_l2: float > 0, l2 leaf regularization
-            gd_steps: int > 0, number of gradient steps while computing leaf values
-
-            max_depth: int > 0, maximum tree depth. Setting it to large values (>12) may cause OOM for wide datasets
-            min_data_in_leaf: int, minimal leaf size. Note - for some loss fn leaf size is approximated
-                with hessian values to speed up training
-            colsample: float or Callable, sumsample of columns to construct trees or callable - custom sampling
-            subsample: float or Callable, sumsample of rows to construct trees or callable - custom sampling
-            quant_sample: int, subsample to quantize features
-            target_splitter: str or Callable, target splitter, defined multioutput strategy:
-                'Single', 'OneVsAll' or custom
-            multioutput_sketch: None or Callable. Defines the sketching strategy to simplify scoring function
-                in multioutput case. If None full scoring function is used
-            use_hess: If True hessians will be used in tree structure search
-
-            quantization: str or Quantizer, method for quantizatrion. One of 'Quantile', 'Uniform',
-                'Uniquant' or custom implementation
-            quant_sample: int, subsample to quantize features
-            max_bin: int in [2, 256] maximum number of bins to quantize features
-            min_data_in_bin: int in [2, 256] minimal bin size. NOTE: currently ignored
-
-            es: int, early stopping rounds. If 0, no early stopping
-            seed: int, random state
-            verbose: int, verbosity freq
-            callbacks: list of Callback, callbacks to customize training are passed here
-
-            debug: bool, if debug mode is enabled (it removes ability to use deprecated functions,
-                         thus optimizing memory usage)
-        """
-
-        super().__init__()
-
-        self.params = {
-
-            'loss': loss,
-            'metric': metric,
-            'ntrees': ntrees,
-            'lr': lr,
-            'min_gain_to_split': min_gain_to_split,
-            'lambda_l2': lambda_l2,
-            'gd_steps': gd_steps,
-
-            'max_depth': max_depth,
-            'min_data_in_leaf': min_data_in_leaf,
-            'colsample': colsample,
-            'subsample': subsample,
-
-            'target_splitter': target_splitter,
-            'multioutput_sketch': multioutput_sketch,
-            'use_hess': use_hess,
-
-            'quantization': quantization,
-            'quant_sample': quant_sample,
-            'max_bin': max_bin,
-            'min_data_in_bin': min_data_in_bin,
-
-            'es': es,
-            'seed': seed,
-            'verbose': verbose,
-            'callbacks': callbacks,
-
-            'debug': debug
-        }
-
-    def _infer_params(self):
-
-        self.ntrees = self.params['ntrees']
-        self.lr = self.params['lr']
-        self.min_gain_to_split = self.params['min_gain_to_split']
-        self.lambda_l2 = self.params['lambda_l2']
-        self.gd_steps = self.params['gd_steps']
-
-        self.max_depth = self.params['max_depth']
-        self.min_data_in_leaf = self.params['min_data_in_leaf']
-        self.use_hess = self.params['use_hess']
-
-        self.colsample = self.params['colsample']
-        if type(self.params['colsample']) in [float, int]:
-            self.colsample = BaseSampler(self.params['colsample'], axis=1)
-
-        self.subsample = self.params['subsample']
-        if type(self.params['subsample']) in [float, int]:
-            self.subsample = BaseSampler(self.params['subsample'], axis=0)
-
-        if self.params['target_splitter'] == 'Single':
-            splitter = SingleSplitter()
-        elif self.params['target_splitter'] == 'OneVsAll':
-            splitter = OneVsAllSplitter()
-        else:
-            splitter = self.params['target_splitter']
-
-        self.target_splitter = splitter
-
-        self.multioutput_sketch = self.params['multioutput_sketch']
-        if self.params['multioutput_sketch'] is None:
-            self.multioutput_sketch = GradSketch()
-
-        self.quantization = self.params['quantization']
-        self.quant_sample = self.params['quant_sample']
-        self.max_bin = self.params['max_bin']
-        self.min_data_in_bin = self.params['min_data_in_bin']
-
-        self.es = self.params['es']
-        self.verbose = self.params['verbose']
-
-        self.loss = self.params['loss']
-        if type(self.params['loss']) is str:
-            self.loss = loss_alias[self.params['loss']]
-
-        self.metric = self.params['metric']
-        if self.params['metric'] is None or type(self.params['metric']) is str:
-            self.metric = self.loss.get_metric_from_string(self.params['metric'])
-        self.seed = self.params['seed']
-
-        self.history = []
-
-        self.callbacks = CallbackPipeline(
-
-            self.subsample,
-            self.colsample,
-            self.target_splitter,
-            self.multioutput_sketch,
-            *([] if self.params['callbacks'] is None else self.params['callbacks']),
-            EvalHistory(self.history, verbose=self.params['verbose']),
-            EarlyStopping(self.params['es']),
-        )
-
-    def _fit(self, builder, build_info):
-        """Fit with tree builder and build info
-
-        Args:
-            builder: DepthwiseTreeBuilder
-            build_info: build info state dict
-
-        Returns:
-
-        """
-        train, valid = build_info['data']['train'], build_info['data']['valid']
-        self.callbacks.before_train(build_info)
-
-        for i in range(self.ntrees):
-
-            build_info['num_iter'] = i
-            train['grad'], train['hess'] = self.loss(train['target'], train['ensemble'])
-
-            self.callbacks.before_iteration(build_info)
-
-            tree, leaves, preds, val_leaves, val_preds = \
-                builder.build_tree(train['features_gpu'],
-                                   train['grad'],
-                                   train['hess'],
-                                   train['sample_weight'],
-                                   lambda x: self.loss(train['target'], train['ensemble'] + x),
-                                   *valid['features_gpu'])
-
-            # update ensemble
-            train['ensemble'] += preds
-            for vp, tp in zip(valid['ensemble'], val_preds):
-                vp += tp
-
-            train['last_tree'] = {
-
-                'leaves': leaves,
-                'preds': preds
-
-            }
-            valid['last_tree'] = {
-
-                'leaves': val_leaves,
-                'preds': val_preds
-
-            }
-
-            self.models.append(tree)
-            # check exit info
-            if self.callbacks.after_iteration(build_info):
-                tree.reformat(nfeats=self.nfeats, debug=self.params['debug'])
-                break
-            tree.reformat(nfeats=self.nfeats, debug=self.params['debug'])
-
-        self.callbacks.after_train(build_info)
-        self.base_score = self.base_score.get()
-
-    def fit(self, X, y, sample_weight=None, eval_sets=None):
-        """Fit model
-
-        Args:
-            X: np.ndarray feature matrix
-            y: np.ndarray of target
-            sample_weight: np.ndarray of sample weights
-            eval_sets: list of dict of eval sets. Ex [{'X':X0, 'y': y0, 'sample_weight': w0}, ...}]
-
-        Returns:
-            trained instance
-        """
-        self._infer_params()
-
-        X, y, sample_weight, eval_sets = validate_input(X, y, sample_weight, eval_sets)
-        # fit and free memory
-        mempool = cp.cuda.MemoryPool()
-        with cp.cuda.using_allocator(allocator=mempool.malloc):
-            # quantize
-            X_enc, max_bin, borders, eval_enc = self.quantize(X, eval_sets)
-            # create build info
-            builder, build_info = self._create_build_info(mempool, X, X_enc, y, sample_weight,
-                                                          max_bin, borders, eval_sets, eval_enc)
-            self._fit(builder, build_info)
-        mempool.free_all_blocks()
-
-        return self
-
-    def _create_build_info(self, mempool, X, X_enc, y, sample_weight, max_bin, borders, eval_sets, eval_enc):
-        """Quantize data, create tree builder and build_info
-
-        Args:
-            mempool: cp.cuda.MemoryPool, memory pool to use
-            X: np.ndarray feature matrix
-            y: np.ndarray of target
-            sample_weight: np.ndarray of sample weights
-            eval_sets: list of dict of eval sets. Ex [{'X':X0, 'y': y0, 'sample_weight': w0}, ...}]
-
-        Returns:
-            DepthwiseTreeBuilder, build_info
-        """
-        # quantization
-
-        y = cp.array(y, order='C', dtype=cp.float32)
-
-        if sample_weight is not None:
-            sample_weight = cp.array(sample_weight, order='C', dtype=cp.float32)
-
-        X_cp = pad_and_move(X_enc)
-
-        X_val = [cp.array(x, order='C') for x in eval_enc]
-        y_val = [cp.array(x['y'], order='C', dtype=cp.float32) for x in eval_sets]
-        w_val = [None if x['sample_weight'] is None else cp.array(x['sample_weight'], order='C', dtype=cp.float32)
-                 for x in eval_sets]
-
-        # save nfeatures for the feature importances
-        self.nfeats = X.shape[1]
-        self.postprocess_fn = self.loss.postprocess_output
-
-        builder = DepthwiseTreeBuilder(borders,
-                                       use_hess=self.use_hess,
-                                       colsampler=self.colsample,
-                                       subsampler=self.subsample,
-                                       target_splitter=self.target_splitter,
-                                       multioutput_sketch=self.multioutput_sketch,
-                                       gd_steps=self.gd_steps,
-                                       lr=self.lr,
-                                       min_gain_to_split=self.min_gain_to_split,
-                                       min_data_in_leaf=self.min_data_in_leaf,
-                                       lambda_l2=self.lambda_l2,
-                                       max_depth=self.max_depth,
-                                       max_bin=max_bin,
-                                       )
-        cp.random.seed(self.seed)
-
-        y = self.loss.preprocess_input(y)
-        y_val = [self.loss.preprocess_input(x) for x in y_val]
-        self.base_score = self.loss.base_score(y)
-
-        # init ensembles
-        ens = cp.empty((y.shape[0], self.base_score.shape[0]), order='C', dtype=cp.float32)
-        ens[:] = self.base_score
-        # init val ens
-        val_ens = [cp.empty((x.shape[0], self.base_score.shape[0]), order='C') for x in y_val]
-        for ve in val_ens:
-            ve[:] = self.base_score
-
-        self.models = []
-
-        build_info = {
-            'data': {
-                'train': {
-                    'features_cpu': X,
-                    'features_gpu': X_cp,
-                    'target': y,
-                    'sample_weight': sample_weight,
-                    'ensemble': ens,
-                    'grad': None,
-                    'hess': None
-                },
-                'valid': {
-                    'features_cpu': [dat['X'] for dat in eval_sets],
-                    'features_gpu': X_val,
-                    'target': y_val,
-                    'sample_weight': w_val,
-                    'ensemble': val_ens,
-                }
-            },
-            'borders': borders,
-            'model': self,
-            'mempool': mempool,
-            'builder': builder
-        }
-
-        return builder, build_info
+"""Gradient boosting builder"""
+
+try:
+    import cupy as cp
+except Exception:
+    pass
+from .base import Ensemble
+from .losses import loss_alias
+from .tree import DepthwiseTreeBuilder
+from .utils import pad_and_move, validate_input
+from ..callbacks.callback import EarlyStopping, EvalHistory, CallbackPipeline
+from ..multioutput.sketching import GradSketch
+from ..multioutput.target_splitter import SingleSplitter, OneVsAllSplitter
+from ..sampling.bagging import BaseSampler
+
+
+class GradientBoosting(Ensemble):
+    """Basic Gradient Boosting on depthwise trees"""
+
+    def __init__(self, loss,
+                 metric=None,
+                 ntrees=100,
+                 lr=0.05,
+                 min_gain_to_split=0,
+                 lambda_l2=1,
+                 gd_steps=1,
+
+                 max_depth=6,
+                 min_data_in_leaf=10,
+                 colsample=1.,
+                 subsample=1.,
+                 target_splitter='Single',
+                 multioutput_sketch=None,
+                 use_hess=True,
+
+                 quantization='Quantile',
+                 quant_sample=2000000,
+                 max_bin=256,
+                 min_data_in_bin=3,
+
+                 es=100,
+                 seed=42,
+                 verbose=10,
+                 callbacks=None,
+
+                 debug=False
+                 ):
+        """
+
+        Args:
+            loss: str or Loss, loss function
+            metric: None or str or Metric, metric
+            ntrees: int, maximum number of trees
+            lr: float, learning rate
+            min_gain_to_split: float >=0, minimal gain to split
+            lambda_l2: float > 0, l2 leaf regularization
+            gd_steps: int > 0, number of gradient steps while computing leaf values
+
+            max_depth: int > 0, maximum tree depth. Setting it to large values (>12) may cause OOM for wide datasets
+            min_data_in_leaf: int, minimal leaf size. Note - for some loss fn leaf size is approximated
+                with hessian values to speed up training
+            colsample: float or Callable, sumsample of columns to construct trees or callable - custom sampling
+            subsample: float or Callable, sumsample of rows to construct trees or callable - custom sampling
+            quant_sample: int, subsample to quantize features
+            target_splitter: str or Callable, target splitter, defined multioutput strategy:
+                'Single', 'OneVsAll' or custom
+            multioutput_sketch: None or Callable. Defines the sketching strategy to simplify scoring function
+                in multioutput case. If None full scoring function is used
+            use_hess: If True hessians will be used in tree structure search
+
+            quantization: str or Quantizer, method for quantizatrion. One of 'Quantile', 'Uniform',
+                'Uniquant' or custom implementation
+            quant_sample: int, subsample to quantize features
+            max_bin: int in [2, 256] maximum number of bins to quantize features
+            min_data_in_bin: int in [2, 256] minimal bin size. NOTE: currently ignored
+
+            es: int, early stopping rounds. If 0, no early stopping
+            seed: int, random state
+            verbose: int, verbosity freq
+            callbacks: list of Callback, callbacks to customize training are passed here
+
+            debug: bool, if debug mode is enabled (it removes ability to use deprecated functions,
+                         thus optimizing memory usage)
+        """
+
+        super().__init__()
+
+        self.params = {
+
+            'loss': loss,
+            'metric': metric,
+            'ntrees': ntrees,
+            'lr': lr,
+            'min_gain_to_split': min_gain_to_split,
+            'lambda_l2': lambda_l2,
+            'gd_steps': gd_steps,
+
+            'max_depth': max_depth,
+            'min_data_in_leaf': min_data_in_leaf,
+            'colsample': colsample,
+            'subsample': subsample,
+
+            'target_splitter': target_splitter,
+            'multioutput_sketch': multioutput_sketch,
+            'use_hess': use_hess,
+
+            'quantization': quantization,
+            'quant_sample': quant_sample,
+            'max_bin': max_bin,
+            'min_data_in_bin': min_data_in_bin,
+
+            'es': es,
+            'seed': seed,
+            'verbose': verbose,
+            'callbacks': callbacks,
+
+            'debug': debug
+        }
+
+    def _infer_params(self):
+
+        self.ntrees = self.params['ntrees']
+        self.lr = self.params['lr']
+
+        assert self.params['min_gain_to_split'] >= 0, 'Param min_gain_to_split should be >= 0'
+
+        self.min_gain_to_split = self.params['min_gain_to_split']
+        self.lambda_l2 = self.params['lambda_l2']
+        self.gd_steps = self.params['gd_steps']
+
+        self.max_depth = self.params['max_depth']
+        self.min_data_in_leaf = self.params['min_data_in_leaf']
+        self.use_hess = self.params['use_hess']
+
+        self.colsample = self.params['colsample']
+        if type(self.params['colsample']) in [float, int]:
+            self.colsample = BaseSampler(self.params['colsample'], axis=1)
+
+        self.subsample = self.params['subsample']
+        if type(self.params['subsample']) in [float, int]:
+            self.subsample = BaseSampler(self.params['subsample'], axis=0)
+
+        if self.params['target_splitter'] == 'Single':
+            splitter = SingleSplitter()
+        elif self.params['target_splitter'] == 'OneVsAll':
+            splitter = OneVsAllSplitter()
+        else:
+            splitter = self.params['target_splitter']
+
+        self.target_splitter = splitter
+
+        self.multioutput_sketch = self.params['multioutput_sketch']
+        if self.params['multioutput_sketch'] is None:
+            self.multioutput_sketch = GradSketch()
+
+        self.quantization = self.params['quantization']
+        self.quant_sample = self.params['quant_sample']
+        self.max_bin = self.params['max_bin']
+        self.min_data_in_bin = self.params['min_data_in_bin']
+
+        self.es = self.params['es']
+        self.verbose = self.params['verbose']
+
+        self.loss = self.params['loss']
+        if type(self.params['loss']) is str:
+            self.loss = loss_alias[self.params['loss']]
+
+        self.postprocess_fn = self.loss.postprocess_output
+
+        self.metric = self.params['metric']
+        if self.params['metric'] is None or type(self.params['metric']) is str:
+            self.metric = self.loss.get_metric_from_string(self.params['metric'])
+        self.seed = self.params['seed']
+
+        self.history = []
+
+        self.callbacks = CallbackPipeline(
+
+            self.subsample,
+            self.colsample,
+            self.target_splitter,
+            self.multioutput_sketch,
+            *([] if self.params['callbacks'] is None else self.params['callbacks']),
+            EvalHistory(self.history, verbose=self.params['verbose']),
+            EarlyStopping(self.params['es']),
+        )
+
+    def _fit(self, builder, build_info):
+        """Fit with tree builder and build info
+
+        Args:
+            builder: DepthwiseTreeBuilder
+            build_info: build info state dict
+
+        Returns:
+
+        """
+        train, valid = build_info['data']['train'], build_info['data']['valid']
+        self.callbacks.before_train(build_info)
+
+        for i in range(self.ntrees):
+
+            build_info['num_iter'] = i
+            train['grad'], train['hess'] = self.loss(train['target'], train['ensemble'])
+
+            self.callbacks.before_iteration(build_info)
+
+            tree, leaves, preds, val_leaves, val_preds = \
+                builder.build_tree(train['features_gpu'],
+                                   train['grad'],
+                                   train['hess'],
+                                   train['sample_weight'],
+                                   lambda x: self.loss(train['target'], train['ensemble'] + x),
+                                   *valid['features_gpu'])
+
+            # update ensemble
+            train['ensemble'] += preds
+            for vp, tp in zip(valid['ensemble'], val_preds):
+                vp += tp
+
+            train['last_tree'] = {
+
+                'leaves': leaves,
+                'preds': preds
+
+            }
+            valid['last_tree'] = {
+
+                'leaves': val_leaves,
+                'preds': val_preds
+
+            }
+
+            self.models.append(tree)
+            # check exit info
+            if self.callbacks.after_iteration(build_info):
+                tree.reformat(nfeats=self.nfeats, debug=self.params['debug'])
+                break
+            tree.reformat(nfeats=self.nfeats, debug=self.params['debug'])
+
+        self.callbacks.after_train(build_info)
+        self.base_score = self.base_score.get()
+
+    def fit(self, X, y, sample_weight=None, eval_sets=None):
+        """Fit model
+
+        Args:
+            X: np.ndarray feature matrix
+            y: np.ndarray of target
+            sample_weight: np.ndarray of sample weights
+            eval_sets: list of dict of eval sets. Ex [{'X':X0, 'y': y0, 'sample_weight': w0}, ...}]
+
+        Returns:
+            trained instance
+        """
+        self._infer_params()
+
+        X, y, sample_weight, eval_sets = validate_input(X, y, sample_weight, eval_sets)
+        # fit and free memory
+        mempool = cp.cuda.MemoryPool()
+        with cp.cuda.using_allocator(allocator=mempool.malloc):
+            # quantize
+            X_enc, max_bin, borders, eval_enc = self.quantize(X, eval_sets)
+            # create build info
+            builder, build_info = self._create_build_info(mempool, X, X_enc, y, sample_weight,
+                                                          max_bin, borders, eval_sets, eval_enc)
+            self._fit(builder, build_info)
+        mempool.free_all_blocks()
+
+        return self
+
+    def _create_build_info(self, mempool, X, X_enc, y, sample_weight, max_bin, borders, eval_sets, eval_enc):
+        """Quantize data, create tree builder and build_info
+
+        Args:
+            mempool: cp.cuda.MemoryPool, memory pool to use
+            X: np.ndarray feature matrix
+            y: np.ndarray of target
+            sample_weight: np.ndarray of sample weights
+            eval_sets: list of dict of eval sets. Ex [{'X':X0, 'y': y0, 'sample_weight': w0}, ...}]
+
+        Returns:
+            DepthwiseTreeBuilder, build_info
+        """
+        # quantization
+
+        y = cp.array(y, order='C', dtype=cp.float32)
+
+        if sample_weight is not None:
+            sample_weight = cp.array(sample_weight, order='C', dtype=cp.float32)
+
+        X_cp = pad_and_move(X_enc)
+
+        X_val = [cp.array(x, order='C') for x in eval_enc]
+        y_val = [cp.array(x['y'], order='C', dtype=cp.float32) for x in eval_sets]
+        w_val = [None if x['sample_weight'] is None else cp.array(x['sample_weight'], order='C', dtype=cp.float32)
+                 for x in eval_sets]
+
+        # save nfeatures for the feature importances
+        self.nfeats = X.shape[1]
+
+        builder = DepthwiseTreeBuilder(borders,
+                                       use_hess=self.use_hess,
+                                       colsampler=self.colsample,
+                                       subsampler=self.subsample,
+                                       target_splitter=self.target_splitter,
+                                       multioutput_sketch=self.multioutput_sketch,
+                                       gd_steps=self.gd_steps,
+                                       lr=self.lr,
+                                       min_gain_to_split=self.min_gain_to_split,
+                                       min_data_in_leaf=self.min_data_in_leaf,
+                                       lambda_l2=self.lambda_l2,
+                                       max_depth=self.max_depth,
+                                       max_bin=max_bin,
+                                       )
+        cp.random.seed(self.seed)
+
+        y = self.loss.preprocess_input(y)
+        y_val = [self.loss.preprocess_input(x) for x in y_val]
+        self.base_score = self.loss.base_score(y)
+
+        # init ensembles
+        ens = cp.empty((y.shape[0], self.base_score.shape[0]), order='C', dtype=cp.float32)
+        ens[:] = self.base_score
+        # init val ens
+        val_ens = [cp.empty((x.shape[0], self.base_score.shape[0]), order='C') for x in y_val]
+        for ve in val_ens:
+            ve[:] = self.base_score
+
+        self.models = []
+
+        build_info = {
+            'data': {
+                'train': {
+                    'features_cpu': X,
+                    'features_gpu': X_cp,
+                    'target': y,
+                    'sample_weight': sample_weight,
+                    'ensemble': ens,
+                    'grad': None,
+                    'hess': None
+                },
+                'valid': {
+                    'features_cpu': [dat['X'] for dat in eval_sets],
+                    'features_gpu': X_val,
+                    'target': y_val,
+                    'sample_weight': w_val,
+                    'ensemble': val_ens,
+                }
+            },
+            'borders': borders,
+            'model': self,
+            'mempool': mempool,
+            'builder': builder
+        }
+
+        return builder, build_info
+
+    def load(self, file):
+        """Load weights fromm file
+
+        Args:
+            file: str, file path
+
+        Returns:
+            Py-Boost GradientBoosting
+        """
+        self._infer_params()
+
+        return super().load(file)
```

### Comparing `py_boost-0.4.3/py_boost/gpu/losses/losses.py` & `py_boost-0.5.0/py_boost/gpu/losses/losses.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,239 +1,239 @@
-"""Common losses"""
-
-import numpy as np
-try:
-    import cupy as cp
-    CUDA_FOUND = True
-except Exception:
-    CUDA_FOUND = False
-
-from .metrics import metric_alias, RMSEMetric, RMSLEMetric, BCEMetric
-from .multiclass_metrics import multiclass_metric_alias, CrossEntropyMetric
-
-
-class Loss:
-    """Base class to define loss function"""
-
-    def get_grad_hess(self, y_true, y_pred):
-        """Method implements how to calculate gradients and hessians.
-        Output gradient should have the shape (n_samples, n_outputs)
-        Output hessian should have the shape (n_samples, n_outputs) or (n_samples, 1)
-            if the same hess used for all outputs (for ex. MSELoss)
-
-        Definition don't use sample_weight, because it is applied later at the tree building stage
-
-        Args:
-            y_true: cp.ndarray, target
-            y_pred: cp.ndarray, current prediction
-
-        Returns:
-
-        """
-        raise NotImplementedError
-
-    def __call__(self, y_true, y_pred):
-        grad, hess = self.get_grad_hess(y_true, y_pred)
-        return grad, hess
-
-    def preprocess_input(self, y_true):
-        """Method defines how raw input target variable should be processed before train starts
-            (ex. applying log1p for MSLELoss)
-
-        Args:
-            y_true: cp.ndarray, raw target
-
-        Returns:
-
-        """
-        return y_true
-
-    def postprocess_output(self, y_pred):
-        """Method defines how to postprocess sum of trees to output prediction (ex. apply sigmoid for BCELoss)
-
-        Args:
-            y_pred: cp.ndarray, predictions
-
-        Returns:
-
-        """
-        return y_pred
-
-    def base_score(self, y_true):
-        """Method defines how to initialize an empty ensemble (ex. initialize with mean values for MSELoss)
-
-        Args:
-            y_true: cp.ndarray, processed target (after applying preprocess_input)
-
-        Returns:
-
-        """
-        raise NotImplementedError
-
-    def get_metric_from_string(self, name=None):
-        """Method defines how to interpret eval metric given in str format or None.
-        For ex. you can define the default metric to use here if name is None
-
-        Args:
-            name:
-
-        Returns:
-
-        """
-        return metric_alias['name']
-
-
-class MSELoss(Loss):
-    """MSE Loss function for regression/multiregression"""
-
-    def get_grad_hess(self, y_true, y_pred):
-        return (y_pred - y_true), cp.ones((y_true.shape[0], 1), dtype=cp.float32)
-
-    def base_score(self, y_true):
-        return y_true.mean(axis=0)
-
-    def get_metric_from_string(self, name=None):
-        if name is None:
-            return RMSEMetric()
-        return metric_alias[name]
-
-
-class MSLELoss(Loss):
-    """MSLE Loss function for regression/multiregression"""
-
-    def preprocess_input(self, y_true):
-        assert (y_true >= 0).all(), 'Inputs for msle should be non negative'
-
-        return y_true
-
-    def get_grad_hess(self, y_true, y_pred):
-        y_true = cp.log1p(y_true)
-
-        return (y_pred - y_true), cp.ones((y_true.shape[0], 1), dtype=cp.float32)
-
-    def postprocess_output(self, y_pred):
-        return cp.expm1(y_pred)
-
-    def base_score(self, y_true):
-        y_true = cp.log1p(y_true)
-        return y_true.mean(axis=0)
-
-    def get_metric_from_string(self, name=None):
-        if name is None:
-            return RMSLEMetric()
-        return metric_alias[name]
-
-
-class BCELoss(Loss):
-    """LogLoss for binary/multilabel classification"""
-
-    def __init__(self, clip_value=1e-7):
-        self.clip_value = clip_value
-
-    def base_score(self, y_true):
-        means = cp.clip(y_true.mean(axis=0), self.clip_value, 1 - self.clip_value)
-        return cp.log(means / (1 - means))
-
-    def get_grad_hess(self, y_true, y_pred):
-        pred = 1 / (1 + cp.exp(-y_pred))
-        pred = cp.clip(pred, self.clip_value, 1 - self.clip_value)
-        grad = pred - y_true
-        hess = pred * (1 - pred)
-
-        return grad, hess
-
-    def postprocess_output(self, y_pred):
-        xp = np if type(y_pred) is np.ndarray else cp
-        pred = 1 / (1 + xp.exp(-y_pred))
-        pred = xp.clip(pred, self.clip_value, 1 - self.clip_value)
-
-        return pred
-
-    def get_metric_from_string(self, name=None):
-        if name is None:
-            return BCEMetric()
-        return metric_alias[name]
-
-
-def softmax(x, clip_val=1e-5):
-    
-    xp = np if type(x) is np.ndarray else cp
-    exp_p = xp.exp(x - x.max(axis=1, keepdims=True))
-
-    return xp.clip(exp_p / exp_p.sum(axis=1, keepdims=True), clip_val, 1 - clip_val)
-
-
-# multiclass losses
-
-ce_grad_kernel = cp.ElementwiseKernel(
-    'T pred, raw S label, raw S nlabels, T factor',
-    'T grad, T hess',
-
-    """
-    int y_pr = i % nlabels;
-    int y_tr = label[i / nlabels];
-
-    grad = pred - (float) (y_pr == y_tr);
-    hess = pred * (1. - pred) * factor;
-
-    """,
-    "ce_grad_kernel"
-) if CUDA_FOUND else None
-
-
-def ce_grad(y_true, y_pred):
-    factor = y_pred.shape[1] / (y_pred.shape[1] - 1)
-    grad, hess = ce_grad_kernel(y_pred, y_true, y_pred.shape[1], factor)
-
-    return grad, hess
-
-
-class CrossEntropyLoss(Loss):
-    """CrossEntropy for multiclass classification"""
-
-    def __init__(self, clip_value=1e-6):
-        self.clip_value = clip_value
-
-    def base_score(self, y_true):
-        num_classes = int(y_true.max() + 1)
-        hist = cp.zeros((num_classes,), dtype=cp.float32)
-
-        return hist
-
-    def get_grad_hess(self, y_true, y_pred):
-        pred = softmax(y_pred, self.clip_value)
-        grad, hess = ce_grad(y_true, pred)
-        return grad, hess
-
-    def postprocess_output(self, y_pred):
-        
-        return softmax(y_pred, self.clip_value)
-
-    def preprocess_input(self, y_true):
-        return y_true[:, 0].astype(cp.int32)
-
-    def get_metric_from_string(self, name=None):
-        if name is None:
-            return CrossEntropyMetric()
-        return multiclass_metric_alias[name]
-
-
-loss_alias = {
-
-    # for bce
-    'binary': BCELoss(),
-    'bce': BCELoss(),
-    'multilabel': BCELoss(),
-    'logloss': BCELoss(),
-
-    # for multiclass
-    'multiclass': CrossEntropyLoss(),
-    'crossentropy': CrossEntropyLoss(),
-
-    # for regression
-    'mse': MSELoss(),
-    'regression': MSELoss(),
-    'l2': MSELoss(),
-    'multitask': MSELoss(),
-    'msle': MSLELoss()
-
-}
+"""Common losses"""
+
+import numpy as np
+try:
+    import cupy as cp
+    CUDA_FOUND = True
+except Exception:
+    CUDA_FOUND = False
+
+from .metrics import metric_alias, RMSEMetric, RMSLEMetric, BCEMetric
+from .multiclass_metrics import multiclass_metric_alias, CrossEntropyMetric
+
+
+class Loss:
+    """Base class to define loss function"""
+
+    def get_grad_hess(self, y_true, y_pred):
+        """Method implements how to calculate gradients and hessians.
+        Output gradient should have the shape (n_samples, n_outputs)
+        Output hessian should have the shape (n_samples, n_outputs) or (n_samples, 1)
+            if the same hess used for all outputs (for ex. MSELoss)
+
+        Definition don't use sample_weight, because it is applied later at the tree building stage
+
+        Args:
+            y_true: cp.ndarray, target
+            y_pred: cp.ndarray, current prediction
+
+        Returns:
+
+        """
+        raise NotImplementedError
+
+    def __call__(self, y_true, y_pred):
+        grad, hess = self.get_grad_hess(y_true, y_pred)
+        return grad, hess
+
+    def preprocess_input(self, y_true):
+        """Method defines how raw input target variable should be processed before train starts
+            (ex. applying log1p for MSLELoss)
+
+        Args:
+            y_true: cp.ndarray, raw target
+
+        Returns:
+
+        """
+        return y_true
+
+    def postprocess_output(self, y_pred):
+        """Method defines how to postprocess sum of trees to output prediction (ex. apply sigmoid for BCELoss)
+
+        Args:
+            y_pred: cp.ndarray, predictions
+
+        Returns:
+
+        """
+        return y_pred
+
+    def base_score(self, y_true):
+        """Method defines how to initialize an empty ensemble (ex. initialize with mean values for MSELoss)
+
+        Args:
+            y_true: cp.ndarray, processed target (after applying preprocess_input)
+
+        Returns:
+
+        """
+        raise NotImplementedError
+
+    def get_metric_from_string(self, name=None):
+        """Method defines how to interpret eval metric given in str format or None.
+        For ex. you can define the default metric to use here if name is None
+
+        Args:
+            name:
+
+        Returns:
+
+        """
+        return metric_alias['name']
+
+
+class MSELoss(Loss):
+    """MSE Loss function for regression/multiregression"""
+
+    def get_grad_hess(self, y_true, y_pred):
+        return (y_pred - y_true), cp.ones((y_true.shape[0], 1), dtype=cp.float32)
+
+    def base_score(self, y_true):
+        return y_true.mean(axis=0)
+
+    def get_metric_from_string(self, name=None):
+        if name is None:
+            return RMSEMetric()
+        return metric_alias[name]
+
+
+class MSLELoss(Loss):
+    """MSLE Loss function for regression/multiregression"""
+
+    def preprocess_input(self, y_true):
+        assert (y_true >= 0).all(), 'Inputs for msle should be non negative'
+
+        return y_true
+
+    def get_grad_hess(self, y_true, y_pred):
+        y_true = cp.log1p(y_true)
+
+        return (y_pred - y_true), cp.ones((y_true.shape[0], 1), dtype=cp.float32)
+
+    def postprocess_output(self, y_pred):
+        return cp.expm1(y_pred)
+
+    def base_score(self, y_true):
+        y_true = cp.log1p(y_true)
+        return y_true.mean(axis=0)
+
+    def get_metric_from_string(self, name=None):
+        if name is None:
+            return RMSLEMetric()
+        return metric_alias[name]
+
+
+class BCELoss(Loss):
+    """LogLoss for binary/multilabel classification"""
+
+    def __init__(self, clip_value=1e-7):
+        self.clip_value = clip_value
+
+    def base_score(self, y_true):
+        means = cp.clip(y_true.mean(axis=0), self.clip_value, 1 - self.clip_value)
+        return cp.log(means / (1 - means))
+
+    def get_grad_hess(self, y_true, y_pred):
+        pred = 1 / (1 + cp.exp(-y_pred))
+        pred = cp.clip(pred, self.clip_value, 1 - self.clip_value)
+        grad = pred - y_true
+        hess = pred * (1 - pred)
+
+        return grad, hess
+
+    def postprocess_output(self, y_pred):
+        xp = np if type(y_pred) is np.ndarray else cp
+        pred = 1 / (1 + xp.exp(-y_pred))
+        pred = xp.clip(pred, self.clip_value, 1 - self.clip_value)
+
+        return pred
+
+    def get_metric_from_string(self, name=None):
+        if name is None:
+            return BCEMetric()
+        return metric_alias[name]
+
+
+def softmax(x, clip_val=1e-5):
+    
+    xp = np if type(x) is np.ndarray else cp
+    exp_p = xp.exp(x - x.max(axis=1, keepdims=True))
+
+    return xp.clip(exp_p / exp_p.sum(axis=1, keepdims=True), clip_val, 1 - clip_val)
+
+
+# multiclass losses
+
+ce_grad_kernel = cp.ElementwiseKernel(
+    'T pred, raw S label, raw S nlabels, T factor',
+    'T grad, T hess',
+
+    """
+    int y_pr = i % nlabels;
+    int y_tr = label[i / nlabels];
+
+    grad = pred - (float) (y_pr == y_tr);
+    hess = pred * (1. - pred) * factor;
+
+    """,
+    "ce_grad_kernel"
+) if CUDA_FOUND else None
+
+
+def ce_grad(y_true, y_pred):
+    factor = y_pred.shape[1] / (y_pred.shape[1] - 1)
+    grad, hess = ce_grad_kernel(y_pred, y_true, y_pred.shape[1], factor)
+
+    return grad, hess
+
+
+class CrossEntropyLoss(Loss):
+    """CrossEntropy for multiclass classification"""
+
+    def __init__(self, clip_value=1e-6):
+        self.clip_value = clip_value
+
+    def base_score(self, y_true):
+        num_classes = int(y_true.max() + 1)
+        hist = cp.zeros((num_classes,), dtype=cp.float32)
+
+        return hist
+
+    def get_grad_hess(self, y_true, y_pred):
+        pred = softmax(y_pred, self.clip_value)
+        grad, hess = ce_grad(y_true, pred)
+        return grad, hess
+
+    def postprocess_output(self, y_pred):
+        
+        return softmax(y_pred, self.clip_value)
+
+    def preprocess_input(self, y_true):
+        return y_true[:, 0].astype(cp.int32)
+
+    def get_metric_from_string(self, name=None):
+        if name is None:
+            return CrossEntropyMetric()
+        return multiclass_metric_alias[name]
+
+
+loss_alias = {
+
+    # for bce
+    'binary': BCELoss(),
+    'bce': BCELoss(),
+    'multilabel': BCELoss(),
+    'logloss': BCELoss(),
+
+    # for multiclass
+    'multiclass': CrossEntropyLoss(),
+    'crossentropy': CrossEntropyLoss(),
+
+    # for regression
+    'mse': MSELoss(),
+    'regression': MSELoss(),
+    'l2': MSELoss(),
+    'multitask': MSELoss(),
+    'msle': MSLELoss()
+
+}
```

### Comparing `py_boost-0.4.3/py_boost/gpu/losses/metrics.py` & `py_boost-0.5.0/py_boost/gpu/losses/metrics.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,341 +1,341 @@
-"""Common metrics"""
-
-try:
-    import cupy as cp
-except Exception:
-    pass
-
-
-class Metric:
-    """Base class to define eval metric function.
-    Metric could be defined in 2 ways:
-
-        - redefine .error method. Preferred if possible. Simplified metric definition by calculating error function
-            for each point (ex. see RMSEMetric). If metric is defined via .error it also could be used with AdvancedES
-
-        - redefine __call__ method. Used for more complex functions, like ROC-AUC. Handling sample_weight
-            should be done manually here if needed
-
-
-    """
-    alias = 'score'  # defines how metric will be named in the output log
-
-    def error(self, y_true, y_pred):
-        """Simplified metric definition via individual objects error
-
-        Args:
-            y_true: cp.array, targets
-            y_pred: cp.array, predictions
-
-        Returns:
-            float, metric value
-        """
-        raise ValueError('Pointwise error is not implemented for this metric')
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        """Full metric definition. Default is just weighted aggregation of pointwise errors
-
-        Args:
-            y_true: cp.array, targets
-            y_pred: cp.array, predictions
-            sample_weight: None or cp.ndarray, weights
-
-        Returns:
-            float, metric value
-        """
-        err = self.error(y_true, y_pred)
-        shape = err.shape
-        assert shape[0] == y_true.shape[0], 'Error shape should match target shape at first dim'
-
-        if len(shape) == 1:
-            err = err[:, cp.newaxis]
-
-        if sample_weight is None:
-            return err.mean()
-
-        err = (err.mean(axis=1, keepdims=True) * sample_weight).sum() / sample_weight.sum()
-        return err
-
-    def compare(self, v0, v1):
-        """Method defines how to decide if metric was improved. Commonly it should be one of 'v0 > v1' or 'v0 < v1 '
-
-        Args:
-            v0: float, metric value
-            v1: float, metric value
-
-        Returns:
-            bool, if v0 improves score against v1
-        """
-        raise NotImplementedError
-
-    def argmax(self, arr):
-        """Select best metric from list of metrics based on .compare method
-
-        Args:
-            arr: list of float, metric values
-
-        Returns:
-            int, position of the best metric value
-        """
-        best = arr[0]
-        best_n = 0
-
-        for n, val in enumerate(arr[1:], 1):
-            if self.compare(val, best):
-                best = val
-                best_n = n
-
-        return best_n
-
-
-class RMSEMetric(Metric):
-    """RMSE Metric for the regression/multiregression task"""
-    alias = 'rmse'
-
-    def error(self, y_true, y_pred):
-        return (y_true - y_pred) ** 2
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        return super().__call__(y_true, y_pred, sample_weight) ** .5
-
-    def compare(self, v0, v1):
-        return v0 < v1
-
-
-class R2Score(RMSEMetric):
-    """R2 Score Metric for the regression/multiregression task"""
-    alias = 'R2_score'
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-
-        if sample_weight is not None:
-            err = ((y_true - y_pred) ** 2 * sample_weight).sum(axis=0) / sample_weight.sum()
-            std = ((y_true - y_true.mean(axis=0)) ** 2 * sample_weight).sum(axis=0) / sample_weight.sum()
-        else:
-            err = ((y_true - y_pred) ** 2).mean(axis=0)
-            std = y_true.var(axis=0)
-
-        return (1 - err / std).mean()
-
-    def compare(self, v0, v1):
-        return v0 > v1
-
-
-class RMSLEMetric(RMSEMetric):
-    """RMSLE Metric for the regression/multiregression classification task"""
-    alias = 'rmsle'
-
-    def error(self, y_true, y_pred):
-        return super().error(cp.log1p(y_true), cp.log1p(y_pred))
-
-
-class BCEMetric(Metric):
-    """LogLoss for the binary/multilabel classification task"""
-    alias = 'BCE'
-
-    def error(self, y_true, y_pred):
-        return -cp.log(y_true * y_pred + (1 - y_pred) * (1 - y_true))
-
-    def compare(self, v0, v1):
-        return v0 < v1
-
-
-def auc(y, x, sample_weight=None):
-    """Roc-auc score via cupy
-
-    Args:
-        y: cp.ndarray, 1d prediction
-        x: cp.ndarray, 1d binary target
-        sample_weight: optional 1d array of sample weights
-
-    Returns:
-        float, roc-auc metric value
-    """
-    unique_x = cp.unique(x)
-
-    if unique_x.shape[0] <= 1:
-        return 0.5
-
-    if sample_weight is None:
-        sample_weight = cp.ones_like(y)
-
-    rank_x = cp.searchsorted(unique_x, x)
-
-    sum_1 = cp.zeros_like(unique_x, dtype=cp.float64)
-    sum_1.scatter_add(rank_x, sample_weight * y)
-
-    sum_0 = cp.zeros_like(unique_x, dtype=cp.float64)
-    sum_0.scatter_add(rank_x, sample_weight * (1 - y))
-
-    cs_0 = sum_0.cumsum()
-    auc_ = (cs_0 - sum_0 / 2) * sum_1
-
-    tot = cs_0[-1] * sum_1.sum()
-
-    return float(auc_.sum() / tot)
-
-
-class RocAucMetric(Metric):
-    """Roc-auc metric for the binary classification task"""
-    alias = 'AUC'
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        """
-
-        Args:
-            y_true: cp.ndarray of targets
-            y_pred: cp.ndarray of predictions
-            sample_weight: None or cp.ndarray of sample_weights
-
-        Returns:
-
-        """
-        assert y_pred.shape[1] == 1, 'Multioutput is not supported'
-
-        if sample_weight is not None:
-            sample_weight = sample_weight[:, 0]
-
-        return auc(y_true[:, 0], y_pred[:, 0], sample_weight)
-
-    def compare(self, v0, v1):
-        return v0 > v1
-
-
-class ThresholdMetrics(Metric):
-    """Basic class to handle metrics, that accept class label prediction as input"""
-
-    def __init__(self, threshold=0.5, q=None):
-        """Define binarization rule. If quantile is given, threshold defined with quantile
-
-        Args:
-            threshold: float, threshold value
-            q: None or float, quantile threshold
-        """
-        self.threshold = threshold
-        self.q = q
-
-    def get_label(self, y_pred):
-        """Get labels from probabilities
-
-        Args:
-            y_pred: cp.ndarray, predictions
-
-        Returns:
-            cp.ndarray, predicted class labels
-        """
-        threshold = self.threshold
-        if self.q is not None:
-            threshold = cp.quantile(y_pred, self.q, axis=0, interpolation='higher')
-
-        return y_pred >= threshold
-
-    def get_stats(self, y_true, y_pred, sample_weight=None, mode='f1'):
-        """Helpful utils to calc Precision/Recall/F1
-
-        Args:
-            y_true: cp.ndarray, target
-            y_pred: cp.ndarray, predicted class label
-            sample_weight: None or cp.ndarray, weights
-            mode:
-
-        Returns:
-
-        """
-
-        y_pred = self.get_label(y_pred)
-        true = y_pred == y_true
-
-        tp = true * y_pred
-        if sample_weight is not None:
-            tp = tp * sample_weight
-        tp = tp.sum(axis=0)
-
-        if mode == 'p':
-            if sample_weight is not None:
-                return tp, (y_pred * sample_weight).sum(axis=0)
-            return tp, y_pred.sum(axis=0)
-
-        if sample_weight is not None:
-            tot = (y_true * sample_weight).sum(axis=0)
-        else:
-            tot = y_true.sum(axis=0)
-        if mode == 'r':
-            return tp, tot
-
-        if sample_weight is not None:
-            tot_p = (y_pred * sample_weight).sum(axis=0)
-        else:
-            tot_p = y_pred.sum(axis=0)
-
-        return tp, tot, tot_p
-
-    def compare(self, v0, v1):
-        return v0 > v1
-
-
-class AccuracyMetric(ThresholdMetrics):
-    """Accuracy Metric for the binary/multilabel classification task"""
-    alias = 'Accuracy'
-
-    def error(self, y_true, y_pred):
-        y_pred = self.get_label(y_pred)
-        return (y_true == y_pred).mean(axis=1)
-
-
-class Precision(ThresholdMetrics):
-    """Precision Metric for the binary/multilabel classification task"""
-    alias = 'Precision'
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        tp, tot = self.get_stats(y_true, y_pred, sample_weight, mode='p')
-        tot = cp.clip(tot, 1e-5, None)
-        return (tp / tot).mean()
-
-
-class Recall(ThresholdMetrics):
-    """Recall Metric for the binary/multilabel classification task"""
-    alias = 'Recall'
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        tp, tot = self.get_stats(y_true, y_pred, sample_weight, mode='r')
-        tot = cp.clip(tot, 1e-5, None)
-        return (tp / tot).mean()
-
-
-class F1Score(ThresholdMetrics):
-    """F1 Score Metric for the binary/multilabel classification task"""
-    alias = 'F1_score'
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        tp, tot, tot_p = self.get_stats(y_true, y_pred, sample_weight, mode='f1')
-        precision = tp / cp.clip(tot_p, 1e-5, None)
-        recall = tp / cp.clip(tot, 1e-5, None)
-
-        return (2 * (precision * recall) / cp.clip(precision + recall, 1e-5, None)).mean()
-
-
-metric_alias = {
-
-    # for bce
-    'bce': BCEMetric(),
-    'logloss': BCEMetric(),
-
-    'precision': Precision(),
-    'recall': Recall(),
-    'f1_score': F1Score(),
-    'f1': F1Score(),
-
-    'accuracy': AccuracyMetric(),
-    'acc': AccuracyMetric(),
-
-    'auc': RocAucMetric(),
-    'roc': RocAucMetric(),
-
-    # for regression
-    'rmse': RMSEMetric(),
-    'l2': RMSEMetric(),
-    'rmsle': RMSLEMetric(),
-    'r2': R2Score(),
-    'r2_score': R2Score(),
-
-}
+"""Common metrics"""
+
+try:
+    import cupy as cp
+except Exception:
+    pass
+
+
+class Metric:
+    """Base class to define eval metric function.
+    Metric could be defined in 2 ways:
+
+        - redefine .error method. Preferred if possible. Simplified metric definition by calculating error function
+            for each point (ex. see RMSEMetric). If metric is defined via .error it also could be used with AdvancedES
+
+        - redefine __call__ method. Used for more complex functions, like ROC-AUC. Handling sample_weight
+            should be done manually here if needed
+
+
+    """
+    alias = 'score'  # defines how metric will be named in the output log
+
+    def error(self, y_true, y_pred):
+        """Simplified metric definition via individual objects error
+
+        Args:
+            y_true: cp.array, targets
+            y_pred: cp.array, predictions
+
+        Returns:
+            float, metric value
+        """
+        raise ValueError('Pointwise error is not implemented for this metric')
+
+    def __call__(self, y_true, y_pred, sample_weight=None):
+        """Full metric definition. Default is just weighted aggregation of pointwise errors
+
+        Args:
+            y_true: cp.array, targets
+            y_pred: cp.array, predictions
+            sample_weight: None or cp.ndarray, weights
+
+        Returns:
+            float, metric value
+        """
+        err = self.error(y_true, y_pred)
+        shape = err.shape
+        assert shape[0] == y_true.shape[0], 'Error shape should match target shape at first dim'
+
+        if len(shape) == 1:
+            err = err[:, cp.newaxis]
+
+        if sample_weight is None:
+            return err.mean()
+
+        err = (err.mean(axis=1, keepdims=True) * sample_weight).sum() / sample_weight.sum()
+        return err
+
+    def compare(self, v0, v1):
+        """Method defines how to decide if metric was improved. Commonly it should be one of 'v0 > v1' or 'v0 < v1 '
+
+        Args:
+            v0: float, metric value
+            v1: float, metric value
+
+        Returns:
+            bool, if v0 improves score against v1
+        """
+        raise NotImplementedError
+
+    def argmax(self, arr):
+        """Select best metric from list of metrics based on .compare method
+
+        Args:
+            arr: list of float, metric values
+
+        Returns:
+            int, position of the best metric value
+        """
+        best = arr[0]
+        best_n = 0
+
+        for n, val in enumerate(arr[1:], 1):
+            if self.compare(val, best):
+                best = val
+                best_n = n
+
+        return best_n
+
+
+class RMSEMetric(Metric):
+    """RMSE Metric for the regression/multiregression task"""
+    alias = 'rmse'
+
+    def error(self, y_true, y_pred):
+        return (y_true - y_pred) ** 2
+
+    def __call__(self, y_true, y_pred, sample_weight=None):
+        return super().__call__(y_true, y_pred, sample_weight) ** .5
+
+    def compare(self, v0, v1):
+        return v0 < v1
+
+
+class R2Score(RMSEMetric):
+    """R2 Score Metric for the regression/multiregression task"""
+    alias = 'R2_score'
+
+    def __call__(self, y_true, y_pred, sample_weight=None):
+
+        if sample_weight is not None:
+            err = ((y_true - y_pred) ** 2 * sample_weight).sum(axis=0) / sample_weight.sum()
+            std = ((y_true - y_true.mean(axis=0)) ** 2 * sample_weight).sum(axis=0) / sample_weight.sum()
+        else:
+            err = ((y_true - y_pred) ** 2).mean(axis=0)
+            std = y_true.var(axis=0)
+
+        return (1 - err / std).mean()
+
+    def compare(self, v0, v1):
+        return v0 > v1
+
+
+class RMSLEMetric(RMSEMetric):
+    """RMSLE Metric for the regression/multiregression classification task"""
+    alias = 'rmsle'
+
+    def error(self, y_true, y_pred):
+        return super().error(cp.log1p(y_true), cp.log1p(y_pred))
+
+
+class BCEMetric(Metric):
+    """LogLoss for the binary/multilabel classification task"""
+    alias = 'BCE'
+
+    def error(self, y_true, y_pred):
+        return -cp.log(y_true * y_pred + (1 - y_pred) * (1 - y_true))
+
+    def compare(self, v0, v1):
+        return v0 < v1
+
+
+def auc(y, x, sample_weight=None):
+    """Roc-auc score via cupy
+
+    Args:
+        y: cp.ndarray, 1d prediction
+        x: cp.ndarray, 1d binary target
+        sample_weight: optional 1d array of sample weights
+
+    Returns:
+        float, roc-auc metric value
+    """
+    unique_x = cp.unique(x)
+
+    if unique_x.shape[0] <= 1:
+        return 0.5
+
+    if sample_weight is None:
+        sample_weight = cp.ones_like(y)
+
+    rank_x = cp.searchsorted(unique_x, x)
+
+    sum_1 = cp.zeros_like(unique_x, dtype=cp.float64)
+    sum_1.scatter_add(rank_x, sample_weight * y)
+
+    sum_0 = cp.zeros_like(unique_x, dtype=cp.float64)
+    sum_0.scatter_add(rank_x, sample_weight * (1 - y))
+
+    cs_0 = sum_0.cumsum()
+    auc_ = (cs_0 - sum_0 / 2) * sum_1
+
+    tot = cs_0[-1] * sum_1.sum()
+
+    return float(auc_.sum() / tot)
+
+
+class RocAucMetric(Metric):
+    """Roc-auc metric for the binary classification task"""
+    alias = 'AUC'
+
+    def __call__(self, y_true, y_pred, sample_weight=None):
+        """
+
+        Args:
+            y_true: cp.ndarray of targets
+            y_pred: cp.ndarray of predictions
+            sample_weight: None or cp.ndarray of sample_weights
+
+        Returns:
+
+        """
+        assert y_pred.shape[1] == 1, 'Multioutput is not supported'
+
+        if sample_weight is not None:
+            sample_weight = sample_weight[:, 0]
+
+        return auc(y_true[:, 0], y_pred[:, 0], sample_weight)
+
+    def compare(self, v0, v1):
+        return v0 > v1
+
+
+class ThresholdMetrics(Metric):
+    """Basic class to handle metrics, that accept class label prediction as input"""
+
+    def __init__(self, threshold=0.5, q=None):
+        """Define binarization rule. If quantile is given, threshold defined with quantile
+
+        Args:
+            threshold: float, threshold value
+            q: None or float, quantile threshold
+        """
+        self.threshold = threshold
+        self.q = q
+
+    def get_label(self, y_pred):
+        """Get labels from probabilities
+
+        Args:
+            y_pred: cp.ndarray, predictions
+
+        Returns:
+            cp.ndarray, predicted class labels
+        """
+        threshold = self.threshold
+        if self.q is not None:
+            threshold = cp.quantile(y_pred, self.q, axis=0, interpolation='higher')
+
+        return y_pred >= threshold
+
+    def get_stats(self, y_true, y_pred, sample_weight=None, mode='f1'):
+        """Helpful utils to calc Precision/Recall/F1
+
+        Args:
+            y_true: cp.ndarray, target
+            y_pred: cp.ndarray, predicted class label
+            sample_weight: None or cp.ndarray, weights
+            mode:
+
+        Returns:
+
+        """
+
+        y_pred = self.get_label(y_pred)
+        true = y_pred == y_true
+
+        tp = true * y_pred
+        if sample_weight is not None:
+            tp = tp * sample_weight
+        tp = tp.sum(axis=0)
+
+        if mode == 'p':
+            if sample_weight is not None:
+                return tp, (y_pred * sample_weight).sum(axis=0)
+            return tp, y_pred.sum(axis=0)
+
+        if sample_weight is not None:
+            tot = (y_true * sample_weight).sum(axis=0)
+        else:
+            tot = y_true.sum(axis=0)
+        if mode == 'r':
+            return tp, tot
+
+        if sample_weight is not None:
+            tot_p = (y_pred * sample_weight).sum(axis=0)
+        else:
+            tot_p = y_pred.sum(axis=0)
+
+        return tp, tot, tot_p
+
+    def compare(self, v0, v1):
+        return v0 > v1
+
+
+class AccuracyMetric(ThresholdMetrics):
+    """Accuracy Metric for the binary/multilabel classification task"""
+    alias = 'Accuracy'
+
+    def error(self, y_true, y_pred):
+        y_pred = self.get_label(y_pred)
+        return (y_true == y_pred).mean(axis=1)
+
+
+class Precision(ThresholdMetrics):
+    """Precision Metric for the binary/multilabel classification task"""
+    alias = 'Precision'
+
+    def __call__(self, y_true, y_pred, sample_weight=None):
+        tp, tot = self.get_stats(y_true, y_pred, sample_weight, mode='p')
+        tot = cp.clip(tot, 1e-5, None)
+        return (tp / tot).mean()
+
+
+class Recall(ThresholdMetrics):
+    """Recall Metric for the binary/multilabel classification task"""
+    alias = 'Recall'
+
+    def __call__(self, y_true, y_pred, sample_weight=None):
+        tp, tot = self.get_stats(y_true, y_pred, sample_weight, mode='r')
+        tot = cp.clip(tot, 1e-5, None)
+        return (tp / tot).mean()
+
+
+class F1Score(ThresholdMetrics):
+    """F1 Score Metric for the binary/multilabel classification task"""
+    alias = 'F1_score'
+
+    def __call__(self, y_true, y_pred, sample_weight=None):
+        tp, tot, tot_p = self.get_stats(y_true, y_pred, sample_weight, mode='f1')
+        precision = tp / cp.clip(tot_p, 1e-5, None)
+        recall = tp / cp.clip(tot, 1e-5, None)
+
+        return (2 * (precision * recall) / cp.clip(precision + recall, 1e-5, None)).mean()
+
+
+metric_alias = {
+
+    # for bce
+    'bce': BCEMetric(),
+    'logloss': BCEMetric(),
+
+    'precision': Precision(),
+    'recall': Recall(),
+    'f1_score': F1Score(),
+    'f1': F1Score(),
+
+    'accuracy': AccuracyMetric(),
+    'acc': AccuracyMetric(),
+
+    'auc': RocAucMetric(),
+    'roc': RocAucMetric(),
+
+    # for regression
+    'rmse': RMSEMetric(),
+    'l2': RMSEMetric(),
+    'rmsle': RMSLEMetric(),
+    'r2': R2Score(),
+    'r2_score': R2Score(),
+
+}
```

### Comparing `py_boost-0.4.3/py_boost/gpu/losses/multiclass_metrics.py` & `py_boost-0.5.0/py_boost/gpu/losses/multiclass_metrics.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-"""Common multiclass metrics"""
-
-try:
-    import cupy as cp
-except Exception:
-    pass
-
-from .metrics import Metric, metric_alias
-
-
-class CrossEntropyMetric(Metric):
-    """CrossEntropy Metric for the multiclassification task"""
-    alias = 'Crossentropy'
-
-    def error(self, y_true, y_pred):
-        return -cp.log(cp.take_along_axis(y_pred, y_true[:, cp.newaxis], axis=1))
-
-    def compare(self, v0, v1):
-        return v0 < v1
-
-
-class MultiAccuracyMetric(Metric):
-    """Accuracy Metric for the multiclassification task"""
-    alias = 'Accuracy'
-
-    def error(self, y_true, y_pred):
-        cl_pred = y_pred.argmax(axis=1)
-        return (cl_pred == y_true).astype(cp.float32)
-
-    def compare(self, v0, v1):
-        return v0 > v1
-
-
-class MultiMetric(Metric):
-    """Basic class to handle metrics, that accept class label prediction as input for the multiclassificationn task"""
-
-    def __init__(self, average='macro'):
-        """
-
-        Args:
-            average: str, one of 'micro' / 'macro'
-        """
-        self.average = average
-
-    @staticmethod
-    def get_stats(y_true, y_pred, sample_weight=None, mode='f1'):
-        """Helpful utils to calc Precision/Recall/F1
-
-        Args:
-            y_true: cp.ndarray, target
-            y_pred: cp.ndarray, predicted class label
-            sample_weight: None or cp.ndarray, weights
-            mode:
-
-        Returns:
-
-        """
-
-        if sample_weight is None:
-            sample_weight = cp.ones(y_true.shape, dtype=cp.float32)
-        else:
-            sample_weight = sample_weight[:, 0]
-
-        cl_pred = y_pred.argmax(axis=1)
-        true = y_true == cl_pred
-
-        tp = cp.zeros(y_pred.shape[1], dtype=cp.float64)
-        tp.scatter_add(cl_pred, true * sample_weight)
-
-        tot = cp.zeros(y_pred.shape[1], dtype=cp.float64)
-        if mode == 'p':
-            tot.scatter_add(cl_pred, sample_weight)
-            return tp, tot
-
-        tot.scatter_add(y_true, sample_weight)
-        if mode == 'r':
-            return tp, tot
-
-        tot_p = cp.zeros(y_pred.shape[1], dtype=cp.float64)
-        tot_p.scatter_add(cl_pred, sample_weight)
-
-        return tp, tot, tot_p
-
-    def get_metric(self, tp, tot):
-
-        tot = cp.clip(tot, 1e-5, None)
-
-        if self.average == 'micro':
-            return float(tp.sum() / tot.sum())
-
-        return float((tp / tot).mean())
-
-    def compare(self, v0, v1):
-        return v0 > v1
-
-
-class MultiPrecision(MultiMetric):
-    """Precision Metric for the multiclassification classification task"""
-    alias = 'Precision'
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        tp, tot = self.get_stats(y_true, y_pred, sample_weight=sample_weight, mode='p')
-        return self.get_metric(tp, tot)
-
-
-class MultiRecall(MultiMetric):
-    """Recall Metric for the multiclassification classification task"""
-    alias = 'Recall'
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        tp, tot = self.get_stats(y_true, y_pred, sample_weight=sample_weight, mode='r')
-        return self.get_metric(tp, tot)
-
-
-class MultiF1Score(MultiMetric):
-    """F1 Score Metric for the multiclassification classification task"""
-    alias = 'F1_score'
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        tp, tot, tot_p = self.get_stats(y_true, y_pred, sample_weight=sample_weight, mode='f1')
-        precision = self.get_metric(tp, tot_p)
-        recall = self.get_metric(tp, tot)
-        return 2 * (precision * recall) / (precision + recall)
-
-
-multiclass_metric_alias = {**metric_alias, **{
-
-    'crossentropy': CrossEntropyMetric(),
-
-    'precision': MultiPrecision(),
-    'recall': MultiRecall(),
-    'f1_score': MultiF1Score(),
-    'f1': MultiF1Score(),
-
-    'accuracy': MultiAccuracyMetric(),
-    'acc': MultiAccuracyMetric(),
-
-}}
+"""Common multiclass metrics"""
+
+try:
+    import cupy as cp
+except Exception:
+    pass
+
+from .metrics import Metric, metric_alias
+
+
+class CrossEntropyMetric(Metric):
+    """CrossEntropy Metric for the multiclassification task"""
+    alias = 'Crossentropy'
+
+    def error(self, y_true, y_pred):
+        return -cp.log(cp.take_along_axis(y_pred, y_true[:, cp.newaxis], axis=1))
+
+    def compare(self, v0, v1):
+        return v0 < v1
+
+
+class MultiAccuracyMetric(Metric):
+    """Accuracy Metric for the multiclassification task"""
+    alias = 'Accuracy'
+
+    def error(self, y_true, y_pred):
+        cl_pred = y_pred.argmax(axis=1)
+        return (cl_pred == y_true).astype(cp.float32)
+
+    def compare(self, v0, v1):
+        return v0 > v1
+
+
+class MultiMetric(Metric):
+    """Basic class to handle metrics, that accept class label prediction as input for the multiclassificationn task"""
+
+    def __init__(self, average='macro'):
+        """
+
+        Args:
+            average: str, one of 'micro' / 'macro'
+        """
+        self.average = average
+
+    @staticmethod
+    def get_stats(y_true, y_pred, sample_weight=None, mode='f1'):
+        """Helpful utils to calc Precision/Recall/F1
+
+        Args:
+            y_true: cp.ndarray, target
+            y_pred: cp.ndarray, predicted class label
+            sample_weight: None or cp.ndarray, weights
+            mode:
+
+        Returns:
+
+        """
+
+        if sample_weight is None:
+            sample_weight = cp.ones(y_true.shape, dtype=cp.float32)
+        else:
+            sample_weight = sample_weight[:, 0]
+
+        cl_pred = y_pred.argmax(axis=1)
+        true = y_true == cl_pred
+
+        tp = cp.zeros(y_pred.shape[1], dtype=cp.float64)
+        tp.scatter_add(cl_pred, true * sample_weight)
+
+        tot = cp.zeros(y_pred.shape[1], dtype=cp.float64)
+        if mode == 'p':
+            tot.scatter_add(cl_pred, sample_weight)
+            return tp, tot
+
+        tot.scatter_add(y_true, sample_weight)
+        if mode == 'r':
+            return tp, tot
+
+        tot_p = cp.zeros(y_pred.shape[1], dtype=cp.float64)
+        tot_p.scatter_add(cl_pred, sample_weight)
+
+        return tp, tot, tot_p
+
+    def get_metric(self, tp, tot):
+
+        tot = cp.clip(tot, 1e-5, None)
+
+        if self.average == 'micro':
+            return float(tp.sum() / tot.sum())
+
+        return float((tp / tot).mean())
+
+    def compare(self, v0, v1):
+        return v0 > v1
+
+
+class MultiPrecision(MultiMetric):
+    """Precision Metric for the multiclassification classification task"""
+    alias = 'Precision'
+
+    def __call__(self, y_true, y_pred, sample_weight=None):
+        tp, tot = self.get_stats(y_true, y_pred, sample_weight=sample_weight, mode='p')
+        return self.get_metric(tp, tot)
+
+
+class MultiRecall(MultiMetric):
+    """Recall Metric for the multiclassification classification task"""
+    alias = 'Recall'
+
+    def __call__(self, y_true, y_pred, sample_weight=None):
+        tp, tot = self.get_stats(y_true, y_pred, sample_weight=sample_weight, mode='r')
+        return self.get_metric(tp, tot)
+
+
+class MultiF1Score(MultiMetric):
+    """F1 Score Metric for the multiclassification classification task"""
+    alias = 'F1_score'
+
+    def __call__(self, y_true, y_pred, sample_weight=None):
+        tp, tot, tot_p = self.get_stats(y_true, y_pred, sample_weight=sample_weight, mode='f1')
+        precision = self.get_metric(tp, tot_p)
+        recall = self.get_metric(tp, tot)
+        return 2 * (precision * recall) / (precision + recall)
+
+
+multiclass_metric_alias = {**metric_alias, **{
+
+    'crossentropy': CrossEntropyMetric(),
+
+    'precision': MultiPrecision(),
+    'recall': MultiRecall(),
+    'f1_score': MultiF1Score(),
+    'f1': MultiF1Score(),
+
+    'accuracy': MultiAccuracyMetric(),
+    'acc': MultiAccuracyMetric(),
+
+}}
```

### Comparing `py_boost-0.4.3/py_boost/gpu/sketch_boost.py` & `py_boost-0.5.0/py_boost/gpu/sketch_boost.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-"""Implements SketchBoost for multioutput class"""
-
-from .boosting import GradientBoosting
-from ..multioutput.sketching import FilterSketch, TopOutputsSketch, SVDSketch, RandomSamplingSketch, \
-    RandomProjectionSketch
-
-
-class SketchBoost(GradientBoosting):
-    """
-    Gradient Boosting with built-in FilterSketch to handle multioutput tasks. If single output is passed,
-    it is handled as usual
-    """
-
-    def __init__(self, loss,
-                 metric=None,
-                 ntrees=100,
-                 lr=0.05,
-                 min_gain_to_split=0,
-                 lambda_l2=1,
-                 gd_steps=1,
-                 max_depth=6,
-                 min_data_in_leaf=10,
-                 colsample=1.,
-                 subsample=1.,
-
-                 quantization='Quantile',
-                 quant_sample=2000000,
-                 max_bin=256,
-                 min_data_in_bin=3,
-
-                 es=100,
-                 seed=42,
-                 verbose=10,
-
-                 sketch_outputs=1,
-                 sketch_method='proj',
-                 use_hess=False,
-
-                 callbacks=None,
-                 sketch_params=None
-                 ):
-        """
-
-        Args:
-            loss: str or Loss, loss function
-            metric: None or str or Metric, metric
-            ntrees: int, maximum number of trees
-            lr: float, learning rate
-            min_gain_to_split: float >=0, minimal gain to split
-            lambda_l2: float > 0, l2 leaf regularization
-            gd_steps: int > 0, number of gradient steps
-            max_depth: int > 0, maximum tree depth. Setting it to large values (>12) may cause OOM for wide datasets
-            min_data_in_leaf: int, minimal leaf size. Note - for some loss fn leaf size is approximated
-                with hessian values to speed up training
-            colsample: float or Callable, sumsample of columns to construct trees or callable - custom sampling
-            subsample: float or Callable, sumsample of rows to construct trees or callable - custom sampling
-
-            quantization: str or Quantizer, method for quantizatrion. One of 'Quantile', 'Uniform',
-                'Uniquant' or custom implementation
-            quant_sample: int, subsample to quantize features
-            max_bin: int in [2, 256] maximum number of bins to quantize features
-            min_data_in_bin: int in [2, 256] minimal bin size. NOTE: currently ignored
-
-            es: int, early stopping rounds. If 0, no early stopping
-            seed: int, random state
-            verbose: int, verbosity freq
-            sketch_outputs: int, number of outputs to keep
-            sketch_method: str, name of the sketching strategy
-            use_hess: bool, use hessians in multioutput training
-            callbacks: list of Callback, callbacks to customize training are passed here
-            sketch_params: dict, optional kwargs for sketching strategy
-        """
-        if sketch_params is None:
-            sketch_params = {}
-
-        if sketch_method == 'filter':
-            sketch = FilterSketch(sketch_outputs, **sketch_params)
-
-        elif sketch_method == 'svd':
-            sketch = SVDSketch(sketch_outputs, **sketch_params)
-
-        elif sketch_method == 'topk':
-            sketch = TopOutputsSketch(sketch_outputs)
-
-        elif sketch_method == 'rand':
-            sketch = RandomSamplingSketch(sketch_outputs, **sketch_params)
-
-        elif sketch_method == 'proj':
-            sketch = RandomProjectionSketch(sketch_outputs, **sketch_params)
-
-        elif sketch_method is None:
-            sketch = None
-
-        else:
-            raise ValueError('Unknown sketching strategy')
-
-        super().__init__(loss=loss,
-                         metric=metric,
-                         ntrees=ntrees,
-                         lr=lr,
-                         min_gain_to_split=min_gain_to_split,
-                         lambda_l2=lambda_l2,
-                         gd_steps=gd_steps,
-                         max_depth=max_depth,
-                         min_data_in_leaf=min_data_in_leaf,
-                         colsample=colsample,
-                         subsample=subsample,
-
-                         quantization=quantization,
-                         quant_sample=quant_sample,
-                         max_bin=max_bin,
-                         min_data_in_bin=min_data_in_bin,
-
-                         target_splitter='Single',
-                         multioutput_sketch=sketch,
-                         use_hess=use_hess,
-                         es=es,
-                         seed=seed,
-                         verbose=verbose,
-                         callbacks=callbacks)
+"""Implements SketchBoost for multioutput class"""
+
+from .boosting import GradientBoosting
+from ..multioutput.sketching import FilterSketch, TopOutputsSketch, SVDSketch, RandomSamplingSketch, \
+    RandomProjectionSketch
+
+
+class SketchBoost(GradientBoosting):
+    """
+    Gradient Boosting with built-in FilterSketch to handle multioutput tasks. If single output is passed,
+    it is handled as usual
+    """
+
+    def __init__(self, loss,
+                 metric=None,
+                 ntrees=100,
+                 lr=0.05,
+                 min_gain_to_split=0,
+                 lambda_l2=1,
+                 gd_steps=1,
+                 max_depth=6,
+                 min_data_in_leaf=10,
+                 colsample=1.,
+                 subsample=1.,
+
+                 quantization='Quantile',
+                 quant_sample=2000000,
+                 max_bin=256,
+                 min_data_in_bin=3,
+
+                 es=100,
+                 seed=42,
+                 verbose=10,
+
+                 sketch_outputs=1,
+                 sketch_method='proj',
+                 use_hess=False,
+
+                 callbacks=None,
+                 sketch_params=None
+                 ):
+        """
+
+        Args:
+            loss: str or Loss, loss function
+            metric: None or str or Metric, metric
+            ntrees: int, maximum number of trees
+            lr: float, learning rate
+            min_gain_to_split: float >=0, minimal gain to split
+            lambda_l2: float > 0, l2 leaf regularization
+            gd_steps: int > 0, number of gradient steps
+            max_depth: int > 0, maximum tree depth. Setting it to large values (>12) may cause OOM for wide datasets
+            min_data_in_leaf: int, minimal leaf size. Note - for some loss fn leaf size is approximated
+                with hessian values to speed up training
+            colsample: float or Callable, sumsample of columns to construct trees or callable - custom sampling
+            subsample: float or Callable, sumsample of rows to construct trees or callable - custom sampling
+
+            quantization: str or Quantizer, method for quantizatrion. One of 'Quantile', 'Uniform',
+                'Uniquant' or custom implementation
+            quant_sample: int, subsample to quantize features
+            max_bin: int in [2, 256] maximum number of bins to quantize features
+            min_data_in_bin: int in [2, 256] minimal bin size. NOTE: currently ignored
+
+            es: int, early stopping rounds. If 0, no early stopping
+            seed: int, random state
+            verbose: int, verbosity freq
+            sketch_outputs: int, number of outputs to keep
+            sketch_method: str, name of the sketching strategy
+            use_hess: bool, use hessians in multioutput training
+            callbacks: list of Callback, callbacks to customize training are passed here
+            sketch_params: dict, optional kwargs for sketching strategy
+        """
+        if sketch_params is None:
+            sketch_params = {}
+
+        if sketch_method == 'filter':
+            sketch = FilterSketch(sketch_outputs, **sketch_params)
+
+        elif sketch_method == 'svd':
+            sketch = SVDSketch(sketch_outputs, **sketch_params)
+
+        elif sketch_method == 'topk':
+            sketch = TopOutputsSketch(sketch_outputs)
+
+        elif sketch_method == 'rand':
+            sketch = RandomSamplingSketch(sketch_outputs, **sketch_params)
+
+        elif sketch_method == 'proj':
+            sketch = RandomProjectionSketch(sketch_outputs, **sketch_params)
+
+        elif sketch_method is None:
+            sketch = None
+
+        else:
+            raise ValueError('Unknown sketching strategy')
+
+        super().__init__(loss=loss,
+                         metric=metric,
+                         ntrees=ntrees,
+                         lr=lr,
+                         min_gain_to_split=min_gain_to_split,
+                         lambda_l2=lambda_l2,
+                         gd_steps=gd_steps,
+                         max_depth=max_depth,
+                         min_data_in_leaf=min_data_in_leaf,
+                         colsample=colsample,
+                         subsample=subsample,
+
+                         quantization=quantization,
+                         quant_sample=quant_sample,
+                         max_bin=max_bin,
+                         min_data_in_bin=min_data_in_bin,
+
+                         target_splitter='Single',
+                         multioutput_sketch=sketch,
+                         use_hess=use_hess,
+                         es=es,
+                         seed=seed,
+                         verbose=verbose,
+                         callbacks=callbacks)
```

### Comparing `py_boost-0.4.3/py_boost/gpu/tree.py` & `py_boost-0.5.0/py_boost/gpu/tree.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,581 +1,581 @@
-"""Decision trees building and inference"""
-
-try:
-    import cupy as cp
-except Exception:
-    pass
-import numpy as np
-
-from .utils import apply_values, depthwise_grow_tree, get_tree_node, set_leaf_values, calc_node_values
-from .utils import tree_prediction_leaves_typed_kernels, tree_prediction_leaves_typed_kernels_f
-from .utils import tree_prediction_values_kernel
-
-
-class Tree:
-    """This class initializes an empty tree structure, implements methods to set tree values and single tree inference.
-    The instance of this object represents the actual boosting step, but not the single tree!
-    Actual amount of trees in the instance (at each boosting step) is defined by ngroups argument. What it means:
-    Assume you have 5 class classification task, so you model output size equals 5. Possible cases here:
-        - Build single decision tree that outputs a vector of 5 values. In this case ngroups eq. 1
-        - Build 5 decision trees, each tree predict a value for its own class (one-vs-all).
-            In this case ngroups eq. 5
-        - Create custom target split strategy. For ex. you can build 2 trees, first will predict [0, 1, 2] classes,
-            second - [3, 4]. In this case ngroups eq. 2
-
-    Grouped trees structure is defined by arrays:
-        feats, shape (ngroups, max_nodes) - feature index to use for the split in each group/node.
-            If -1, the node is terminal (leaf)
-        val_splits, shape (ngroups, max_nodes) - threshold to compare when choosing the next node
-            if feature value is not NaN
-        nans, shape (ngroups, max_nodes) - bool values, if True, NaN feature values objects moves left, else - right
-        split, shape (ngroups, max_nodes, 2) - node indices corresponding left/right split for the current node
-
-    Trees structure defines single node id value for each object
-    Values assigned to the outputs are defined by arrays:
-        group_index, shape (nout, ). Defines the group id for predicting each output
-        values, shape (max_nodes, nout). Define output value for each node/output
-        leaves, shape (max_leaves, ngroups). Assigns the leaf index to the terminal nodes
-
-    During the fit stage, the format described above is used.
-    After fitting, additional reformatting occurs that converts the tree to another format to achieve faster inference:
-    - Sub-trees for each group are stored in one array named "test_format":
-        [gr0_node0, ..., gr0_nodeN, gr1_node0, ..., gr1_nodeM, gr2_node0, ..., gr2_nodeK, gr3_node0, ...]
-    - Each node in new formatted tree consists of 4 fields:
-        [feature_index, split_value, left_node_index, right_node_index],
-        feature_index - feature index to use for the split in each node.
-        split_value - threshold to compare when choosing the next node if feature value is not NaN
-        left_node_index - index of the left child in "test_format" array
-        right_node_index - index of the right child in "test_format" array
-    - The size of "test_format" array equals to the sum of all nodes in all subtrees except leaves multiplied by 4.
-        Multiplication by 4 occurs because each node consists of the 4 fields described above.
-        Examples:
-            test_format[0 * 4] == test_format[0] - yields feature_index for node with index 0.
-            test_format[0 * 4 + 1] == test_format[1] - yields split_value for node with index 0.
-            test_format[0 * 4 + 2] == test_format[2] - yields left_node_index for node with index 0.
-            test_format[0 * 4 + 3] == test_format[3] - yields right_node_index for node with index 0.
-            test_format[1 * 4] == test_format[4]  - yields feature_index for node with index 1.
-            test_format[1 * 4 + 1] == test_format[5] - yields split_value for node with index 1.
-            test_format[1 * 4 + 2] == test_format[6] - yields left_node_index for node with index 1.
-            test_format[1 * 4 + 3] == test_format[7] - yields right_node_index for node with index 1.
-            test_format[2 * 4] == test_format[8]  - yields feature_index for node with index 2.
-            ...
-            test_format[79 * 4] == test_format[316]  - yields feature_index for node with index 79.
-            test_format[79 * 4 + 1] == test_format[317] - yields split_value for node with index 79.
-            test_format[79 * 4 + 2] == test_format[318] - yields left_node_index for node with index 79.
-            test_format[79 * 4 + 3] == test_format[319] - yields right_node_index for node with index 79.
-            ...
-    - The sign of the feature_index value shows the behavior in case of feature == NaN (split to the left/right),
-        to the value written in feature_index an extra "1" is added to deal with zero.
-        Examples:
-            feature_index == 8, positive value means that tree follows to the left in case of NaN in feature,
-                the real feature index is calculated as follows: abs(8) - 1 = 7.
-            feature_index == -19, negative value means that tree follows to the right in case of NaN in feature,
-                the real feature index is calculated as follows: abs(-19) - 1 = 18.
-            feature_index == 0, impossible due to construction algorithm.
-    - If left_node_index/right_node_index is negative, it means that it shows index in the values array;
-        In case of a negative value, an extra "1" is added to deal with zero.
-        Examples:
-            left_node_index == 8, non-negative value means that left child node is stored in "test_format" with index 8;
-            left_node_index == -13, means that left child is a leaf, the index in "values" array for that leaf can
-                be calculated as follows: abs(-13) - 1 = 12. Thus, index in "values" array is 12.
-    - All subtrees are stored in one array, so an additional array of indexes where each subtree is starting
-        is required (index of the subtree roots), array "gr_subtree_offsets" stores these indexes,
-        size of "gr_subtree_offsets" equals to number of groups in the tree (number of subtrees).
-        Example:
-            gr_subtree_offsets == [0, 56, 183], means that tree has 3 subtrees (3 groups).
-            The first subtree has its root as node with index 0;
-            The second subtree has its root as node with index 56;
-            The third subtree has its root as node with index 183.
-            Example how to access the values of the root node in the second subtree:
-                test_format[56 * 4] == test_format[224]  - yields feature_index for the root of the second subtree;
-                test_format[56 * 4 + 1] == test_format[225] - yields split_value for the root of the second subtree;
-                test_format[56 * 4 + 2] == test_format[226] - yields left_node_index for the root of the second subtree;
-                test_format[56 * 4 + 3] == test_format[227] - yields right_node_index for the root of the second subtree
-    - Two fields, 'feature_importance_gain' and 'feature_importance_split', store feature importance arrays
-        and describe the fitted tree accordingly.
-    """
-
-    def __init__(self, max_nodes, nout, ngroups):
-        """Initialize empty tree
-
-        Args:
-            max_nodes: int, maximum number of nodes in tree
-            nout: int, number of outputs in tree
-            ngroups: int, number of groups
-        """
-        self.nout = nout
-        self.ngroups = ngroups
-        self.max_nodes = max_nodes
-
-        self.gains = np.zeros((ngroups, max_nodes,), dtype=np.float32)
-        self.feats = np.zeros((ngroups, max_nodes,), dtype=np.int64) - 1
-        self.bin_splits = np.zeros((ngroups, max_nodes,), dtype=np.int32)
-        self.nans = np.zeros((ngroups, max_nodes,), dtype=np.bool_)
-
-        self.split = np.zeros((ngroups, max_nodes, 2), dtype=np.int32)
-
-        self.val_splits = None
-        self.values = None
-        self.group_index = None
-        self.leaves = None
-        self.max_leaves = None
-
-        self.feature_importance_gain = None
-        self.feature_importance_split = None
-
-        self._debug = None
-        self.test_format = None
-        self.test_format_offsets = None
-
-    def set_nodes(self, group, unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left):
-        """Write info about new nodes
-
-        Args:
-            group: int, group id to write
-            unique_nodes: np.ndarray, nodes id to set info
-            new_nodes_id: np.ndarray, nodes id to left/right split current node
-            best_feat: np.ndarray, feature value to perform a split
-            best_gain: np.ndarray, gain from the split
-            best_split: np.ndarray, quantized threshold to compare when split
-            best_nan_left: np.ndarray, bool if True, nans moved in the left node, else right
-
-        Returns:
-
-        """
-
-        self.gains[group, unique_nodes] = best_gain
-        self.feats[group, unique_nodes] = best_feat
-        self.bin_splits[group, unique_nodes] = best_split
-        self.nans[group, unique_nodes] = best_nan_left
-        self.split[group, unique_nodes] = new_nodes_id
-
-    def set_node_values(self, values, group_index):
-        """Assign output values for each nodes
-
-        Args:
-            values: np.ndarray, node values
-            group_index: np.ndarray, group id of each output
-
-        Returns:
-
-        """
-        self.values = values
-        self.group_index = group_index
-
-    def set_borders(self, borders):
-        """Assign actual feature values based on quantized
-
-        Args:
-            borders: list of np.ndarray, actual node values
-
-        Returns:
-
-        """
-        # borders - list of arrays. Array is borderlines
-        val_splits = [0 if x == -1 else borders[x][min(y, len(borders[x]) - 1)]
-                      for (x, y) in zip(self.feats.ravel(), self.bin_splits.ravel())]
-        self.val_splits = np.array(val_splits, dtype=np.float32).reshape(self.feats.shape)
-
-    def set_leaves(self):
-        """Assign leaf id to the terminal nodes
-
-        Returns:
-
-        """
-        self.leaves, self.max_leaves = set_leaf_values(self.feats, self.split)
-
-    def to_device(self):
-        """Move tree data to the current GPU memory
-
-        Returns:
-
-        """
-        for attr in ['gains', 'feats', 'bin_splits', 'nans', 'split', 'val_splits', 'values', 'group_index', 'leaves',
-                     'test_format', 'test_format_offsets', 'feature_importance_gain', 'feature_importance_split']:
-            arr = getattr(self, attr)
-
-            if type(arr) is np.ndarray:
-                setattr(self, attr, cp.asarray(arr))
-
-    def to_cpu(self):
-        """Move tree data to the CPU memory
-
-        Returns:
-
-        """
-        for attr in ['gains', 'feats', 'bin_splits', 'nans', 'split', 'val_splits', 'values', 'group_index', 'leaves',
-                     'test_format', 'test_format_offsets', 'feature_importance_gain', 'feature_importance_split']:
-            arr = getattr(self, attr)
-
-            if type(arr) is cp.ndarray:
-                setattr(self, attr, arr.get())
-
-    def _predict_node_deprecated(self, X):
-        """(DEPRECATED) Predict node id from the feature matrix X
-
-        Args:
-            X: cp.ndarray of features
-
-        Returns:
-
-        """
-        if self.feats is None:
-            raise Exception('To use _deprecated funcs pass debug=True to .reformat')
-
-        assert type(self.feats) is cp.ndarray, 'Should be moved to GPU first. Call .to_device()'
-        nodes = get_tree_node(X, self.feats, self.val_splits, self.split, self.nans)
-        return nodes
-
-    def _predict_from_nodes_deprecated(self, nodes):
-        """(DEPRECATED) Predict outputs from the nodes indices
-
-        Args:
-            nodes: cp.ndarray of predicted nodes
-
-        Returns:
-            cp.ndarray of nodes
-        """
-        return apply_values(nodes, self.group_index, self.values)
-
-    def _predict_leaf_from_nodes_deprecated(self, nodes):
-        """Predict leaf indices from the nodes indices (Use predict_leaf() method if you need to predict leaves)
-
-        Args:
-            nodes: cp.ndarray of predicted nodes
-
-        Returns:
-            cp.ndarray of leaves
-        """
-        return apply_values(nodes, cp.arange(self.ngroups, dtype=cp.uint64), self.leaves)
-
-    def _predict_deprecated(self, X):
-        """(DEPRECATED) Predict from the feature matrix X
-
-        Args:
-            X: cp.ndarray of features
-
-        Returns:
-            cp.ndarray of predictions
-        """
-        return self._predict_from_nodes_deprecated(
-            self._predict_leaf_from_nodes_deprecated(self._predict_node_deprecated(X)))
-
-    def _predict_leaf_deprecated(self, X):
-        """(DEPRECATED) Predict leaf indices from the feature matrix X
-
-        Args:
-            X: cp.ndarray of features
-
-        Returns:
-            cp.ndarray of leaves
-        """
-        return self._predict_leaf_from_nodes_deprecated(self._predict_node_deprecated(X))
-
-    def predict_leaf(self, X, pred_leaves=None):
-        """Predict leaf indexes from the feature matrix X
-
-        Args:
-            X: cp.ndarray, array of features
-            pred_leaves: cp.ndarray, buffer for predictions
-
-        Returns:
-            pred_leaves: leaf predictions
-
-        """
-        # check if buffer is None and X on GPU
-        assert type(X) is cp.ndarray, "X must be type of cp.ndarray (located on gpu)"
-
-        dt = str(X.dtype)
-
-        assert dt in tree_prediction_leaves_typed_kernels, \
-            f"X array must be of type: {list(tree_prediction_leaves_typed_kernels.keys())}"
-
-        if pred_leaves is None:
-            pred_leaves = cp.empty((X.shape[0], self.ngroups), dtype=cp.int32)
-
-        # CUDA parameters initialization
-        threads = 128  # threads in one CUDA block
-        sz = X.shape[0] * self.ngroups
-        blocks = sz // threads
-        if sz % threads != 0:
-            blocks += 1
-
-        if X.flags["C_CONTIGUOUS"]:
-            tree_prediction_leaves_typed_kernels[dt]((blocks,), (threads,), ((X,
-                                                                              self.test_format,
-                                                                              self.test_format_offsets,
-                                                                              X.shape[1],
-                                                                              X.shape[0],
-                                                                              self.ngroups,
-                                                                              pred_leaves.shape[1],
-                                                                              pred_leaves)))
-        elif X.flags["F_CONTIGUOUS"]:
-            tree_prediction_leaves_typed_kernels_f[dt]((blocks,), (threads,), ((X,
-                                                                                self.test_format,
-                                                                                self.test_format_offsets,
-                                                                                X.shape[1],
-                                                                                X.shape[0],
-                                                                                self.ngroups,
-                                                                                pred_leaves.shape[1],
-                                                                                pred_leaves)))
-        else:
-            raise Exception("X must be 'C_CONTIGUOUS' or 'F_CONTIGUOUS'")
-        return pred_leaves
-
-    def predict(self, X, pred=None, pred_leaves=None):
-        """Predict from the feature matrix X
-
-        Args:
-            X: cp.ndarray, array of features
-            pred: cp.ndarray, buffer for predictions on GPU, if None - created automatically
-            pred_leaves: cp.ndarray, buffer for internal leaf predictions on GPU, if None - created automatically
-
-        Returns:
-            pred: cp.ndarray, prediction array
-
-        """
-        # check if buffers are None
-        if pred is None:
-            pred = cp.zeros((X.shape[0], self.nout), dtype=cp.float32)
-        if pred_leaves is None:
-            pred_leaves = cp.empty((X.shape[0], self.ngroups), dtype=cp.int32)
-
-        # first step - leaves predictions, actually prediction of indexes in values
-        self.predict_leaf(X, pred_leaves)
-
-        # CUDA parameters initialization
-        threads = 128  # threads in one CUDA block
-        sz = X.shape[0] * self.nout
-        blocks = sz // threads
-        if sz % threads != 0:
-            blocks += 1
-
-        # second step, prediction of actual values
-        tree_prediction_values_kernel((blocks,), (threads,), ((pred_leaves,
-                                                               self.group_index,
-                                                               self.values,
-                                                               self.nout,
-                                                               X.shape[0],
-                                                               pred_leaves.shape[1],
-                                                               pred)))
-        return pred
-
-    def reformat(self, nfeats, debug):
-        """Creates new internal format of the tree for faster inference
-        
-        Args:
-            nfeats: int, number of features in X (train set)
-            debug: bool, if in debug mode
-
-        Returns:
-
-        """
-        n_gr = self.ngroups
-
-        # memory allocation for new tree array
-        gr_subtree_offsets = np.zeros(n_gr, dtype=np.int32)
-        check_empty = []
-        total_size = 0
-        for i in range(n_gr):
-            curr_size = int((self.feats[i] >= 0).sum())
-            # add special case handling - single leaf, no splits
-            check_empty.append(curr_size == 0)
-            curr_size = max(1, curr_size)
-            total_size += curr_size
-
-            if i < n_gr - 1:
-                gr_subtree_offsets[i + 1] = total_size
-        nf = np.zeros(total_size * 4, dtype=np.float32)
-
-        # reformatting the tree
-        for i in range(n_gr):
-            # handle special case - single leaf, no splits - make a pseudo split node
-            if check_empty[i]:
-                nf[4 * gr_subtree_offsets[i]] = 1.
-                nf[4 * gr_subtree_offsets[i] + 1] = 0.
-                nf[4 * gr_subtree_offsets[i] + 2] = -1.
-                nf[4 * gr_subtree_offsets[i] + 3] = -1.
-
-                continue
-
-            q = [(0, 0)]
-
-            while len(q) != 0:  # BFS in tree
-                n_old, n_new = q[0]
-                if not self.nans[i][n_old]:
-                    nf[4 * (gr_subtree_offsets[i] + n_new)] = float(self.feats[i][n_old] + 1)
-                else:
-                    nf[4 * (gr_subtree_offsets[i] + n_new)] = float(-(self.feats[i][n_old] + 1))
-                nf[4 * (gr_subtree_offsets[i] + n_new) + 1] = float(self.val_splits[i][n_old])
-                ln = self.split[i][n_old][0]
-                rn = self.split[i][n_old][1]
-
-                if self.feats[i][ln] < 0:
-                    nf[4 * (gr_subtree_offsets[i] + n_new) + 2] = float(-(self.leaves[ln][i] + 1))
-                else:
-                    new_node_number = q[-1][1] + 1
-                    nf[4 * (gr_subtree_offsets[i] + n_new) + 2] = float(new_node_number)
-                    q.append((ln, new_node_number))
-
-                if self.feats[i][rn] < 0:
-                    nf[4 * (gr_subtree_offsets[i] + n_new) + 3] = float(-(self.leaves[rn][i] + 1))
-                else:
-                    new_node_number = q[-1][1] + 1
-                    nf[4 * (gr_subtree_offsets[i] + n_new) + 3] = float(new_node_number)
-                    q.append((rn, new_node_number))
-                q.pop(0)
-
-        self.test_format = nf
-        self.test_format_offsets = gr_subtree_offsets
-
-        # feature_ importance with gain
-        self.feature_importance_gain = np.zeros(nfeats, dtype=np.float32)
-        sl = self.feats >= 0
-        np.add.at(self.feature_importance_gain, self.feats[sl], self.gains[sl])
-
-        # feature_ importance with split
-        self.feature_importance_split = np.zeros(nfeats, dtype=np.float32)
-        sl = self.feats >= 0
-        np.add.at(self.feature_importance_split, self.feats[sl], 1)
-
-        if not debug:
-            for attr in ['gains', 'feats', 'bin_splits', 'nans', 'split', 'val_splits', 'leaves']:
-                setattr(self, attr, None)
-
-
-class DepthwiseTreeBuilder:
-    """This class builds decision tree with given parameters"""
-
-    def __init__(self, borders,
-                 use_hess=True,
-                 colsampler=None,
-                 subsampler=None,
-                 target_splitter=None,
-                 multioutput_sketch=None,
-                 gd_steps=1,
-                 **tree_params
-                 ):
-        """
-
-        Args:
-            borders: list of np.ndarray, actual split borders for quantized features
-            colsampler: Callable or None, column sampling strategy
-            subsampler: Callable or None, rows sampling strategy
-            target_splitter: Callable or None, target grouping strategy
-            multioutput_sketch: Callable or None, multioutput sketching strategy
-            **tree_params: other tree building parameters
-        """
-        self.borders = borders
-        self.use_hess = use_hess
-        self.params = {**{
-
-            'lr': 1.,
-            'lambda_l2': .01,
-            'max_bin': 256,
-            'max_depth': 6,
-            'min_data_in_leaf': 10,
-            'min_gain_to_split': 0
-        }, **tree_params}
-
-        self.colsampler = colsampler
-        self.subsampler = subsampler
-        self.target_grouper = target_splitter
-        self.multioutput_sketch = multioutput_sketch
-        self.gd_steps = gd_steps
-
-    def build_tree(self, X, grad, hess, sample_weight=None, grad_fn=None, *val_arrays):
-        """Build tree and return nodes/values predictions for train and validation sets
-
-        Args:
-            X: cp.ndarray, quantized feature matrix
-            grad: cp.ndarray, gradient matrix
-            hess: cp.ndarray, hessian matrix
-            sample_weight: cp.ndarray or None, sample's weights
-            grad_fn: gradient fn
-            *val_arrays: list of cp.ndarray, list of quantized features for validation sets
-
-        Returns:
-            tree, Tree, constructed tree
-            nodes_group, cp.ndarray, nodes id for the train set
-            pred, cp.ndarray, prediction for the train set
-            valid_nodes_group, list of cp.ndarray, list of predicted nodes for valid sets
-            val_preds, list of cp.ndarray, list of predictions for valid sets
-        """
-        if self.colsampler is None:
-            col_indexer = cp.arange(X.shape[1], dtype=cp.uint64)
-        else:
-            col_indexer = self.colsampler()
-
-        if self.subsampler is None:
-            row_indexer = cp.arange(X.shape[0], dtype=cp.uint64)
-        else:
-            row_indexer = self.subsampler()
-
-        if self.target_grouper is None:
-            output_groups = [cp.arange(grad.shape[1], dtype=cp.uint64)]
-        else:
-            output_groups = self.target_grouper()
-
-        if sample_weight is not None:
-            grad = grad * sample_weight
-            hess = hess * sample_weight
-
-        max_nodes = int((2 ** np.arange(self.params['max_depth'] + 1)).sum())
-        tree = Tree(max_nodes, grad.shape[1], len(output_groups))
-
-        nodes_group = cp.empty((grad.shape[0], len(output_groups)), dtype=cp.int32)
-        valid_nodes_group = [cp.empty((x.shape[0], len(output_groups)), dtype=cp.int32) for x in val_arrays]
-
-        group_index = cp.zeros(grad.shape[1], dtype=cp.uint64)
-
-        for n_grp, grp_indexer in enumerate(output_groups):
-            G = grad[:, grp_indexer]
-            # if output group len eq. 1, we have single output tree, use hess for structure search
-            if G.shape[1] == 1:
-                H = hess if hess.shape[1] == 1 else hess[:, grp_indexer]
-            # else we can decide: should we use hess for tree structure search or
-            # assume hess eq. sample weight for all outputs, and then we can use proxy for tree structure search
-            else:
-                if self.use_hess:
-                    H = hess[:, grp_indexer]
-                else:
-                    H = sample_weight if sample_weight is not None else cp.ones((G.shape[0], 1), dtype=cp.float32)
-                if self.multioutput_sketch is not None:
-                    G, H = self.multioutput_sketch(G, H)
-
-            group_index[grp_indexer] = n_grp
-            # grow single group of the tree and get nodes index
-            train_nodes, valid_nodes = depthwise_grow_tree(tree, n_grp, X, G, H,
-                                                           row_indexer, col_indexer, self.params,
-                                                           valid_arrs=val_arrays)
-            # update nodes group
-            nodes_group[:, n_grp] = train_nodes
-            for vn, vp in zip(valid_nodes_group, valid_nodes):
-                vn[:, n_grp] = vp
-
-        # transform nodes to leaves
-        tree.set_leaves()
-        leaves_idx, max_leaves, leaves_grp = cp.asarray(tree.leaves, dtype=cp.int32), tree.max_leaves, \
-                                             cp.arange(len(output_groups), dtype=cp.uint64)
-
-        leaves = apply_values(nodes_group, leaves_grp, leaves_idx)
-        val_leaves = [apply_values(x, leaves_grp, leaves_idx) for x in valid_nodes_group]
-
-        # perform multiple grad steps
-        values = calc_node_values(grad, hess, leaves, row_indexer, group_index, max_leaves, self.params['lr'],
-                                  lambda_l2=self.params['lambda_l2'])
-        pred = apply_values(leaves, group_index, values)
-
-        tree.set_borders(self.borders)
-
-        for i in range(1, self.gd_steps):
-            grad, hess = grad_fn(pred)
-            values += calc_node_values(grad, hess, leaves, row_indexer, group_index, max_leaves, self.params['lr'],
-                                       lambda_l2=self.params['lambda_l2'])
-            pred = apply_values(leaves, group_index, values)
-
-        # transform leaves to values
-        val_preds = [apply_values(x, group_index, values) for x in val_leaves]
-        tree.set_node_values(values.get(), group_index.get())
-
-        return tree, leaves, pred, val_leaves, val_preds
+"""Decision trees building and inference"""
+
+try:
+    import cupy as cp
+except Exception:
+    pass
+import numpy as np
+
+from .utils import apply_values, depthwise_grow_tree, get_tree_node, set_leaf_values, calc_node_values
+from .utils import tree_prediction_leaves_typed_kernels, tree_prediction_leaves_typed_kernels_f
+from .utils import tree_prediction_values_kernel
+
+
+class Tree:
+    """This class initializes an empty tree structure, implements methods to set tree values and single tree inference.
+    The instance of this object represents the actual boosting step, but not the single tree!
+    Actual amount of trees in the instance (at each boosting step) is defined by ngroups argument. What it means:
+    Assume you have 5 class classification task, so you model output size equals 5. Possible cases here:
+        - Build single decision tree that outputs a vector of 5 values. In this case ngroups eq. 1
+        - Build 5 decision trees, each tree predict a value for its own class (one-vs-all).
+            In this case ngroups eq. 5
+        - Create custom target split strategy. For ex. you can build 2 trees, first will predict [0, 1, 2] classes,
+            second - [3, 4]. In this case ngroups eq. 2
+
+    Grouped trees structure is defined by arrays:
+        feats, shape (ngroups, max_nodes) - feature index to use for the split in each group/node.
+            If -1, the node is terminal (leaf)
+        val_splits, shape (ngroups, max_nodes) - threshold to compare when choosing the next node
+            if feature value is not NaN
+        nans, shape (ngroups, max_nodes) - bool values, if True, NaN feature values objects moves left, else - right
+        split, shape (ngroups, max_nodes, 2) - node indices corresponding left/right split for the current node
+
+    Trees structure defines single node id value for each object
+    Values assigned to the outputs are defined by arrays:
+        group_index, shape (nout, ). Defines the group id for predicting each output
+        values, shape (max_nodes, nout). Define output value for each node/output
+        leaves, shape (max_leaves, ngroups). Assigns the leaf index to the terminal nodes
+
+    During the fit stage, the format described above is used.
+    After fitting, additional reformatting occurs that converts the tree to another format to achieve faster inference:
+    - Sub-trees for each group are stored in one array named "test_format":
+        [gr0_node0, ..., gr0_nodeN, gr1_node0, ..., gr1_nodeM, gr2_node0, ..., gr2_nodeK, gr3_node0, ...]
+    - Each node in new formatted tree consists of 4 fields:
+        [feature_index, split_value, left_node_index, right_node_index],
+        feature_index - feature index to use for the split in each node.
+        split_value - threshold to compare when choosing the next node if feature value is not NaN
+        left_node_index - index of the left child in "test_format" array
+        right_node_index - index of the right child in "test_format" array
+    - The size of "test_format" array equals to the sum of all nodes in all subtrees except leaves multiplied by 4.
+        Multiplication by 4 occurs because each node consists of the 4 fields described above.
+        Examples:
+            test_format[0 * 4] == test_format[0] - yields feature_index for node with index 0.
+            test_format[0 * 4 + 1] == test_format[1] - yields split_value for node with index 0.
+            test_format[0 * 4 + 2] == test_format[2] - yields left_node_index for node with index 0.
+            test_format[0 * 4 + 3] == test_format[3] - yields right_node_index for node with index 0.
+            test_format[1 * 4] == test_format[4]  - yields feature_index for node with index 1.
+            test_format[1 * 4 + 1] == test_format[5] - yields split_value for node with index 1.
+            test_format[1 * 4 + 2] == test_format[6] - yields left_node_index for node with index 1.
+            test_format[1 * 4 + 3] == test_format[7] - yields right_node_index for node with index 1.
+            test_format[2 * 4] == test_format[8]  - yields feature_index for node with index 2.
+            ...
+            test_format[79 * 4] == test_format[316]  - yields feature_index for node with index 79.
+            test_format[79 * 4 + 1] == test_format[317] - yields split_value for node with index 79.
+            test_format[79 * 4 + 2] == test_format[318] - yields left_node_index for node with index 79.
+            test_format[79 * 4 + 3] == test_format[319] - yields right_node_index for node with index 79.
+            ...
+    - The sign of the feature_index value shows the behavior in case of feature == NaN (split to the left/right),
+        to the value written in feature_index an extra "1" is added to deal with zero.
+        Examples:
+            feature_index == 8, positive value means that tree follows to the left in case of NaN in feature,
+                the real feature index is calculated as follows: abs(8) - 1 = 7.
+            feature_index == -19, negative value means that tree follows to the right in case of NaN in feature,
+                the real feature index is calculated as follows: abs(-19) - 1 = 18.
+            feature_index == 0, impossible due to construction algorithm.
+    - If left_node_index/right_node_index is negative, it means that it shows index in the values array;
+        In case of a negative value, an extra "1" is added to deal with zero.
+        Examples:
+            left_node_index == 8, non-negative value means that left child node is stored in "test_format" with index 8;
+            left_node_index == -13, means that left child is a leaf, the index in "values" array for that leaf can
+                be calculated as follows: abs(-13) - 1 = 12. Thus, index in "values" array is 12.
+    - All subtrees are stored in one array, so an additional array of indexes where each subtree is starting
+        is required (index of the subtree roots), array "gr_subtree_offsets" stores these indexes,
+        size of "gr_subtree_offsets" equals to number of groups in the tree (number of subtrees).
+        Example:
+            gr_subtree_offsets == [0, 56, 183], means that tree has 3 subtrees (3 groups).
+            The first subtree has its root as node with index 0;
+            The second subtree has its root as node with index 56;
+            The third subtree has its root as node with index 183.
+            Example how to access the values of the root node in the second subtree:
+                test_format[56 * 4] == test_format[224]  - yields feature_index for the root of the second subtree;
+                test_format[56 * 4 + 1] == test_format[225] - yields split_value for the root of the second subtree;
+                test_format[56 * 4 + 2] == test_format[226] - yields left_node_index for the root of the second subtree;
+                test_format[56 * 4 + 3] == test_format[227] - yields right_node_index for the root of the second subtree
+    - Two fields, 'feature_importance_gain' and 'feature_importance_split', store feature importance arrays
+        and describe the fitted tree accordingly.
+    """
+
+    def __init__(self, max_nodes, nout, ngroups):
+        """Initialize empty tree
+
+        Args:
+            max_nodes: int, maximum number of nodes in tree
+            nout: int, number of outputs in tree
+            ngroups: int, number of groups
+        """
+        self.nout = nout
+        self.ngroups = ngroups
+        self.max_nodes = max_nodes
+
+        self.gains = np.zeros((ngroups, max_nodes,), dtype=np.float32)
+        self.feats = np.zeros((ngroups, max_nodes,), dtype=np.int64) - 1
+        self.bin_splits = np.zeros((ngroups, max_nodes,), dtype=np.int32)
+        self.nans = np.zeros((ngroups, max_nodes,), dtype=np.bool_)
+
+        self.split = np.zeros((ngroups, max_nodes, 2), dtype=np.int32)
+
+        self.val_splits = None
+        self.values = None
+        self.group_index = None
+        self.leaves = None
+        self.max_leaves = None
+
+        self.feature_importance_gain = None
+        self.feature_importance_split = None
+
+        self._debug = None
+        self.test_format = None
+        self.test_format_offsets = None
+
+    def set_nodes(self, group, unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left):
+        """Write info about new nodes
+
+        Args:
+            group: int, group id to write
+            unique_nodes: np.ndarray, nodes id to set info
+            new_nodes_id: np.ndarray, nodes id to left/right split current node
+            best_feat: np.ndarray, feature value to perform a split
+            best_gain: np.ndarray, gain from the split
+            best_split: np.ndarray, quantized threshold to compare when split
+            best_nan_left: np.ndarray, bool if True, nans moved in the left node, else right
+
+        Returns:
+
+        """
+
+        self.gains[group, unique_nodes] = best_gain
+        self.feats[group, unique_nodes] = best_feat
+        self.bin_splits[group, unique_nodes] = best_split
+        self.nans[group, unique_nodes] = best_nan_left
+        self.split[group, unique_nodes] = new_nodes_id
+
+    def set_node_values(self, values, group_index):
+        """Assign output values for each nodes
+
+        Args:
+            values: np.ndarray, node values
+            group_index: np.ndarray, group id of each output
+
+        Returns:
+
+        """
+        self.values = values
+        self.group_index = group_index
+
+    def set_borders(self, borders):
+        """Assign actual feature values based on quantized
+
+        Args:
+            borders: list of np.ndarray, actual node values
+
+        Returns:
+
+        """
+        # borders - list of arrays. Array is borderlines
+        val_splits = [0 if x == -1 else borders[x][min(y, len(borders[x]) - 1)]
+                      for (x, y) in zip(self.feats.ravel(), self.bin_splits.ravel())]
+        self.val_splits = np.array(val_splits, dtype=np.float32).reshape(self.feats.shape)
+
+    def set_leaves(self):
+        """Assign leaf id to the terminal nodes
+
+        Returns:
+
+        """
+        self.leaves, self.max_leaves = set_leaf_values(self.feats, self.split)
+
+    def to_device(self):
+        """Move tree data to the current GPU memory
+
+        Returns:
+
+        """
+        for attr in ['gains', 'feats', 'bin_splits', 'nans', 'split', 'val_splits', 'values', 'group_index', 'leaves',
+                     'test_format', 'test_format_offsets', 'feature_importance_gain', 'feature_importance_split']:
+            arr = getattr(self, attr)
+
+            if type(arr) is np.ndarray:
+                setattr(self, attr, cp.asarray(arr))
+
+    def to_cpu(self):
+        """Move tree data to the CPU memory
+
+        Returns:
+
+        """
+        for attr in ['gains', 'feats', 'bin_splits', 'nans', 'split', 'val_splits', 'values', 'group_index', 'leaves',
+                     'test_format', 'test_format_offsets', 'feature_importance_gain', 'feature_importance_split']:
+            arr = getattr(self, attr)
+
+            if type(arr) is cp.ndarray:
+                setattr(self, attr, arr.get())
+
+    def _predict_node_deprecated(self, X):
+        """(DEPRECATED) Predict node id from the feature matrix X
+
+        Args:
+            X: cp.ndarray of features
+
+        Returns:
+
+        """
+        if self.feats is None:
+            raise Exception('To use _deprecated funcs pass debug=True to .reformat')
+
+        assert type(self.feats) is cp.ndarray, 'Should be moved to GPU first. Call .to_device()'
+        nodes = get_tree_node(X, self.feats, self.val_splits, self.split, self.nans)
+        return nodes
+
+    def _predict_from_nodes_deprecated(self, nodes):
+        """(DEPRECATED) Predict outputs from the nodes indices
+
+        Args:
+            nodes: cp.ndarray of predicted nodes
+
+        Returns:
+            cp.ndarray of nodes
+        """
+        return apply_values(nodes, self.group_index, self.values)
+
+    def _predict_leaf_from_nodes_deprecated(self, nodes):
+        """Predict leaf indices from the nodes indices (Use predict_leaf() method if you need to predict leaves)
+
+        Args:
+            nodes: cp.ndarray of predicted nodes
+
+        Returns:
+            cp.ndarray of leaves
+        """
+        return apply_values(nodes, cp.arange(self.ngroups, dtype=cp.uint64), self.leaves)
+
+    def _predict_deprecated(self, X):
+        """(DEPRECATED) Predict from the feature matrix X
+
+        Args:
+            X: cp.ndarray of features
+
+        Returns:
+            cp.ndarray of predictions
+        """
+        return self._predict_from_nodes_deprecated(
+            self._predict_leaf_from_nodes_deprecated(self._predict_node_deprecated(X)))
+
+    def _predict_leaf_deprecated(self, X):
+        """(DEPRECATED) Predict leaf indices from the feature matrix X
+
+        Args:
+            X: cp.ndarray of features
+
+        Returns:
+            cp.ndarray of leaves
+        """
+        return self._predict_leaf_from_nodes_deprecated(self._predict_node_deprecated(X))
+
+    def predict_leaf(self, X, pred_leaves=None):
+        """Predict leaf indexes from the feature matrix X
+
+        Args:
+            X: cp.ndarray, array of features
+            pred_leaves: cp.ndarray, buffer for predictions
+
+        Returns:
+            pred_leaves: leaf predictions
+
+        """
+        # check if buffer is None and X on GPU
+        assert type(X) is cp.ndarray, "X must be type of cp.ndarray (located on gpu)"
+
+        dt = str(X.dtype)
+
+        assert dt in tree_prediction_leaves_typed_kernels, \
+            f"X array must be of type: {list(tree_prediction_leaves_typed_kernels.keys())}"
+
+        if pred_leaves is None:
+            pred_leaves = cp.empty((X.shape[0], self.ngroups), dtype=cp.int32)
+
+        # CUDA parameters initialization
+        threads = 128  # threads in one CUDA block
+        sz = X.shape[0] * self.ngroups
+        blocks = sz // threads
+        if sz % threads != 0:
+            blocks += 1
+
+        if X.flags["C_CONTIGUOUS"]:
+            tree_prediction_leaves_typed_kernels[dt]((blocks,), (threads,), ((X,
+                                                                              self.test_format,
+                                                                              self.test_format_offsets,
+                                                                              X.shape[1],
+                                                                              X.shape[0],
+                                                                              self.ngroups,
+                                                                              pred_leaves.shape[1],
+                                                                              pred_leaves)))
+        elif X.flags["F_CONTIGUOUS"]:
+            tree_prediction_leaves_typed_kernels_f[dt]((blocks,), (threads,), ((X,
+                                                                                self.test_format,
+                                                                                self.test_format_offsets,
+                                                                                X.shape[1],
+                                                                                X.shape[0],
+                                                                                self.ngroups,
+                                                                                pred_leaves.shape[1],
+                                                                                pred_leaves)))
+        else:
+            raise Exception("X must be 'C_CONTIGUOUS' or 'F_CONTIGUOUS'")
+        return pred_leaves
+
+    def predict(self, X, pred=None, pred_leaves=None):
+        """Predict from the feature matrix X
+
+        Args:
+            X: cp.ndarray, array of features
+            pred: cp.ndarray, buffer for predictions on GPU, if None - created automatically
+            pred_leaves: cp.ndarray, buffer for internal leaf predictions on GPU, if None - created automatically
+
+        Returns:
+            pred: cp.ndarray, prediction array
+
+        """
+        # check if buffers are None
+        if pred is None:
+            pred = cp.zeros((X.shape[0], self.nout), dtype=cp.float32)
+        if pred_leaves is None:
+            pred_leaves = cp.empty((X.shape[0], self.ngroups), dtype=cp.int32)
+
+        # first step - leaves predictions, actually prediction of indexes in values
+        self.predict_leaf(X, pred_leaves)
+
+        # CUDA parameters initialization
+        threads = 128  # threads in one CUDA block
+        sz = X.shape[0] * self.nout
+        blocks = sz // threads
+        if sz % threads != 0:
+            blocks += 1
+
+        # second step, prediction of actual values
+        tree_prediction_values_kernel((blocks,), (threads,), ((pred_leaves,
+                                                               self.group_index,
+                                                               self.values,
+                                                               self.nout,
+                                                               X.shape[0],
+                                                               pred_leaves.shape[1],
+                                                               pred)))
+        return pred
+
+    def reformat(self, nfeats, debug):
+        """Creates new internal format of the tree for faster inference
+        
+        Args:
+            nfeats: int, number of features in X (train set)
+            debug: bool, if in debug mode
+
+        Returns:
+
+        """
+        n_gr = self.ngroups
+
+        # memory allocation for new tree array
+        gr_subtree_offsets = np.zeros(n_gr, dtype=np.int32)
+        check_empty = []
+        total_size = 0
+        for i in range(n_gr):
+            curr_size = int((self.feats[i] >= 0).sum())
+            # add special case handling - single leaf, no splits
+            check_empty.append(curr_size == 0)
+            curr_size = max(1, curr_size)
+            total_size += curr_size
+
+            if i < n_gr - 1:
+                gr_subtree_offsets[i + 1] = total_size
+        nf = np.zeros(total_size * 4, dtype=np.float32)
+
+        # reformatting the tree
+        for i in range(n_gr):
+            # handle special case - single leaf, no splits - make a pseudo split node
+            if check_empty[i]:
+                nf[4 * gr_subtree_offsets[i]] = 1.
+                nf[4 * gr_subtree_offsets[i] + 1] = 0.
+                nf[4 * gr_subtree_offsets[i] + 2] = -1.
+                nf[4 * gr_subtree_offsets[i] + 3] = -1.
+
+                continue
+
+            q = [(0, 0)]
+
+            while len(q) != 0:  # BFS in tree
+                n_old, n_new = q[0]
+                if not self.nans[i][n_old]:
+                    nf[4 * (gr_subtree_offsets[i] + n_new)] = float(self.feats[i][n_old] + 1)
+                else:
+                    nf[4 * (gr_subtree_offsets[i] + n_new)] = float(-(self.feats[i][n_old] + 1))
+                nf[4 * (gr_subtree_offsets[i] + n_new) + 1] = float(self.val_splits[i][n_old])
+                ln = self.split[i][n_old][0]
+                rn = self.split[i][n_old][1]
+
+                if self.feats[i][ln] < 0:
+                    nf[4 * (gr_subtree_offsets[i] + n_new) + 2] = float(-(self.leaves[ln][i] + 1))
+                else:
+                    new_node_number = q[-1][1] + 1
+                    nf[4 * (gr_subtree_offsets[i] + n_new) + 2] = float(new_node_number)
+                    q.append((ln, new_node_number))
+
+                if self.feats[i][rn] < 0:
+                    nf[4 * (gr_subtree_offsets[i] + n_new) + 3] = float(-(self.leaves[rn][i] + 1))
+                else:
+                    new_node_number = q[-1][1] + 1
+                    nf[4 * (gr_subtree_offsets[i] + n_new) + 3] = float(new_node_number)
+                    q.append((rn, new_node_number))
+                q.pop(0)
+
+        self.test_format = nf
+        self.test_format_offsets = gr_subtree_offsets
+
+        # feature_ importance with gain
+        self.feature_importance_gain = np.zeros(nfeats, dtype=np.float32)
+        sl = self.feats >= 0
+        np.add.at(self.feature_importance_gain, self.feats[sl], self.gains[sl])
+
+        # feature_ importance with split
+        self.feature_importance_split = np.zeros(nfeats, dtype=np.float32)
+        sl = self.feats >= 0
+        np.add.at(self.feature_importance_split, self.feats[sl], 1)
+
+        if not debug:
+            for attr in ['gains', 'feats', 'bin_splits', 'nans', 'split', 'val_splits', 'leaves']:
+                setattr(self, attr, None)
+
+
+class DepthwiseTreeBuilder:
+    """This class builds decision tree with given parameters"""
+
+    def __init__(self, borders,
+                 use_hess=True,
+                 colsampler=None,
+                 subsampler=None,
+                 target_splitter=None,
+                 multioutput_sketch=None,
+                 gd_steps=1,
+                 **tree_params
+                 ):
+        """
+
+        Args:
+            borders: list of np.ndarray, actual split borders for quantized features
+            colsampler: Callable or None, column sampling strategy
+            subsampler: Callable or None, rows sampling strategy
+            target_splitter: Callable or None, target grouping strategy
+            multioutput_sketch: Callable or None, multioutput sketching strategy
+            **tree_params: other tree building parameters
+        """
+        self.borders = borders
+        self.use_hess = use_hess
+        self.params = {**{
+
+            'lr': 1.,
+            'lambda_l2': .01,
+            'max_bin': 256,
+            'max_depth': 6,
+            'min_data_in_leaf': 10,
+            'min_gain_to_split': 0
+        }, **tree_params}
+
+        self.colsampler = colsampler
+        self.subsampler = subsampler
+        self.target_grouper = target_splitter
+        self.multioutput_sketch = multioutput_sketch
+        self.gd_steps = gd_steps
+
+    def build_tree(self, X, grad, hess, sample_weight=None, grad_fn=None, *val_arrays):
+        """Build tree and return nodes/values predictions for train and validation sets
+
+        Args:
+            X: cp.ndarray, quantized feature matrix
+            grad: cp.ndarray, gradient matrix
+            hess: cp.ndarray, hessian matrix
+            sample_weight: cp.ndarray or None, sample's weights
+            grad_fn: gradient fn
+            *val_arrays: list of cp.ndarray, list of quantized features for validation sets
+
+        Returns:
+            tree, Tree, constructed tree
+            nodes_group, cp.ndarray, nodes id for the train set
+            pred, cp.ndarray, prediction for the train set
+            valid_nodes_group, list of cp.ndarray, list of predicted nodes for valid sets
+            val_preds, list of cp.ndarray, list of predictions for valid sets
+        """
+        if self.colsampler is None:
+            col_indexer = cp.arange(X.shape[1], dtype=cp.uint64)
+        else:
+            col_indexer = self.colsampler()
+
+        if self.subsampler is None:
+            row_indexer = cp.arange(X.shape[0], dtype=cp.uint64)
+        else:
+            row_indexer = self.subsampler()
+
+        if self.target_grouper is None:
+            output_groups = [cp.arange(grad.shape[1], dtype=cp.uint64)]
+        else:
+            output_groups = self.target_grouper()
+
+        if sample_weight is not None:
+            grad = grad * sample_weight
+            hess = hess * sample_weight
+
+        max_nodes = int((2 ** np.arange(self.params['max_depth'] + 1)).sum())
+        tree = Tree(max_nodes, grad.shape[1], len(output_groups))
+
+        nodes_group = cp.empty((grad.shape[0], len(output_groups)), dtype=cp.int32)
+        valid_nodes_group = [cp.empty((x.shape[0], len(output_groups)), dtype=cp.int32) for x in val_arrays]
+
+        group_index = cp.zeros(grad.shape[1], dtype=cp.uint64)
+
+        for n_grp, grp_indexer in enumerate(output_groups):
+            G = grad[:, grp_indexer]
+            # if output group len eq. 1, we have single output tree, use hess for structure search
+            if G.shape[1] == 1:
+                H = hess if hess.shape[1] == 1 else hess[:, grp_indexer]
+            # else we can decide: should we use hess for tree structure search or
+            # assume hess eq. sample weight for all outputs, and then we can use proxy for tree structure search
+            else:
+                if self.use_hess:
+                    H = hess[:, grp_indexer]
+                else:
+                    H = sample_weight if sample_weight is not None else cp.ones((G.shape[0], 1), dtype=cp.float32)
+                if self.multioutput_sketch is not None:
+                    G, H = self.multioutput_sketch(G, H)
+
+            group_index[grp_indexer] = n_grp
+            # grow single group of the tree and get nodes index
+            train_nodes, valid_nodes = depthwise_grow_tree(tree, n_grp, X, G, H,
+                                                           row_indexer, col_indexer, self.params,
+                                                           valid_arrs=val_arrays)
+            # update nodes group
+            nodes_group[:, n_grp] = train_nodes
+            for vn, vp in zip(valid_nodes_group, valid_nodes):
+                vn[:, n_grp] = vp
+
+        # transform nodes to leaves
+        tree.set_leaves()
+        leaves_idx, max_leaves, leaves_grp = cp.asarray(tree.leaves, dtype=cp.int32), tree.max_leaves, \
+                                             cp.arange(len(output_groups), dtype=cp.uint64)
+
+        leaves = apply_values(nodes_group, leaves_grp, leaves_idx)
+        val_leaves = [apply_values(x, leaves_grp, leaves_idx) for x in valid_nodes_group]
+
+        # perform multiple grad steps
+        values = calc_node_values(grad, hess, leaves, row_indexer, group_index, max_leaves, self.params['lr'],
+                                  lambda_l2=self.params['lambda_l2'])
+        pred = apply_values(leaves, group_index, values)
+
+        tree.set_borders(self.borders)
+
+        for i in range(1, self.gd_steps):
+            grad, hess = grad_fn(pred)
+            values += calc_node_values(grad, hess, leaves, row_indexer, group_index, max_leaves, self.params['lr'],
+                                       lambda_l2=self.params['lambda_l2'])
+            pred = apply_values(leaves, group_index, values)
+
+        # transform leaves to values
+        val_preds = [apply_values(x, group_index, values) for x in val_leaves]
+        tree.set_node_values(values.get(), group_index.get())
+
+        return tree, leaves, pred, val_leaves, val_preds
```

### Comparing `py_boost-0.4.3/py_boost/gpu/utils.py` & `py_boost-0.5.0/py_boost/gpu/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,974 +1,1005 @@
-"""Utilities used for trees building and inference"""
-
-import math
-import numba
-import numpy as np
-try:
-    import cupy as cp
-    CUDA_FOUND = True
-except Exception:
-    CUDA_FOUND = False
-
-
-def validate_input(X, y, sample_weight=None, eval_sets=None):
-    if eval_sets is None:
-        eval_sets = []
-
-    if len(y.shape) == 1:
-        y = y[:, np.newaxis]
-
-    if (sample_weight is not None) and (len(sample_weight.shape) == 1):
-        sample_weight = sample_weight[:, np.newaxis]
-
-    eval_sets = list(eval_sets)
-    for val_arr in eval_sets:
-        if len(val_arr['y'].shape) == 1:
-            val_arr['y'] = val_arr['y'][:, np.newaxis]
-
-        if 'sample_weight' not in val_arr:
-            val_arr['sample_weight'] = None
-
-        if (val_arr['sample_weight'] is not None) and (len(val_arr['sample_weight'].shape) == 1):
-            val_arr['sample_weight'] = val_arr['sample_weight'][:, np.newaxis]
-
-    return X, y, sample_weight, eval_sets
-
-
-def pad_and_move(arr, pad_size=4):
-    """Pad array memory placeholder to make feature size divisible by pad_size and move to GPU.
-    Returned array is the same size as input, but it is not contiguous.
-    Basic memory placeholder size is divisible by pad_size and could be accesses via arr.base.
-    This trick helps to speed up histogram computation for the large arrays.
-
-    Args:
-        arr: 2d np.ndarray of uint8 containing quantized features matrix
-        pad_size: int, memory placeholder feature size will be divisible by pad_size
-
-    Returns:
-        cp.ndarray of quantized features
-    """
-    assert arr.dtype == np.uint8, 'Array dtype should be unsigned 8bit int'
-
-    pfeats = math.ceil(arr.shape[1] / pad_size) * pad_size
-    arr_cpu_padded = np.zeros((arr.shape[0], pfeats), dtype=np.uint8)
-    arr_cpu_padded[:, :arr.shape[1]] = arr
-    arr_gpu_padded = cp.asarray(arr_cpu_padded)
-
-    return arr_gpu_padded[:, :arr.shape[1]]
-
-
-isin_code = """
-int fnode;
-int leaf = 0;
-int minval = 0;
-int maxval = l - 1;
-
-int node_val = nodes[index];
-
-while (true) {{
-
-    leaf = minval + (maxval - minval) / 2;
-    fnode = un[leaf];
-
-    if (fnode == node_val) {{
-
-        isin={0};
-        return;
-
-    }} else if (minval >= maxval) {{
-
-        isin={1};
-        return ;
-
-    }} else if (fnode < node_val) {{
-
-        minval = leaf + 1;
-
-    }} else  {{
-
-        maxval = leaf - 1;
-
-    }} 
-}}
-
-"""
-
-isin_kernel = cp.ElementwiseKernel(
-    'Q index, raw E nodes, raw R un, uint64 l',
-    'bool isin',
-
-    isin_code.format('true', 'false'),
-
-    'isin_kernel'
-) if CUDA_FOUND else None
-
-isin_pos_kernel = cp.ElementwiseKernel(
-    'Q index, raw E nodes, raw R un, uint64 l',
-    'int32 isin',
-
-    isin_code.format('leaf', -1),
-
-    'isin_pos_kernel'
-) if CUDA_FOUND else None
-
-
-def isin(a, b, index=None, return_pos=False):
-    """Check if b contains elements of a. Custom function is faster than build in cupy's
-
-    Args:
-        a: cp.ndarray to apply
-        b: cp.ndarray lookup array
-        index: cp.ndarray indices of a to check. If None, check for all a
-        return_pos: bool, if True, return position of a[i] in b, otherwise return bool array if a[i] is in b
-
-    Returns:
-        cp.ndarray of bool or int
-    """
-    if index is None:
-        index = cp.arange(a.shape[0], dtype=cp.uint64)
-
-    if return_pos:
-        return isin_pos_kernel(index, a, b, b.shape[0])
-    else:
-        return isin_kernel(index, a, b, b.shape[0])
-
-
-histogram_kernel_idx = cp.ElementwiseKernel(
-    """
-    uint64 i_, uint64 j_, uint64 k_, 
-    uint64 kk,
-
-    raw uint64 jj,
-    raw bool padded_bool_indexer,
-
-    raw float32 target, 
-    raw T arr, 
-    raw int32 nodes,
-
-    uint64 hlen,
-    uint64 flen, 
-    uint64 length,
-    uint64 feats,
-    uint64 nout 
-    """,
-    'raw float32 hist',
-
-    """
-    unsigned int feat_4t = arr[i_ * feats + j_];
-    int d;
-    int j;
-    int val;
-    int pos;
-    float *x_ptr;
-    float y = target[i_ * nout + k_];
-
-    for (d = 0; d < 4; d++) {
-
-        pos = (i_ + d) % 4;
-
-        if (padded_bool_indexer[j_ * 4 + pos]) {
-
-            val = (feat_4t >> (8 * pos)) % 256;
-            j = jj[j_ * 4 + pos];
-            x_ptr = &hist[0] +  kk * hlen + nodes[i_] * flen + j * length + val;
-            atomicAdd(x_ptr, y); 
-        }
-    }
-
-    """,
-
-    'histogram_kernel_idx') if CUDA_FOUND else None
-
-feature_grouper_kernel = cp.ElementwiseKernel(
-    """
-    uint64 col_indexer
-    """,
-    'raw bool padded_bool_indexer, raw bool tuple_indexer, raw uint64 padded_col_indexer',
-    """
-    int tuple_id = col_indexer / 4;
-    padded_bool_indexer[col_indexer] = true;
-    tuple_indexer[tuple_id] = true;
-    padded_col_indexer[col_indexer] = i;
-
-    """,
-    'feature_grouper_kernel') if CUDA_FOUND else None
-
-
-def fill_histogram(res, arr, target, nodes, col_indexer, row_indexer, out_indexer):
-    """Fill the histogram res
-
-    Args:
-        res: cp.ndarray, histogram of zeros, shape (n_out, n_nodes, n_features, n_bins)
-        arr: cp.ndarray, features array, shape (n_data, n_features)
-        target: cp.ndarray, values to accumulate, shape (n_data, n_out)
-        nodes: cp.ndarray, tree node indices, shape (n_data, )
-        col_indexer: cp.ndarray, indices of features to accumulate
-        row_indexer: cp.ndarray, indices of rows to accumulate
-        out_indexer: cp.ndarray, indices of outputs to accumulate
-
-    Returns:
-
-    """
-    # define data split for kernel launch
-    nout, nnodes, nfeats, nbins = res.shape
-
-    # padded array of 4 feature tuple
-    arr_4t = arr.base.view(dtype=cp.uint32)
-    pfeats = arr_4t.shape[1]
-
-    # create 4 feats tuple indexer
-    padded_bool_indexer = cp.zeros((arr.base.shape[1],), dtype=cp.bool_)
-    padded_col_indexer = cp.zeros((arr.base.shape[1],), dtype=cp.uint64)
-    tuple_indexer = cp.zeros((arr_4t.shape[1],), dtype=cp.bool_)
-
-    feature_grouper_kernel(col_indexer, padded_bool_indexer, tuple_indexer, padded_col_indexer)
-    tuple_indexer = cp.arange(arr_4t.shape[1], dtype=cp.uint64)[tuple_indexer]
-
-    fb = nfeats * nbins
-    nfb = nnodes * fb
-
-    magic_constant = 2 ** 19  # optimal value for my V100
-
-    # split features
-    nsplits = math.ceil(nfb / magic_constant)
-    # first split by feats
-    feats_batch = math.ceil(pfeats / nsplits)
-    # split by features
-    if feats_batch == nfeats:
-        out_batch = magic_constant // nfb
-    else:
-        out_batch = 1
-
-    ri = row_indexer[:, cp.newaxis, cp.newaxis]
-    ti = tuple_indexer[cp.newaxis, :, cp.newaxis]
-    oi = out_indexer[cp.newaxis, cp.newaxis, :]
-
-    oii = cp.arange(oi.shape[2], dtype=cp.uint64)[cp.newaxis, cp.newaxis, :]
-
-    for j in range(0, pfeats, feats_batch):
-        ti_ = ti[:, j: j + feats_batch]
-
-        for k in range(0, nout, out_batch):
-            oi_ = oi[..., k: k + out_batch]
-            oii_ = oii[..., k: k + out_batch]
-
-            histogram_kernel_idx(ri, ti_, oi_,
-                                 oii_,
-                                 padded_col_indexer,
-                                 padded_bool_indexer,
-                                 target,
-                                 arr_4t,
-                                 nodes,
-                                 nfb, fb, nbins, arr_4t.shape[1], nout,
-                                 res)
-
-
-def histogram(arr, gh, nodes, col_indexer, row_indexer, out_indexer, nnodes, max_bins,
-              prev_hist=None, small_index=None, big_index=None):
-    """Compute grad/hess histogram
-
-    Args:
-        arr: cp.ndarray, features array, shape (n_data, n_features)
-        gh: cp.ndarray of grad/hess, shape (n_data, n_out + 1), assume the last output is hess, others for grads
-        nodes: cp.ndarray, tree node indices, shape (n_data, )
-        col_indexer: cp.ndarray, indices of features to accumulate
-        row_indexer: cp.ndarray, indices of rows to accumulate
-        out_indexer: cp.ndarray, indices of outputs to accumulate
-        nnodes: int, total number of nodes in the sample
-        max_bins: int, maximum number of feature bins
-        prev_hist: cp.ndarray or None, histogram from previous step to apply histogram subtraction trick
-        small_index: cp.ndarray or None, node indices to accumulate
-        big_index: cp.ndarray or None, node indices to compute by subtraction from prev_hist
-
-    Returns:
-        cp.ndarray, histogram of shape (n_out + 1, n_nodes, n_features, n_bins)
-    """
-
-    nout = out_indexer.shape[0]
-    nfeats = col_indexer.shape[0]
-    # init union histogram for grad and hess
-    # we assume, we have 1 dim hess for one output group
-
-    res = cp.zeros((nout, nnodes, nfeats, max_bins), dtype=cp.float32)
-
-    if prev_hist is not None:
-        row_indexer = row_indexer[isin(nodes, small_index, row_indexer)]
-
-    fill_histogram(res, arr, gh, nodes, col_indexer, row_indexer, out_indexer)
-    res = res.cumsum(axis=-1)
-
-    if prev_hist is not None:
-        # indices are paired.
-        res[:, big_index] = prev_hist - res[:, big_index + (1 - 2 * (big_index % 2))]
-
-    return res
-
-
-loss_kernel = cp.ElementwiseKernel(
-    """
-    float32 grad, float32 hess, 
-    float32 total_grad, float32 total_hess, 
-    float32 nan_grad, float32 nan_hess, 
-
-    uint64 nodes_count, 
-    float32 lambda_l2, float32 min_data_in_left
-
-
-    """,
-    'raw float32 res',
-
-    """
-
-    float rG;
-    float G = grad;
-    float H = hess;
-    float C = hess / total_hess * nodes_count;
-
-
-    if (fmin(nodes_count - C, C) > min_data_in_left) {
-        rG = total_grad - G;
-        res[2 * i] = G * G / (H + lambda_l2) + rG * rG / (total_hess - H + lambda_l2);
-    }
-
-    if ((nan_hess > 0) and (hess < total_hess)) {
-
-        C -= nan_hess / total_hess * nodes_count;
-
-        if (fmin(nodes_count - C, C) > min_data_in_left) {
-
-            G -= nan_grad;
-            H -= nan_hess;
-            rG = total_grad - G;
-            res[2 * i + 1] = G * G / (H + lambda_l2) + rG * rG / (total_hess - H + lambda_l2);
-
-        }
-    }
-
-    """,
-
-    'loss_kernel') if CUDA_FOUND else None
-
-
-def calc_loss(grad, hess, nodes_count, lambda_l2=0.1, min_data_in_leaf=10.):
-    """Calculate loss function
-
-    Args:
-        grad:
-        hess:
-        nodes_count:
-        lambda_l2:
-        min_data_in_leaf:
-
-    Returns:
-
-    """
-    # fill loss
-    res = cp.zeros(grad.shape + (2,), dtype=cp.float32)
-    loss_kernel(grad, hess,
-                grad[..., -1:], hess[..., -1:],
-                grad[..., :1], hess[..., :1],
-                nodes_count[cp.newaxis, :, cp.newaxis, cp.newaxis],
-                lambda_l2, min_data_in_leaf, res)
-
-    return res
-
-
-select_among_feature = cp.ElementwiseKernel(
-    """
-    int64 best_idx, 
-    raw float32 loss,
-    uint64 binsx2
-    """,
-    'float32 best_gain, int32 best_split, bool best_nan_left',
-
-    """
-    best_gain = loss[i * binsx2 + best_idx];
-    best_split = best_idx / 2;
-    best_nan_left = (bool) (1 - best_idx % 2);
-
-    """,
-
-    'select_among_feature') if CUDA_FOUND else None
-
-select_total = cp.ElementwiseKernel(
-    """
-    int64 best_idx,
-    raw float32 feat_loss,
-    raw int32 feat_split,
-    raw bool feat_nan_left,
-    raw uint64 col_indexer, 
-
-    uint64 feats
-    """,
-    'int64 best_feat, float32 best_gain, int32 best_split, bool best_nan_left',
-
-    """
-    unsigned long f_ptr = i * feats + best_idx;
-
-    best_gain = feat_loss[f_ptr];
-    best_split = feat_split[f_ptr];
-    best_nan_left = feat_nan_left[f_ptr];
-    best_feat = col_indexer[best_idx];
-
-    """,
-
-    'select_total') if CUDA_FOUND else None
-
-
-def get_best_split(loss, col_indexer):
-    nnodes, nfeats, nbins, _ = loss.shape
-    # shape - nnodes * nfeats
-    best_loss_among_feat_idx = loss.reshape((nnodes, nfeats, -1)).argmax(axis=-1)
-
-    best_gain, best_split, best_nan_left = \
-        select_among_feature(
-            best_loss_among_feat_idx, loss, nbins * 2
-        )
-
-    best_feat_ = best_gain.argmax(axis=-1)
-
-    best_feat, best_gain, best_split, best_nan_left = \
-        select_total(
-            best_feat_, best_gain, best_split, best_nan_left, col_indexer, nfeats
-        )
-
-    best_gain -= loss[:, 0, -1, 0]
-
-    return best_feat, best_gain, best_split, best_nan_left
-
-
-split_kernel = cp.ElementwiseKernel(
-    """
-    int32 nodes_index,
-    int32 nodes_old,
-    raw uint8 arr,
-    raw int32 split_nodes,
-    raw int64 feat,
-    raw int32 split,
-    raw bool nan_left,
-    uint64 F
-    """,
-    'int32 nodes',
-
-    """
-    if (nodes_index >= 0) {
-
-        int f = feat[nodes_index];
-        int s = split[nodes_index];
-        bool nl = nan_left[nodes_index];
-
-        int val = arr[i * F + f];
-
-        int d = 0;
-        if ((val > s) or ((val == 0) and (not nl))) {d = 1;}
-
-        nodes = split_nodes[2 * nodes_index + d];
-
-    } else {nodes=nodes_old;}
-
-    """,
-
-    'split_kernel') if CUDA_FOUND else None
-
-
-def make_split(nodes, arr, unique_nodes, split_nodes, feat, split, nan_left, return_pos=False):
-    nodes_index = isin(nodes, unique_nodes, return_pos=True)
-    new_nodes = split_kernel(nodes_index, nodes, arr, split_nodes, feat, split, nan_left, arr.shape[1])
-
-    if return_pos:
-        nodes_index = isin(new_nodes, split_nodes.ravel(), return_pos=True)
-        return new_nodes, nodes_index
-
-    return new_nodes
-
-
-def get_prev_hist(cpu_counts, prev_hist, is_valid_node):
-    nbins = prev_hist.shape[-1]
-    magic_constant = 20
-
-    is_max = cpu_counts.reshape((-1, 2)).argsort(axis=1).astype(np.bool_).ravel()
-    valid = is_max & (cpu_counts > nbins)
-
-    bigger_pos = np.arange(valid.shape[0])[valid]
-    smaller_pos = np.arange(valid.shape[0])[~valid]
-
-    if cpu_counts[valid].sum() > (nbins * magic_constant):
-        return None, None, None
-
-    bigger_pos = cp.asarray(bigger_pos)
-    smaller_pos = cp.asarray(smaller_pos)
-
-    hist_idx = cp.arange(prev_hist.shape[1])[is_valid_node][bigger_pos // 2]
-
-    prev_hist = prev_hist[:, hist_idx]
-
-    return prev_hist, smaller_pos, bigger_pos
-
-
-apply_values_kernel = cp.ElementwiseKernel(
-    """
-    uint64 row_indexer,
-    uint64 grp_index,
-
-    raw int32 nodes,
-    raw T values,
-    uint64 ngroups,
-    uint64 nout
-    """,
-    'T pred',
-
-    """
-    int out = i % nout;
-    int node = nodes[row_indexer * ngroups + grp_index];
-    pred = values[node * nout + out];
-
-    """,
-
-    'apply_values_kernel') if CUDA_FOUND else None
-
-
-def apply_values(nodes, group_index, values):
-    row_indexer = cp.arange(nodes.shape[0], dtype=cp.uint64)
-    ngroups = nodes.shape[1]
-    nout = group_index.shape[0]
-
-    return apply_values_kernel(row_indexer[:, cp.newaxis], group_index[cp.newaxis, :], nodes,
-                               values, ngroups, nout)
-
-
-node_index_kernel = cp.ElementwiseKernel(
-    """
-    uint64 i_,
-    uint64 j_,
-
-    raw T X,
-
-    raw int64 feats,
-    raw float32 val_splits,
-    raw int32 splits,
-    raw bool nan_left,
-
-    uint64 l
-    """,
-    'int32 node',
-
-    """
-    node = 0;
-
-    int f;
-    float x;
-    int right;
-    unsigned long x_ptr;
-
-    while (true) {
-
-        x_ptr = j_ + node;
-        f = feats[x_ptr];
-
-        if (f < 0) {return;}
-
-        x = X[i_ * l + f];
-
-        if (isnan(x)) {
-
-            right = 1 - (int) nan_left[x_ptr];
-
-        } else {
-
-            right = (int) (x > val_splits[x_ptr]);
-
-        }
-
-        node = splits[2 * x_ptr + right];
-
-    }
-
-    """,
-
-    'node_index_kernel') if CUDA_FOUND else None
-
-# if F-contiguous array on GPU
-generic_tree_prediction_leaves_kernel_f = r'''
-    extern "C" __global__
-    void tree_prediction_leaves_kernel_f_{TT}(
-        const {T}* X,
-        const float4* tree,
-        const int* gr_subtree_offsets,
-        const int n_features,
-        const int x_size,
-        const int n_gr,
-        const int n_buffer,
-        int* res)
-    {{
-        long long th = blockIdx.x * blockDim.x + threadIdx.x;
-        long long i_ = th / n_gr;
-        if (i_ >= x_size) {{
-            return;
-        }}
-        int j_ = (int)(th % n_gr);
-
-        int tree_offset = gr_subtree_offsets[j_];
-        int n_node = 0;
-        float4 nd;
-        {T} x;
-        int n_feat_raw;
-
-        // going through the tree
-        while (n_node >= 0) {{
-            nd = tree[tree_offset + n_node];
-
-            n_feat_raw = (int)nd.x;
-            x = X[x_size * (abs(n_feat_raw) - 1) + i_];
-
-            {comp}
-        }}
-
-        // writing result
-        res[i_ * n_buffer + j_] = (-n_node - 1);
-    }}
-    '''
-
-generic_tree_prediction_leaves_kernel = r'''
-    extern "C" __global__
-    void tree_prediction_leaves_kernel_{TT}(
-        const {T}* X,
-        const float4* tree,
-        const int* gr_subtree_offsets,
-        const int n_features,
-        const int x_size,
-        const int n_gr,
-        const int n_buffer, 
-        int* res)
-    {{
-        long long th = blockIdx.x * blockDim.x + threadIdx.x;
-        long long i_ = th / n_gr;
-        if (i_ >= x_size) {{
-            return;
-        }}
-        int j_ = (int)(th % n_gr);
-
-        long long x_feat_offset = n_features * i_;
-        int tree_offset = gr_subtree_offsets[j_];
-        int n_node = 0;
-        float4 nd;
-        {T} x;
-        int n_feat_raw;
-
-        // going through the tree
-        while (n_node >= 0) {{
-            nd = tree[tree_offset + n_node];
-
-            n_feat_raw = (int)nd.x;
-            x = X[x_feat_offset + abs(n_feat_raw) - 1];
-            
-            {comp}
-        }}
-
-        // writing result
-        res[i_ * n_buffer + j_] = (-n_node - 1);
-    }}
-    '''
-
-comp_float = '''
-                if (isnan(x)) {
-                    n_node = (n_feat_raw > 0) ? (int)nd.w : (int)nd.z;
-                } else {
-                    n_node = ((float)x > nd.y) ? (int)nd.w : (int)nd.z;
-                }'''
-comp_int = "n_node = ((float)x > nd.y) ? (int)nd.w : (int)nd.z;"
-tree_prediction_leaves_typed_kernels = {
-    'float32': cp.RawKernel(generic_tree_prediction_leaves_kernel.format(T='float', TT='float', comp=comp_float),
-                            'tree_prediction_leaves_kernel_float') if CUDA_FOUND else None,
-    'float64': cp.RawKernel(generic_tree_prediction_leaves_kernel.format(T='double', TT='double', comp=comp_float),
-                            'tree_prediction_leaves_kernel_double') if CUDA_FOUND else None,
-    'int32': cp.RawKernel(generic_tree_prediction_leaves_kernel.format(T='int', TT='int', comp=comp_int),
-                          'tree_prediction_leaves_kernel_int') if CUDA_FOUND else None,
-    'int64': cp.RawKernel(generic_tree_prediction_leaves_kernel.format(T='long long', TT='longlong', comp=comp_int),
-                          'tree_prediction_leaves_kernel_longlong') if CUDA_FOUND else None
-}
-tree_prediction_leaves_typed_kernels_f = {
-    'float32': cp.RawKernel(generic_tree_prediction_leaves_kernel_f.format(T='float', TT='float', comp=comp_float),
-                            'tree_prediction_leaves_kernel_f_float') if CUDA_FOUND else None,
-    'float64': cp.RawKernel(generic_tree_prediction_leaves_kernel_f.format(T='double', TT='double', comp=comp_float),
-                            'tree_prediction_leaves_kernel_f_double') if CUDA_FOUND else None,
-    'int32': cp.RawKernel(generic_tree_prediction_leaves_kernel_f.format(T='int', TT='int', comp=comp_int),
-                          'tree_prediction_leaves_kernel_f_int') if CUDA_FOUND else None,
-    'int64': cp.RawKernel(generic_tree_prediction_leaves_kernel_f.format(T='long long', TT='longlong', comp=comp_int),
-                          'tree_prediction_leaves_kernel_f_longlong') if CUDA_FOUND else None
-}
-
-tree_prediction_values_kernel = cp.RawKernel(
-    r'''
-    extern "C" __global__
-    void tree_prediction_values_kernel(
-        const int* leaves,
-        const unsigned long long* indexes,
-        const float* values,
-        const int n_out,
-        const int x_size,
-        const int n_gr,
-        float* res)
-    {
-        long long th = blockIdx.x * blockDim.x + threadIdx.x;
-        long long i_ = th / n_out;
-        if (i_ >= x_size) {
-            return;
-        }
-        int i_out = (int)(th % n_out);
-        
-        float prev_val = res[th];
-        int i_gr = indexes[i_out];
-        int val_offset = leaves[(i_ * n_gr) + i_gr] * n_out;
-        float new_val = values[val_offset + i_out];
-        res[th] = prev_val + new_val;
-    }
-    ''',
-    'tree_prediction_values_kernel') if CUDA_FOUND else None
-
-
-def get_tree_node(arr, feats, val_splits, split, nan_left):
-    n_gr, nf = feats.shape
-
-    row_indexer = cp.arange(arr.shape[0], dtype=cp.uint64)[:, cp.newaxis]
-    out_indexer = cp.arange(0, n_gr * nf, nf, dtype=cp.uint64)[cp.newaxis, :]
-
-    nodes = node_index_kernel(row_indexer, out_indexer, arr, feats,
-                              val_splits, split, nan_left, arr.shape[1])
-
-    return nodes
-
-
-def get_cpu_splitters(unique_nodes, best_feat, best_gain, best_split, best_nan_left, min_gain_to_split=0):
-    # print(best_gain.shape, best_gain)
-
-    best_gain = best_gain.get()
-    vs = best_gain > min_gain_to_split
-    n_vs = vs.sum()
-
-    if n_vs == 0:
-        return [], None, None, None, None, None, None
-
-    best_feat = best_feat.get()
-    best_split = best_split.get()
-    best_nan_left = best_nan_left.get()
-    last_node = unique_nodes[-1] + 1
-
-    if n_vs < vs.shape[0]:
-        unique_nodes = unique_nodes[vs]
-        best_gain = best_gain[vs]
-        best_feat = best_feat[vs]
-        best_split = best_split[vs]
-        best_nan_left = best_nan_left[vs]
-
-    new_nodes_id = np.arange(last_node, last_node + unique_nodes.shape[0] * 2,
-                             dtype=np.int32).reshape((-1, 2))
-
-    return unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left, vs
-
-
-def get_gpu_splitters(unique_nodes, new_nodes_id, best_feat, best_split, best_nan_left):
-    out = []
-
-    for arr in [unique_nodes, new_nodes_id, best_feat, best_split, best_nan_left]:
-        gpu_arr = cp.asarray(arr)
-        out.append(gpu_arr)
-
-    new_unique_nodes = new_nodes_id.ravel()
-
-    return out, new_unique_nodes
-
-
-def depthwise_grow_tree(tree, group, arr, grad, hess, row_indexer, col_indexer, params, valid_arrs=None):
-    if valid_arrs is None:
-        valid_arrs = []
-
-    # create gh
-    n_out = grad.shape[1]
-    gh = cp.concatenate((grad, hess), axis=1)
-    out_indexer = cp.arange(gh.shape[1], dtype=cp.uint64)
-
-    # init nodes with single zero node
-    unique_nodes = np.zeros(1, dtype=np.int32)
-    # count unique nodes in active rows
-    nodes_count = cp.ones(1, dtype=cp.uint64) * row_indexer.shape[0]
-    # nodes for all rows
-    nodes = cp.zeros(arr.shape[0], dtype=cp.int32)
-    # init valid nodes
-    valid_nodes = [cp.zeros(x.shape[0], dtype=cp.int32) for x in valid_arrs]
-    # index of node in unique array
-    node_indexes = nodes
-    prev_hist, small_index, big_index = [None] * 3
-
-    for niter in range(params['max_depth']):
-
-        nnodes = len(unique_nodes)
-        gh_hist = histogram(arr, gh, node_indexes,
-                            col_indexer=col_indexer,
-                            row_indexer=row_indexer,
-                            out_indexer=out_indexer,
-                            nnodes=nnodes,
-                            max_bins=params['max_bin'],
-                            prev_hist=prev_hist,
-                            small_index=small_index,
-                            big_index=big_index)
-
-        # assume hess is the last output
-        loss = calc_loss(gh_hist[:n_out], gh_hist[n_out:], nodes_count, lambda_l2=params['lambda_l2'],
-                         min_data_in_leaf=params['min_data_in_leaf'])
-
-        if loss.shape[0] > 1:
-            loss = loss.sum(axis=0)
-        else:
-            loss = loss[0]
-
-        best_feat, best_gain, best_split, best_nan_left = get_best_split(loss, col_indexer)
-
-        # move to CPU and apply min_gain_to_split condition
-        unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left, is_valid_node = \
-            get_cpu_splitters(unique_nodes, best_feat, best_gain, best_split, best_nan_left,
-                              params['min_gain_to_split'])
-        # if all nodes are not valid to split - exit
-        if len(unique_nodes) == 0:
-            break
-        # write node info to the Tree
-        tree.set_nodes(group, unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left)
-        # get args back on gpu
-        split_args, unique_nodes = get_gpu_splitters(unique_nodes, new_nodes_id,
-                                                     best_feat, best_split, best_nan_left)
-
-        # perform split for train set
-        nodes, node_indexes = make_split(nodes, arr, *split_args, return_pos=True)
-        # perform split for valid sets
-        valid_nodes = [make_split(x, y, *split_args, return_pos=False) for (x, y) in zip(valid_nodes, valid_arrs)]
-
-        # update info for the next step
-        if niter < (params['max_depth'] - 1):
-            # update counts
-            nodes_count = cp.zeros((unique_nodes.shape[0] + 1,), dtype=np.uint64)
-            nodes_count.scatter_add(node_indexes[row_indexer], 1)
-            nodes_count = nodes_count[:-1]
-            cpu_counts = nodes_count.get()
-
-            # remove unused rows from indexer
-            if cpu_counts.sum() < row_indexer.shape[0]:
-                row_indexer = row_indexer[isin(nodes, split_args[1].ravel(), index=row_indexer)]
-
-            # save histogram for the subs trick
-            prev_hist, small_index, big_index = get_prev_hist(cpu_counts,
-                                                              gh_hist, cp.asarray(is_valid_node))
-
-    return nodes, valid_nodes
-
-
-accumulate_gh_kernel = cp.ElementwiseKernel(
-    """
-    uint64 row_indexer,
-    uint64 group_index, 
-
-    raw float32 grad, 
-    raw float32 hess,
-    raw int32 nodes,
-
-    uint64 nout,
-    uint64 ngroups,
-    uint64 hxst,
-    uint64 hyst
-
-    """,
-    'raw float32 grad_sum, raw float32 hess_sum',
-
-    """
-    int out = i % nout;
-    int node = nodes[row_indexer * ngroups + group_index];
-
-    int y_ptr =  node * nout + out;
-
-    atomicAdd(&grad_sum[y_ptr], grad[row_indexer * nout + out]); 
-    atomicAdd(&hess_sum[y_ptr], hess[row_indexer * hxst + out * hyst]); 
-
-    """,
-
-    'accumulate_gh_kernel') if CUDA_FOUND else None
-
-
-def calc_node_values(grad, hess, nodes, row_indexer, group_index, max_nodes, lr=1, lambda_l2=0.1):
-    """Calculate node values based on grad/hess
-
-    Args:
-        grad:
-        hess:
-        nodes:
-        row_indexer:
-        group_index:
-        max_nodes:
-        lr:
-        lambda_l2:
-
-    Returns:
-
-    """
-    nout = grad.shape[1]
-    ngroups = nodes.shape[1]
-
-    grad_sum = cp.zeros((max_nodes, nout), dtype=cp.float32)
-    hess_sum = cp.zeros((max_nodes, nout), dtype=cp.float32)
-
-    accumulate_gh_kernel(row_indexer[:, cp.newaxis], group_index[cp.newaxis, :], grad, hess, nodes,
-                         nout, ngroups, hess.shape[1], int(hess.shape[1] > 1),
-                         grad_sum, hess_sum)
-
-    node_values = - grad_sum * lr / (hess_sum + lambda_l2)
-
-    return node_values
-
-
-def pinned_array(array):
-    """Move cpu array to the pinned memory
-
-    Args:
-        array: np.ndarray
-
-    Returns:
-        np.ndarray
-    """
-    mem = cp.cuda.alloc_pinned_memory(array.nbytes)
-    src = np.frombuffer(mem, array.dtype, array.size).reshape(array.shape)
-    src[...] = array
-    return src
-
-
-@numba.njit
-def set_leaf_values(feats, split):
-    """Assign leaf indices to the terminal nodes
-
-    Args:
-        feats: np.ndarray of tree's split features, shape (n_groups, max_nodes)
-        split: shape (ngroups, max_nodes, 2) - node indices corresponding left/right split for the current node
-
-    Returns:
-        np.ndarray of leaf indices
-    """
-    leaves = np.zeros(feats.shape[::-1], dtype=np.int32)
-    max_leaves = 0
-
-    for i in range(feats.shape[0]):
-
-        acc = 0
-        
-        nodes = [np.int32(0), ]
-        
-        while len(nodes) > 0:
-            new_nodes = []
-            
-            for n in nodes:
-                if feats[i, n] == -1:
-                    leaves[n, i] = acc
-                    acc += 1
-                else:
-                    new_nodes.extend(split[i, n])
-                    
-            nodes = new_nodes
-        
-        max_leaves = max(max_leaves, acc)
-
-    return leaves, max_leaves
+"""Utilities used for trees building and inference"""
+
+import math
+
+import numba
+import numpy as np
+
+try:
+    import cupy as cp
+
+    CUDA_FOUND = True
+except Exception:
+    CUDA_FOUND = False
+
+
+def validate_input_single(X, y, sample_weight):
+    """Format single dataset to fit py_boost
+
+    Args:
+        X: np.ndarray, features
+        y: np.ndarray, targets
+        sample_weight: np.ndarray or None, sample weights
+
+    Returns:
+        tuple
+    """
+    y = np.asarray(y)
+    if len(y.shape) == 1:
+        y = y[:, np.newaxis]
+
+    X = np.asarray(X)
+    if np.issubdtype(X.dtype, np.integer):
+        X = X.astype(np.float32)
+
+    if (sample_weight is not None) and (len(sample_weight.shape) == 1):
+        sample_weight = sample_weight[:, np.newaxis]
+
+    return X, y, sample_weight
+
+
+def validate_input(X, y, sample_weight=None, eval_sets=None):
+    """Format train and valid datasets to fit py_boost
+
+    Args:
+        X: np.ndarray, features
+        y: np.ndarray, targets
+        sample_weight: np.ndarray or None, sample weights
+        eval_sets: list of dicts, valid datasets
+
+    Returns:
+        tuple
+    """
+    X, y, sample_weight = validate_input_single(X, y, sample_weight)
+
+    if eval_sets is None:
+        eval_sets = []
+    else:
+        eval_sets = list(eval_sets)
+
+    for val_arr in eval_sets:
+        if 'sample_weight' not in val_arr:
+            val_arr['sample_weight'] = None
+
+        val_arr['X'], val_arr['y'], val_arr['sample_weight'] = validate_input_single(
+            val_arr['X'], val_arr['y'], val_arr['sample_weight'])
+
+    return X, y, sample_weight, eval_sets
+
+
+def pad_and_move(arr, pad_size=4):
+    """Pad array memory placeholder to make feature size divisible by pad_size and move to GPU.
+    Returned array is the same size as input, but it is not contiguous.
+    Basic memory placeholder size is divisible by pad_size and could be accesses via arr.base.
+    This trick helps to speed up histogram computation for the large arrays.
+
+    Args:
+        arr: 2d np.ndarray of uint8 containing quantized features matrix
+        pad_size: int, memory placeholder feature size will be divisible by pad_size
+
+    Returns:
+        cp.ndarray of quantized features
+    """
+    assert arr.dtype == np.uint8, 'Array dtype should be unsigned 8bit int'
+
+    pfeats = math.ceil(arr.shape[1] / pad_size) * pad_size
+    arr_cpu_padded = np.zeros((arr.shape[0], pfeats), dtype=np.uint8)
+    arr_cpu_padded[:, :arr.shape[1]] = arr
+    arr_gpu_padded = cp.asarray(arr_cpu_padded)
+
+    return arr_gpu_padded[:, :arr.shape[1]]
+
+
+isin_code = """
+int fnode;
+int leaf = 0;
+int minval = 0;
+int maxval = l - 1;
+
+int node_val = nodes[index];
+
+while (true) {{
+
+    leaf = minval + (maxval - minval) / 2;
+    fnode = un[leaf];
+
+    if (fnode == node_val) {{
+
+        isin={0};
+        return;
+
+    }} else if (minval >= maxval) {{
+
+        isin={1};
+        return ;
+
+    }} else if (fnode < node_val) {{
+
+        minval = leaf + 1;
+
+    }} else  {{
+
+        maxval = leaf - 1;
+
+    }} 
+}}
+
+"""
+
+isin_kernel = cp.ElementwiseKernel(
+    'Q index, raw E nodes, raw R un, uint64 l',
+    'bool isin',
+
+    isin_code.format('true', 'false'),
+
+    'isin_kernel'
+) if CUDA_FOUND else None
+
+isin_pos_kernel = cp.ElementwiseKernel(
+    'Q index, raw E nodes, raw R un, uint64 l',
+    'int32 isin',
+
+    isin_code.format('leaf', -1),
+
+    'isin_pos_kernel'
+) if CUDA_FOUND else None
+
+
+def isin(a, b, index=None, return_pos=False):
+    """Check if b contains elements of a. Custom function is faster than build in cupy's
+
+    Args:
+        a: cp.ndarray to apply
+        b: cp.ndarray lookup array
+        index: cp.ndarray indices of a to check. If None, check for all a
+        return_pos: bool, if True, return position of a[i] in b, otherwise return bool array if a[i] is in b
+
+    Returns:
+        cp.ndarray of bool or int
+    """
+    if index is None:
+        index = cp.arange(a.shape[0], dtype=cp.uint64)
+
+    if return_pos:
+        return isin_pos_kernel(index, a, b, b.shape[0])
+    else:
+        return isin_kernel(index, a, b, b.shape[0])
+
+
+histogram_kernel_idx = cp.ElementwiseKernel(
+    """
+    uint64 i_, uint64 j_, uint64 k_, 
+    uint64 kk,
+
+    raw uint64 jj,
+    raw bool padded_bool_indexer,
+
+    raw float32 target, 
+    raw T arr, 
+    raw int32 nodes,
+
+    uint64 hlen,
+    uint64 flen, 
+    uint64 length,
+    uint64 feats,
+    uint64 nout 
+    """,
+    'raw float32 hist',
+
+    """
+    unsigned int feat_4t = arr[i_ * feats + j_];
+    int d;
+    int j;
+    int val;
+    int pos;
+    float *x_ptr;
+    float y = target[i_ * nout + k_];
+
+    for (d = 0; d < 4; d++) {
+
+        pos = (i_ + d) % 4;
+
+        if (padded_bool_indexer[j_ * 4 + pos]) {
+
+            val = (feat_4t >> (8 * pos)) % 256;
+            j = jj[j_ * 4 + pos];
+            x_ptr = &hist[0] +  kk * hlen + nodes[i_] * flen + j * length + val;
+            atomicAdd(x_ptr, y); 
+        }
+    }
+
+    """,
+
+    'histogram_kernel_idx') if CUDA_FOUND else None
+
+feature_grouper_kernel = cp.ElementwiseKernel(
+    """
+    uint64 col_indexer
+    """,
+    'raw bool padded_bool_indexer, raw bool tuple_indexer, raw uint64 padded_col_indexer',
+    """
+    int tuple_id = col_indexer / 4;
+    padded_bool_indexer[col_indexer] = true;
+    tuple_indexer[tuple_id] = true;
+    padded_col_indexer[col_indexer] = i;
+
+    """,
+    'feature_grouper_kernel') if CUDA_FOUND else None
+
+
+def fill_histogram(res, arr, target, nodes, col_indexer, row_indexer, out_indexer):
+    """Fill the histogram res
+
+    Args:
+        res: cp.ndarray, histogram of zeros, shape (n_out, n_nodes, n_features, n_bins)
+        arr: cp.ndarray, features array, shape (n_data, n_features)
+        target: cp.ndarray, values to accumulate, shape (n_data, n_out)
+        nodes: cp.ndarray, tree node indices, shape (n_data, )
+        col_indexer: cp.ndarray, indices of features to accumulate
+        row_indexer: cp.ndarray, indices of rows to accumulate
+        out_indexer: cp.ndarray, indices of outputs to accumulate
+
+    Returns:
+
+    """
+    # define data split for kernel launch
+    nout, nnodes, nfeats, nbins = res.shape
+
+    # padded array of 4 feature tuple
+    arr_4t = arr.base.view(dtype=cp.uint32)
+    pfeats = arr_4t.shape[1]
+
+    # create 4 feats tuple indexer
+    padded_bool_indexer = cp.zeros((arr.base.shape[1],), dtype=cp.bool_)
+    padded_col_indexer = cp.zeros((arr.base.shape[1],), dtype=cp.uint64)
+    tuple_indexer = cp.zeros((arr_4t.shape[1],), dtype=cp.bool_)
+
+    feature_grouper_kernel(col_indexer, padded_bool_indexer, tuple_indexer, padded_col_indexer)
+    tuple_indexer = cp.arange(arr_4t.shape[1], dtype=cp.uint64)[tuple_indexer]
+
+    fb = nfeats * nbins
+    nfb = nnodes * fb
+
+    magic_constant = 2 ** 19  # optimal value for my V100
+
+    # split features
+    nsplits = math.ceil(nfb / magic_constant)
+    # first split by feats
+    feats_batch = math.ceil(pfeats / nsplits)
+    # split by features
+    if feats_batch == nfeats:
+        out_batch = magic_constant // nfb
+    else:
+        out_batch = 1
+
+    ri = row_indexer[:, cp.newaxis, cp.newaxis]
+    ti = tuple_indexer[cp.newaxis, :, cp.newaxis]
+    oi = out_indexer[cp.newaxis, cp.newaxis, :]
+
+    oii = cp.arange(oi.shape[2], dtype=cp.uint64)[cp.newaxis, cp.newaxis, :]
+
+    for j in range(0, pfeats, feats_batch):
+        ti_ = ti[:, j: j + feats_batch]
+
+        for k in range(0, nout, out_batch):
+            oi_ = oi[..., k: k + out_batch]
+            oii_ = oii[..., k: k + out_batch]
+
+            histogram_kernel_idx(ri, ti_, oi_,
+                                 oii_,
+                                 padded_col_indexer,
+                                 padded_bool_indexer,
+                                 target,
+                                 arr_4t,
+                                 nodes,
+                                 nfb, fb, nbins, arr_4t.shape[1], nout,
+                                 res)
+
+
+def histogram(arr, gh, nodes, col_indexer, row_indexer, out_indexer, nnodes, max_bins,
+              prev_hist=None, small_index=None, big_index=None):
+    """Compute grad/hess histogram
+
+    Args:
+        arr: cp.ndarray, features array, shape (n_data, n_features)
+        gh: cp.ndarray of grad/hess, shape (n_data, n_out + 1), assume the last output is hess, others for grads
+        nodes: cp.ndarray, tree node indices, shape (n_data, )
+        col_indexer: cp.ndarray, indices of features to accumulate
+        row_indexer: cp.ndarray, indices of rows to accumulate
+        out_indexer: cp.ndarray, indices of outputs to accumulate
+        nnodes: int, total number of nodes in the sample
+        max_bins: int, maximum number of feature bins
+        prev_hist: cp.ndarray or None, histogram from previous step to apply histogram subtraction trick
+        small_index: cp.ndarray or None, node indices to accumulate
+        big_index: cp.ndarray or None, node indices to compute by subtraction from prev_hist
+
+    Returns:
+        cp.ndarray, histogram of shape (n_out + 1, n_nodes, n_features, n_bins)
+    """
+
+    nout = out_indexer.shape[0]
+    nfeats = col_indexer.shape[0]
+    # init union histogram for grad and hess
+    # we assume, we have 1 dim hess for one output group
+
+    res = cp.zeros((nout, nnodes, nfeats, max_bins), dtype=cp.float32)
+
+    if prev_hist is not None:
+        row_indexer = row_indexer[isin(nodes, small_index, row_indexer)]
+
+    fill_histogram(res, arr, gh, nodes, col_indexer, row_indexer, out_indexer)
+    res = res.cumsum(axis=-1)
+
+    if prev_hist is not None:
+        # indices are paired.
+        res[:, big_index] = prev_hist - res[:, big_index + (1 - 2 * (big_index % 2))]
+
+    return res
+
+
+loss_kernel = cp.ElementwiseKernel(
+    # inputs
+    """
+    float32 grad, float32 hess, 
+    float32 total_grad, float32 total_hess, 
+    float32 nan_grad, float32 nan_hess, 
+
+    uint64 nodes_count, 
+    float32 lambda_l2, float32 min_data_in_left
+    """,
+    # output
+    'raw float32 res',
+
+    # kernel
+    """
+    float rG;
+    float G = grad;
+    float H = hess;
+    float C = hess / total_hess * nodes_count;
+    float prev = total_grad * total_grad / (total_hess + lambda_l2);
+
+
+    if (fmin(nodes_count - C, C) > min_data_in_left) {
+        rG = total_grad - G;
+        res[2 * i] = G * G / (H + lambda_l2) + rG * rG / (total_hess - H + lambda_l2) - prev;
+    }
+
+    if ((nan_hess > 0) and (hess < total_hess)) {
+
+        C -= nan_hess / total_hess * nodes_count;
+        if (fmin(nodes_count - C, C) > min_data_in_left) {
+
+            G -= nan_grad;
+            H -= nan_hess;
+            rG = total_grad - G;
+            res[2 * i + 1] = G * G / (H + lambda_l2) + rG * rG / (total_hess - H + lambda_l2) - prev;
+
+        }
+    }
+
+    """,
+
+    'loss_kernel') if CUDA_FOUND else None
+
+
+def calc_loss(grad, hess, nodes_count, lambda_l2=0.1, min_data_in_leaf=10.):
+    """Calculate loss function
+
+    Args:
+        grad:
+        hess:
+        nodes_count:
+        lambda_l2:
+        min_data_in_leaf:
+
+    Returns:
+
+    """
+    # fill loss
+    res = cp.zeros(grad.shape + (2,), dtype=cp.float32)
+    loss_kernel(grad, hess,
+                grad[..., -1:], hess[..., -1:],
+                grad[..., :1], hess[..., :1],
+                nodes_count[cp.newaxis, :, cp.newaxis, cp.newaxis],
+                lambda_l2, min_data_in_leaf, res)
+
+    return res
+
+
+select_among_feature = cp.ElementwiseKernel(
+    """
+    int64 best_idx, 
+    raw float32 loss,
+    uint64 binsx2
+    """,
+    'float32 best_gain, int32 best_split, bool best_nan_left',
+
+    """
+    best_gain = loss[i * binsx2 + best_idx];
+    best_split = best_idx / 2;
+    best_nan_left = (bool) (1 - best_idx % 2);
+
+    """,
+
+    'select_among_feature') if CUDA_FOUND else None
+
+select_total = cp.ElementwiseKernel(
+    """
+    int64 best_idx,
+    raw float32 feat_loss,
+    raw int32 feat_split,
+    raw bool feat_nan_left,
+    raw uint64 col_indexer, 
+
+    uint64 feats
+    """,
+    'int64 best_feat, float32 best_gain, int32 best_split, bool best_nan_left',
+
+    """
+    unsigned long f_ptr = i * feats + best_idx;
+
+    best_gain = feat_loss[f_ptr];
+    best_split = feat_split[f_ptr];
+    best_nan_left = feat_nan_left[f_ptr];
+    best_feat = col_indexer[best_idx];
+
+    """,
+
+    'select_total') if CUDA_FOUND else None
+
+
+def get_best_split(loss, col_indexer):
+    nnodes, nfeats, nbins, _ = loss.shape
+    # shape - nnodes * nfeats
+    best_loss_among_feat_idx = loss.reshape((nnodes, nfeats, -1)).argmax(axis=-1)
+
+    best_gain, best_split, best_nan_left = \
+        select_among_feature(
+            best_loss_among_feat_idx, loss, nbins * 2
+        )
+
+    best_feat_ = best_gain.argmax(axis=-1)
+
+    best_feat, best_gain, best_split, best_nan_left = \
+        select_total(
+            best_feat_, best_gain, best_split, best_nan_left, col_indexer, nfeats
+        )
+
+    return best_feat, best_gain, best_split, best_nan_left
+
+
+split_kernel = cp.ElementwiseKernel(
+    """
+    int32 nodes_index,
+    int32 nodes_old,
+    raw uint8 arr,
+    raw int32 split_nodes,
+    raw int64 feat,
+    raw int32 split,
+    raw bool nan_left,
+    uint64 F
+    """,
+    'int32 nodes',
+
+    """
+    if (nodes_index >= 0) {
+
+        int f = feat[nodes_index];
+        int s = split[nodes_index];
+        bool nl = nan_left[nodes_index];
+
+        int val = arr[i * F + f];
+
+        int d = 0;
+        if ((val > s) or ((val == 0) and (not nl))) {d = 1;}
+
+        nodes = split_nodes[2 * nodes_index + d];
+
+    } else {nodes=nodes_old;}
+
+    """,
+
+    'split_kernel') if CUDA_FOUND else None
+
+
+def make_split(nodes, arr, unique_nodes, split_nodes, feat, split, nan_left, return_pos=False):
+    nodes_index = isin(nodes, unique_nodes, return_pos=True)
+    new_nodes = split_kernel(nodes_index, nodes, arr, split_nodes, feat, split, nan_left, arr.shape[1])
+
+    if return_pos:
+        nodes_index = isin(new_nodes, split_nodes.ravel(), return_pos=True)
+        return new_nodes, nodes_index
+
+    return new_nodes
+
+
+def get_prev_hist(cpu_counts, prev_hist, is_valid_node):
+    nbins = prev_hist.shape[-1]
+    magic_constant = 20
+
+    is_max = cpu_counts.reshape((-1, 2)).argsort(axis=1).astype(np.bool_).ravel()
+    valid = is_max & (cpu_counts > nbins)
+
+    bigger_pos = np.arange(valid.shape[0])[valid]
+    smaller_pos = np.arange(valid.shape[0])[~valid]
+
+    if cpu_counts[valid].sum() > (nbins * magic_constant):
+        return None, None, None
+
+    bigger_pos = cp.asarray(bigger_pos)
+    smaller_pos = cp.asarray(smaller_pos)
+
+    hist_idx = cp.arange(prev_hist.shape[1])[is_valid_node][bigger_pos // 2]
+
+    prev_hist = prev_hist[:, hist_idx]
+
+    return prev_hist, smaller_pos, bigger_pos
+
+
+apply_values_kernel = cp.ElementwiseKernel(
+    """
+    uint64 row_indexer,
+    uint64 grp_index,
+
+    raw int32 nodes,
+    raw T values,
+    uint64 ngroups,
+    uint64 nout
+    """,
+    'T pred',
+
+    """
+    int out = i % nout;
+    int node = nodes[row_indexer * ngroups + grp_index];
+    pred = values[node * nout + out];
+
+    """,
+
+    'apply_values_kernel') if CUDA_FOUND else None
+
+
+def apply_values(nodes, group_index, values):
+    row_indexer = cp.arange(nodes.shape[0], dtype=cp.uint64)
+    ngroups = nodes.shape[1]
+    nout = group_index.shape[0]
+
+    return apply_values_kernel(row_indexer[:, cp.newaxis], group_index[cp.newaxis, :], nodes,
+                               values, ngroups, nout)
+
+
+node_index_kernel = cp.ElementwiseKernel(
+    """
+    uint64 i_,
+    uint64 j_,
+
+    raw T X,
+
+    raw int64 feats,
+    raw float32 val_splits,
+    raw int32 splits,
+    raw bool nan_left,
+
+    uint64 l
+    """,
+    'int32 node',
+
+    """
+    node = 0;
+
+    int f;
+    float x;
+    int right;
+    unsigned long x_ptr;
+
+    while (true) {
+
+        x_ptr = j_ + node;
+        f = feats[x_ptr];
+
+        if (f < 0) {return;}
+
+        x = X[i_ * l + f];
+
+        if (isnan(x)) {
+
+            right = 1 - (int) nan_left[x_ptr];
+
+        } else {
+
+            right = (int) (x > val_splits[x_ptr]);
+
+        }
+
+        node = splits[2 * x_ptr + right];
+
+    }
+
+    """,
+
+    'node_index_kernel') if CUDA_FOUND else None
+
+# if F-contiguous array on GPU
+generic_tree_prediction_leaves_kernel_f = r'''
+    extern "C" __global__
+    void tree_prediction_leaves_kernel_f_{TT}(
+        const {T}* X,
+        const float4* tree,
+        const int* gr_subtree_offsets,
+        const int n_features,
+        const int x_size,
+        const int n_gr,
+        const int n_buffer,
+        int* res)
+    {{
+        long long th = blockIdx.x * blockDim.x + threadIdx.x;
+        long long i_ = th / n_gr;
+        if (i_ >= x_size) {{
+            return;
+        }}
+        int j_ = (int)(th % n_gr);
+
+        int tree_offset = gr_subtree_offsets[j_];
+        int n_node = 0;
+        float4 nd;
+        {T} x;
+        int n_feat_raw;
+
+        // going through the tree
+        while (n_node >= 0) {{
+            nd = tree[tree_offset + n_node];
+
+            n_feat_raw = (int)nd.x;
+            x = X[x_size * (abs(n_feat_raw) - 1) + i_];
+
+            {comp}
+        }}
+
+        // writing result
+        res[i_ * n_buffer + j_] = (-n_node - 1);
+    }}
+    '''
+
+generic_tree_prediction_leaves_kernel = r'''
+    extern "C" __global__
+    void tree_prediction_leaves_kernel_{TT}(
+        const {T}* X,
+        const float4* tree,
+        const int* gr_subtree_offsets,
+        const int n_features,
+        const int x_size,
+        const int n_gr,
+        const int n_buffer, 
+        int* res)
+    {{
+        long long th = blockIdx.x * blockDim.x + threadIdx.x;
+        long long i_ = th / n_gr;
+        if (i_ >= x_size) {{
+            return;
+        }}
+        int j_ = (int)(th % n_gr);
+
+        long long x_feat_offset = n_features * i_;
+        int tree_offset = gr_subtree_offsets[j_];
+        int n_node = 0;
+        float4 nd;
+        {T} x;
+        int n_feat_raw;
+
+        // going through the tree
+        while (n_node >= 0) {{
+            nd = tree[tree_offset + n_node];
+
+            n_feat_raw = (int)nd.x;
+            x = X[x_feat_offset + abs(n_feat_raw) - 1];
+            
+            {comp}
+        }}
+
+        // writing result
+        res[i_ * n_buffer + j_] = (-n_node - 1);
+    }}
+    '''
+
+comp_float = '''
+                if (isnan(x)) {
+                    n_node = (n_feat_raw > 0) ? (int)nd.w : (int)nd.z;
+                } else {
+                    n_node = ((float)x > nd.y) ? (int)nd.w : (int)nd.z;
+                }'''
+comp_int = "n_node = ((float)x > nd.y) ? (int)nd.w : (int)nd.z;"
+tree_prediction_leaves_typed_kernels = {
+    'float32': cp.RawKernel(generic_tree_prediction_leaves_kernel.format(T='float', TT='float', comp=comp_float),
+                            'tree_prediction_leaves_kernel_float') if CUDA_FOUND else None,
+    'float64': cp.RawKernel(generic_tree_prediction_leaves_kernel.format(T='double', TT='double', comp=comp_float),
+                            'tree_prediction_leaves_kernel_double') if CUDA_FOUND else None,
+    'int32': cp.RawKernel(generic_tree_prediction_leaves_kernel.format(T='int', TT='int', comp=comp_int),
+                          'tree_prediction_leaves_kernel_int') if CUDA_FOUND else None,
+    'int64': cp.RawKernel(generic_tree_prediction_leaves_kernel.format(T='long long', TT='longlong', comp=comp_int),
+                          'tree_prediction_leaves_kernel_longlong') if CUDA_FOUND else None
+}
+tree_prediction_leaves_typed_kernels_f = {
+    'float32': cp.RawKernel(generic_tree_prediction_leaves_kernel_f.format(T='float', TT='float', comp=comp_float),
+                            'tree_prediction_leaves_kernel_f_float') if CUDA_FOUND else None,
+    'float64': cp.RawKernel(generic_tree_prediction_leaves_kernel_f.format(T='double', TT='double', comp=comp_float),
+                            'tree_prediction_leaves_kernel_f_double') if CUDA_FOUND else None,
+    'int32': cp.RawKernel(generic_tree_prediction_leaves_kernel_f.format(T='int', TT='int', comp=comp_int),
+                          'tree_prediction_leaves_kernel_f_int') if CUDA_FOUND else None,
+    'int64': cp.RawKernel(generic_tree_prediction_leaves_kernel_f.format(T='long long', TT='longlong', comp=comp_int),
+                          'tree_prediction_leaves_kernel_f_longlong') if CUDA_FOUND else None
+}
+
+tree_prediction_values_kernel = cp.RawKernel(
+    r'''
+    extern "C" __global__
+    void tree_prediction_values_kernel(
+        const int* leaves,
+        const unsigned long long* indexes,
+        const float* values,
+        const int n_out,
+        const int x_size,
+        const int n_gr,
+        float* res)
+    {
+        long long th = blockIdx.x * blockDim.x + threadIdx.x;
+        long long i_ = th / n_out;
+        if (i_ >= x_size) {
+            return;
+        }
+        int i_out = (int)(th % n_out);
+        
+        float prev_val = res[th];
+        int i_gr = indexes[i_out];
+        int val_offset = leaves[(i_ * n_gr) + i_gr] * n_out;
+        float new_val = values[val_offset + i_out];
+        res[th] = prev_val + new_val;
+    }
+    ''',
+    'tree_prediction_values_kernel') if CUDA_FOUND else None
+
+
+def get_tree_node(arr, feats, val_splits, split, nan_left):
+    n_gr, nf = feats.shape
+
+    row_indexer = cp.arange(arr.shape[0], dtype=cp.uint64)[:, cp.newaxis]
+    out_indexer = cp.arange(0, n_gr * nf, nf, dtype=cp.uint64)[cp.newaxis, :]
+
+    nodes = node_index_kernel(row_indexer, out_indexer, arr, feats,
+                              val_splits, split, nan_left, arr.shape[1])
+
+    return nodes
+
+
+def get_cpu_splitters(unique_nodes, best_feat, best_gain, best_split, best_nan_left, min_gain_to_split=0):
+    # print(best_gain.shape, best_gain)
+
+    best_gain = best_gain.get()
+    vs = best_gain > min_gain_to_split
+    n_vs = vs.sum()
+
+    if n_vs == 0:
+        return [], None, None, None, None, None, None
+
+    best_feat = best_feat.get()
+    best_split = best_split.get()
+    best_nan_left = best_nan_left.get()
+    last_node = unique_nodes[-1] + 1
+
+    if n_vs < vs.shape[0]:
+        unique_nodes = unique_nodes[vs]
+        best_gain = best_gain[vs]
+        best_feat = best_feat[vs]
+        best_split = best_split[vs]
+        best_nan_left = best_nan_left[vs]
+
+    new_nodes_id = np.arange(last_node, last_node + unique_nodes.shape[0] * 2,
+                             dtype=np.int32).reshape((-1, 2))
+
+    return unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left, vs
+
+
+def get_gpu_splitters(unique_nodes, new_nodes_id, best_feat, best_split, best_nan_left):
+    out = []
+
+    for arr in [unique_nodes, new_nodes_id, best_feat, best_split, best_nan_left]:
+        gpu_arr = cp.asarray(arr)
+        out.append(gpu_arr)
+
+    new_unique_nodes = new_nodes_id.ravel()
+
+    return out, new_unique_nodes
+
+
+def depthwise_grow_tree(tree, group, arr, grad, hess, row_indexer, col_indexer, params, valid_arrs=None):
+    if valid_arrs is None:
+        valid_arrs = []
+
+    # create gh
+    n_out = grad.shape[1]
+    gh = cp.concatenate((grad, hess), axis=1)
+    out_indexer = cp.arange(gh.shape[1], dtype=cp.uint64)
+
+    # init nodes with single zero node
+    unique_nodes = np.zeros(1, dtype=np.int32)
+    # count unique nodes in active rows
+    nodes_count = cp.ones(1, dtype=cp.uint64) * row_indexer.shape[0]
+    # nodes for all rows
+    nodes = cp.zeros(arr.shape[0], dtype=cp.int32)
+    # init valid nodes
+    valid_nodes = [cp.zeros(x.shape[0], dtype=cp.int32) for x in valid_arrs]
+    # index of node in unique array
+    node_indexes = nodes
+    prev_hist, small_index, big_index = [None] * 3
+
+    for niter in range(params['max_depth']):
+
+        nnodes = len(unique_nodes)
+        gh_hist = histogram(arr, gh, node_indexes,
+                            col_indexer=col_indexer,
+                            row_indexer=row_indexer,
+                            out_indexer=out_indexer,
+                            nnodes=nnodes,
+                            max_bins=params['max_bin'],
+                            prev_hist=prev_hist,
+                            small_index=small_index,
+                            big_index=big_index)
+
+        # assume hess is the last output
+        loss = calc_loss(gh_hist[:n_out], gh_hist[n_out:], nodes_count, lambda_l2=params['lambda_l2'],
+                         min_data_in_leaf=params['min_data_in_leaf'])
+
+        if loss.shape[0] > 1:
+            loss = loss.sum(axis=0)
+        else:
+            loss = loss[0]
+
+        best_feat, best_gain, best_split, best_nan_left = get_best_split(loss, col_indexer)
+
+        # move to CPU and apply min_gain_to_split condition
+        unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left, is_valid_node = \
+            get_cpu_splitters(unique_nodes, best_feat, best_gain, best_split, best_nan_left,
+                              params['min_gain_to_split'])
+        # if all nodes are not valid to split - exit
+        if len(unique_nodes) == 0:
+            break
+        # write node info to the Tree
+        tree.set_nodes(group, unique_nodes, new_nodes_id, best_feat, best_gain, best_split, best_nan_left)
+        # get args back on gpu
+        split_args, unique_nodes = get_gpu_splitters(unique_nodes, new_nodes_id,
+                                                     best_feat, best_split, best_nan_left)
+
+        # perform split for train set
+        nodes, node_indexes = make_split(nodes, arr, *split_args, return_pos=True)
+        # perform split for valid sets
+        valid_nodes = [make_split(x, y, *split_args, return_pos=False) for (x, y) in zip(valid_nodes, valid_arrs)]
+
+        # update info for the next step
+        if niter < (params['max_depth'] - 1):
+            # update counts
+            nodes_count = cp.zeros((unique_nodes.shape[0] + 1,), dtype=np.uint64)
+            nodes_count.scatter_add(node_indexes[row_indexer], 1)
+            nodes_count = nodes_count[:-1]
+            cpu_counts = nodes_count.get()
+
+            # remove unused rows from indexer
+            if cpu_counts.sum() < row_indexer.shape[0]:
+                row_indexer = row_indexer[isin(nodes, split_args[1].ravel(), index=row_indexer)]
+
+            # save histogram for the subs trick
+            prev_hist, small_index, big_index = get_prev_hist(cpu_counts,
+                                                              gh_hist, cp.asarray(is_valid_node))
+
+    return nodes, valid_nodes
+
+
+accumulate_gh_kernel = cp.ElementwiseKernel(
+    """
+    uint64 row_indexer,
+    uint64 group_index, 
+
+    raw float32 grad, 
+    raw float32 hess,
+    raw int32 nodes,
+
+    uint64 nout,
+    uint64 ngroups,
+    uint64 hxst,
+    uint64 hyst
+
+    """,
+    'raw float32 grad_sum, raw float32 hess_sum',
+
+    """
+    int out = i % nout;
+    int node = nodes[row_indexer * ngroups + group_index];
+
+    int y_ptr =  node * nout + out;
+
+    atomicAdd(&grad_sum[y_ptr], grad[row_indexer * nout + out]); 
+    atomicAdd(&hess_sum[y_ptr], hess[row_indexer * hxst + out * hyst]); 
+
+    """,
+
+    'accumulate_gh_kernel') if CUDA_FOUND else None
+
+
+def calc_node_values(grad, hess, nodes, row_indexer, group_index, max_nodes, lr=1, lambda_l2=0.1):
+    """Calculate node values based on grad/hess
+
+    Args:
+        grad:
+        hess:
+        nodes:
+        row_indexer:
+        group_index:
+        max_nodes:
+        lr:
+        lambda_l2:
+
+    Returns:
+
+    """
+    nout = grad.shape[1]
+    ngroups = nodes.shape[1]
+
+    grad_sum = cp.zeros((max_nodes, nout), dtype=cp.float32)
+    hess_sum = cp.zeros((max_nodes, nout), dtype=cp.float32)
+
+    accumulate_gh_kernel(row_indexer[:, cp.newaxis], group_index[cp.newaxis, :], grad, hess, nodes,
+                         nout, ngroups, hess.shape[1], int(hess.shape[1] > 1),
+                         grad_sum, hess_sum)
+
+    node_values = - grad_sum * lr / (hess_sum + lambda_l2)
+
+    return node_values
+
+
+def pinned_array(array):
+    """Move cpu array to the pinned memory
+
+    Args:
+        array: np.ndarray
+
+    Returns:
+        np.ndarray
+    """
+    mem = cp.cuda.alloc_pinned_memory(array.nbytes)
+    src = np.frombuffer(mem, array.dtype, array.size).reshape(array.shape)
+    src[...] = array
+    return src
+
+
+@numba.njit
+def set_leaf_values(feats, split):
+    """Assign leaf indices to the terminal nodes
+
+    Args:
+        feats: np.ndarray of tree's split features, shape (n_groups, max_nodes)
+        split: shape (ngroups, max_nodes, 2) - node indices corresponding left/right split for the current node
+
+    Returns:
+        np.ndarray of leaf indices
+    """
+    leaves = np.zeros(feats.shape[::-1], dtype=np.int32)
+    max_leaves = 0
+
+    for i in range(feats.shape[0]):
+
+        acc = 0
+
+        nodes = [np.int32(0), ]
+
+        while len(nodes) > 0:
+            new_nodes = []
+
+            for n in nodes:
+                if feats[i, n] == -1:
+                    leaves[n, i] = acc
+                    acc += 1
+                else:
+                    new_nodes.extend(split[i, n])
+
+            nodes = new_nodes
+
+        max_leaves = max(max_leaves, acc)
+
+    return leaves, max_leaves
```

### Comparing `py_boost-0.4.3/py_boost/quantization/utils.py` & `py_boost-0.5.0/py_boost/quantization/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,155 +1,157 @@
-"""Quantization utilities"""
-
-import numba
-import numpy as np
-from numba import float32, float64, uint8, prange, njit, int64
-
-numba.config.THREADING_LAYER = 'threadsafe'
-
-
-def _apply_borders_1d(x_raw, x_enc, borders):
-    # encode raw values
-    sl = ~np.isnan(x_raw)
-    x_enc[sl] = np.searchsorted(borders, x_raw[sl])
-
-    return
-
-
-sign = [(float64[:], uint8[:], float64[:]),
-        (float32[:], uint8[:], float32[:]),
-        ]
-
-numba_apply_borders_1d = njit(sign, parallel=False)(_apply_borders_1d)
-
-
-def _apply_borders(X, X_enc, borders):
-    for i in prange(X.shape[1]):
-        numba_apply_borders_1d(X[:, i], X_enc[:, i], borders[i])
-
-    return
-
-
-numba_apply_borders = njit(parallel=True)(_apply_borders)
-
-
-def apply_borders(X, borders):
-    X_enc = np.zeros_like(X, dtype=np.uint8, order='C')
-    numba_apply_borders(X, X_enc, numba.typed.List(borders))
-
-    return X_enc
-
-
-def _preprocess_1d(x_sample):
-    x_sample = x_sample[~np.isnan(x_sample)].copy()
-    neg_inf_clip_value = np.finfo(x_sample).min
-    x_sample[x_sample < neg_inf_clip_value] = neg_inf_clip_value
-    x_sample = np.sort(x_sample)
-
-    return x_sample
-
-
-sign = [(float64[:],), (float32[:],), ]
-numba_preprocess_1d = njit(sign, parallel=False)(_preprocess_1d)
-
-
-def _quantile_1d(x_sample, max_bins, min_data_in_bin):
-    x_sample = numba_preprocess_1d(x_sample)
-    bins = np.unique(x_sample)[:-1]
-
-    if len(bins) > (max_bins - 1):
-        # get quantiles
-        grid = (np.linspace(0, 1, max_bins + 1) * x_sample.shape[0])[1:-1].astype(np.int64)
-        bins = x_sample[grid]
-        bins = np.unique(bins)
-
-    return bins
-
-
-q1d_sign = [(float64[:], int64, int64),
-            (float32[:], int64, int64),
-            ]
-
-numba_quantile_1d = njit(q1d_sign, parallel=False)(_quantile_1d)
-
-
-def _quantize_features(fn, X, max_bins, min_data_in_bin, borders):
-    """
-    Args:
-        X:
-
-    Returns:
-    """
-    for i in prange(X.shape[1]):
-        bins = fn(X[:, i], max_bins, min_data_in_bin)
-        borders[i, 1: len(bins) + 1] = bins
-
-    return borders
-
-
-numba_quantize_features = njit(parallel=True)(_quantize_features)
-
-
-def quantize_features(fn, X, max_bins=255, min_data_in_bin=3):
-    """
-    Perform feature quantization
-    Args:
-        fn: JIT compiled function for 1d quantization
-        X: np.ndarray, raw features
-        max_bins: int, maximum number of bins, <= 255
-        min_data_in_bin: int, sample size for bins construction
-    Returns:
-    """
-    assert 0 < max_bins <= 255, 'Max bins should be between 0 and 255'
-
-    borders_ = np.empty((X.shape[1], max_bins + 1), dtype=X.dtype)
-    borders_[:] = np.nan
-    borders_[:, 0] = -np.inf
-
-    numba_quantize_features(fn, X, max_bins, min_data_in_bin, borders_)
-    borders = []
-
-    for i in range(X.shape[1]):
-        j = 0
-        for j in range(max_bins + 1):
-            val = borders_[i, j]
-            if np.isnan(val):
-                break
-        borders_[i, j] = np.inf
-        borders.append(borders_[i, :j + 1])
-
-    return borders
-
-
-def _uniform_1d(x_sample, max_bins, min_data_in_bin):
-    x_sample = numba_preprocess_1d(x_sample)
-    bins = np.unique(x_sample)[:-1]
-
-    if len(bins) > (max_bins - 1):
-        # get uniform
-        bins = np.linspace(x_sample[0], x_sample[-1], max_bins + 1)[1:-1].astype(x_sample.dtype)
-
-    return bins
-
-
-numba_uniform_1d = njit(q1d_sign, parallel=False)(_uniform_1d)
-
-
-def _uniquant_1d(x_sample, max_bins, min_data_in_bin):
-    x_sample = numba_preprocess_1d(x_sample)
-    bins = np.unique(x_sample)[:-1]
-
-    if len(bins) > (max_bins - 1):
-        # get uniform
-        max_bins_u = max_bins // 2
-        bins_u = np.linspace(x_sample[0], x_sample[-1], max_bins_u + 1)[1:-1].astype(x_sample.dtype)
-        # get quantile
-        max_bins_q = max_bins - max_bins_u
-        grid = (np.linspace(0, 1, max_bins_q + 1) * x_sample.shape[0])[1:-1].astype(np.int64)
-        bins_q = x_sample[grid]
-        # merge
-        bins = np.unique(np.concatenate((bins_u, bins_q)))
-
-    return bins
-
-
-numba_uniquant_1d = njit(q1d_sign, parallel=False)(_uniquant_1d)
+"""Quantization utilities"""
+
+import numba
+import numpy as np
+from numba import float32, float64, uint8, prange, njit, int64
+
+numba.config.THREADING_LAYER = 'threadsafe'
+
+
+def _apply_borders_1d(x_raw, x_enc, borders):
+    # encode raw values
+    sl = np.nonzero(~np.isnan(x_raw))[0]
+    x_enc[sl] = np.searchsorted(borders, x_raw[sl])
+
+    return
+
+
+sign = [(float64[:], uint8[:], float64[:]),
+        (float32[:], uint8[:], float32[:]),
+        ]
+
+numba_apply_borders_1d = njit(sign, parallel=False)(_apply_borders_1d)
+
+
+def _apply_borders(X, X_enc, borders):
+    for i in prange(X.shape[1]):
+        i = int64(i)  # to prevent unsafe cast numba warning
+        numba_apply_borders_1d(X[:, i], X_enc[:, i], borders[i])
+
+    return
+
+
+numba_apply_borders = njit(parallel=True)(_apply_borders)
+
+
+def apply_borders(X, borders):
+    X_enc = np.zeros_like(X, dtype=np.uint8, order='C')
+    numba_apply_borders(X, X_enc, numba.typed.List(borders))
+
+    return X_enc
+
+
+def _preprocess_1d(x_sample):
+    x_sample = x_sample[~np.isnan(x_sample)].copy()
+    neg_inf_clip_value = np.finfo(x_sample).min
+    x_sample[x_sample < neg_inf_clip_value] = neg_inf_clip_value
+    x_sample = np.sort(x_sample)
+
+    return x_sample
+
+
+sign = [(float64[:],), (float32[:],), ]
+numba_preprocess_1d = njit(sign, parallel=False)(_preprocess_1d)
+
+
+def _quantile_1d(x_sample, max_bins, min_data_in_bin):
+    x_sample = numba_preprocess_1d(x_sample)
+    bins = np.unique(x_sample)[:-1]
+
+    if len(bins) > (max_bins - 1):
+        # get quantiles
+        grid = (np.linspace(0, 1, max_bins + 1) * x_sample.shape[0])[1:-1].astype(np.int64)
+        bins = x_sample[grid]
+        bins = np.unique(bins)
+
+    return bins
+
+
+q1d_sign = [(float64[:], int64, int64),
+            (float32[:], int64, int64),
+            ]
+
+numba_quantile_1d = njit(q1d_sign, parallel=False)(_quantile_1d)
+
+
+def _quantize_features(fn, X, max_bins, min_data_in_bin, borders):
+    """
+    Args:
+        X:
+
+    Returns:
+    """
+    for i in prange(X.shape[1]):
+        bins = fn(X[:, i], max_bins, min_data_in_bin)
+        borders[i, 1: len(bins) + 1] = bins
+
+    return borders
+
+
+numba_quantize_features = njit(parallel=True)(_quantize_features)
+
+
+def quantize_features(fn, X, max_bins=255, min_data_in_bin=3):
+    """
+    Perform feature quantization
+    Args:
+        fn: JIT compiled function for 1d quantization
+        X: np.ndarray, raw features
+        max_bins: int, maximum number of bins, <= 255
+        min_data_in_bin: int, sample size for bins construction
+    Returns:
+    """
+    assert 0 < max_bins <= 255, 'Max bins should be between 0 and 255'
+    assert min_data_in_bin > 0, 'Min data in bin should be > 0'
+
+    borders_ = np.empty((X.shape[1], max_bins + 1), dtype=X.dtype)
+    borders_[:] = np.nan
+    borders_[:, 0] = -np.inf
+
+    numba_quantize_features(fn, X, max_bins, min_data_in_bin, borders_)
+    borders = []
+
+    for i in range(X.shape[1]):
+        j = 0
+        for j in range(max_bins + 1):
+            val = borders_[i, j]
+            if np.isnan(val):
+                break
+        borders_[i, j] = np.inf
+        borders.append(borders_[i, :j + 1])
+
+    return borders
+
+
+def _uniform_1d(x_sample, max_bins, min_data_in_bin):
+    x_sample = numba_preprocess_1d(x_sample)
+    bins = np.unique(x_sample)[:-1]
+
+    if len(bins) > (max_bins - 1):
+        # get uniform
+        bins = np.linspace(x_sample[0], x_sample[-1], max_bins + 1)[1:-1].astype(x_sample.dtype)
+
+    return bins
+
+
+numba_uniform_1d = njit(q1d_sign, parallel=False)(_uniform_1d)
+
+
+def _uniquant_1d(x_sample, max_bins, min_data_in_bin):
+    x_sample = numba_preprocess_1d(x_sample)
+    bins = np.unique(x_sample)[:-1]
+
+    if len(bins) > (max_bins - 1):
+        # get uniform
+        max_bins_u = max_bins // 2
+        bins_u = np.linspace(x_sample[0], x_sample[-1], max_bins_u + 1)[1:-1].astype(x_sample.dtype)
+        # get quantile
+        max_bins_q = max_bins - max_bins_u
+        grid = (np.linspace(0, 1, max_bins_q + 1) * x_sample.shape[0])[1:-1].astype(np.int64)
+        bins_q = x_sample[grid]
+        # merge
+        bins = np.unique(np.concatenate((bins_u, bins_q)))
+
+    return bins
+
+
+numba_uniquant_1d = njit(q1d_sign, parallel=False)(_uniquant_1d)
```

### Comparing `py_boost-0.4.3/py_boost/sampling/bagging.py` & `py_boost-0.5.0/py_boost/sampling/bagging.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-"""Basic sampling strategy"""
-
-import numpy as np
-try:
-    import cupy as cp
-except Exception:
-    pass
-from ..callbacks.callback import Callback
-
-
-class BaseSampler(Callback):
-    """Random uniform rows/columns sampler"""
-
-    def __init__(self, sample=1, axis=0):
-        """
-
-        Args:
-            sample: subsample to select at each iteration
-            axis: int, 0 for rows, 1 for columns
-        """
-        self.sample = sample
-        self.axis = axis
-        self.length = None
-        self.valid_sl = None
-        self.indexer = None
-
-    def before_train(self, build_info):
-        """Create indexers
-
-        Args:
-            build_info: dict
-
-        Returns:
-
-        """
-        self.length = build_info['data']['train']['features_gpu'].shape[self.axis]
-        self.indexer = cp.arange(self.length, dtype=cp.uint64)
-        if self.sample < 1:
-            self.valid_sl = cp.zeros(self.length, dtype=cp.bool_)
-            self.valid_sl[:max(1, int(self.length * self.sample))] = True
-
-    def before_iteration(self, build_info):
-        """Shuffle indexers
-
-        Args:
-            build_info: dict
-
-        Returns:
-
-        """
-        if self.sample < 1:
-            cp.random.shuffle(self.valid_sl)
-
-    def __call__(self):
-        """Get the last actual indexer
-
-        Returns:
-
-        """
-        if self.sample == 1:
-            return self.indexer
-
-        return self.indexer[self.valid_sl]
-
-    def after_train(self, build_info):
-        """Clean the state
-
-        Args:
-            build_info:
-
-        Returns:
-
-        """
-        self.__init__(sample=self.sample, axis=self.axis)
-
-
-class MVSSampler(Callback):
-    """
-    MVS rows sampler proposed in
-    https://proceedings.neurips.cc/paper/2019/file/5c8cb735a1ce65dac514233cbd5576d6-Paper.pdf
-    """
-
-    def __init__(self, sample=0.1, lmbd='auto', grid_search_steps=100, grid_multiplier=100):
-        """
-
-        Args:
-            sample: float, subsample
-            lmbd: float or 'auto', lambda hyperparameter
-            grid_search_steps: float, cut off search steps
-            grid_multiplier: float, cut off search multiplier
-        """
-        self.sample = sample
-        self.lmbd = lmbd
-        self.grid_search_steps = grid_search_steps
-        self.grid_multiplier = grid_multiplier
-        self.indexer = None
-
-    def get_probs(self, reg_grad):
-
-        min_ = reg_grad.min()
-
-        grid = cp.linspace(min_, min_ * self.grid_multiplier, self.grid_search_steps, dtype=cp.float32)[cp.newaxis, :]
-
-        probs = cp.clip(reg_grad[:, cp.newaxis] / grid, 0, 1)
-        sample_rates = probs.mean(axis=0)
-        best_idx = cp.abs(sample_rates - self.sample).argmin()
-
-        return probs[:, best_idx]
-
-    def before_train(self, build_info):
-
-        return
-
-    def before_iteration(self, build_info):
-
-        train = build_info['data']['train']
-        grad, hess = train['grad'], train['hess']
-
-        if self.lmbd == 'auto':
-            lmbd = ((grad.sum() / hess.sum()) ** 2).sum()
-        else:
-            lmbd = self.lmbd
-
-        mult = grad.shape[1] / hess.shape[1]
-
-        reg_grad = cp.sqrt((grad ** 2).sum(axis=1) + lmbd * (hess ** 2).sum(axis=1) * mult)
-
-        probs = self.get_probs(reg_grad)
-
-        build_info['data']['train']['grad'] = grad / probs[:, cp.newaxis]
-        sl = probs >= cp.random.rand(grad.shape[0], dtype=cp.float32)
-        self.indexer = cp.arange(grad.shape[0], dtype=cp.uint64)[sl]
-
-    def __call__(self, *args, **kwargs):
-
-        return self.indexer
-
-    def after_train(self, build_info):
-
-        self.indexer = None
-
-
-class ColumnImportanceSampler(Callback):
-    """
-    This class implements a sampling strategy,
-    that sample columns in proportion to thier importance at each step
-    """
-
-    def __init__(self, rate=0.5, smooth=0.1,
-                 update_freq=10, inverse=False, n_force=None, imp_type='split'):
-        """
-
-        Args:
-            rate: float, sampling rate
-            smooth: float, smoothing parameter
-            update_freq: int importance update frequency
-            inverse: inverse the probability of sampling
-            n_force: int or None, number of feats to ignore by sample (always select), counts from the end of data
-            imp_type: str, importance type
-
-        Returns:
-
-        """
-        self.rate = rate
-        self.smooth = smooth
-        self.update_freq = update_freq
-        self.inverse = inverse
-        self.n_force = n_force
-        self.imp_type = imp_type
-        self.p = None
-        self.imp = None
-
-    def update_importance(self, model):
-
-        if self.imp is None:
-            self.imp = model.get_feature_importance(self.imp_type)
-            return self.imp
-
-        for tree in model.models[-self.update_freq:]:
-            if self.imp_type == 'split':
-                self.imp += tree.feature_importance_split
-            else:
-                self.imp += tree.feature_importance_gain
-
-        return self.imp
-
-    def before_iteration(self, build_info):
-        """
-        Define what should be doe before each iteration
-        """
-        # Update feature importance
-        num_iter = build_info['num_iter']
-
-        if (num_iter % self.update_freq) == 0:
-            # update probabilities with actual importance
-            p = self.update_importance(build_info['model']) + 1e-3
-
-            if self.n_force is not None:
-                p = p[:-self.n_force]
-
-            p = cp.asarray(p) / (p.sum())
-            # inverse if needed
-            if self.inverse:
-                p = 1 - p
-                p = p / p.sum()
-            # apply smoothing
-            self.p = p * (1 - self.smooth) + cp.ones_like(p) * self.smooth / p.shape[0]
-
-    def __call__(self):
-        """
-        Method should return the array of indices, that will be used
-        to grow the tree at the current step
-        """
-        # Sample rows
-        n = self.p.shape[0]
-        index = cp.random.choice(cp.arange(n, dtype=cp.uint64),
-                                 size=int(self.rate * n), p=self.p)
-
-        if self.n_force is not None:
-            index = cp.concatenate([index, cp.arange(n, n + self.n_force, dtype=cp.uint64)])
-
-        return index
-
-    def after_train(self, build_info):
-
-        self.p = None
-        self.imp = None
+"""Basic sampling strategy"""
+
+import numpy as np
+try:
+    import cupy as cp
+except Exception:
+    pass
+from ..callbacks.callback import Callback
+
+
+class BaseSampler(Callback):
+    """Random uniform rows/columns sampler"""
+
+    def __init__(self, sample=1, axis=0):
+        """
+
+        Args:
+            sample: subsample to select at each iteration
+            axis: int, 0 for rows, 1 for columns
+        """
+        self.sample = sample
+        self.axis = axis
+        self.length = None
+        self.valid_sl = None
+        self.indexer = None
+
+    def before_train(self, build_info):
+        """Create indexers
+
+        Args:
+            build_info: dict
+
+        Returns:
+
+        """
+        self.length = build_info['data']['train']['features_gpu'].shape[self.axis]
+        self.indexer = cp.arange(self.length, dtype=cp.uint64)
+        if self.sample < 1:
+            self.valid_sl = cp.zeros(self.length, dtype=cp.bool_)
+            self.valid_sl[:max(1, int(self.length * self.sample))] = True
+
+    def before_iteration(self, build_info):
+        """Shuffle indexers
+
+        Args:
+            build_info: dict
+
+        Returns:
+
+        """
+        if self.sample < 1:
+            cp.random.shuffle(self.valid_sl)
+
+    def __call__(self):
+        """Get the last actual indexer
+
+        Returns:
+
+        """
+        if self.sample == 1:
+            return self.indexer
+
+        return self.indexer[self.valid_sl]
+
+    def after_train(self, build_info):
+        """Clean the state
+
+        Args:
+            build_info:
+
+        Returns:
+
+        """
+        self.__init__(sample=self.sample, axis=self.axis)
+
+
+class MVSSampler(Callback):
+    """
+    MVS rows sampler proposed in
+    https://proceedings.neurips.cc/paper/2019/file/5c8cb735a1ce65dac514233cbd5576d6-Paper.pdf
+    """
+
+    def __init__(self, sample=0.1, lmbd='auto', grid_search_steps=100, grid_multiplier=100):
+        """
+
+        Args:
+            sample: float, subsample
+            lmbd: float or 'auto', lambda hyperparameter
+            grid_search_steps: float, cut off search steps
+            grid_multiplier: float, cut off search multiplier
+        """
+        self.sample = sample
+        self.lmbd = lmbd
+        self.grid_search_steps = grid_search_steps
+        self.grid_multiplier = grid_multiplier
+        self.indexer = None
+
+    def get_probs(self, reg_grad):
+
+        min_ = reg_grad.min()
+
+        grid = cp.linspace(min_, min_ * self.grid_multiplier, self.grid_search_steps, dtype=cp.float32)[cp.newaxis, :]
+
+        probs = cp.clip(reg_grad[:, cp.newaxis] / grid, 0, 1)
+        sample_rates = probs.mean(axis=0)
+        best_idx = cp.abs(sample_rates - self.sample).argmin()
+
+        return probs[:, best_idx]
+
+    def before_train(self, build_info):
+
+        return
+
+    def before_iteration(self, build_info):
+
+        train = build_info['data']['train']
+        grad, hess = train['grad'], train['hess']
+
+        if self.lmbd == 'auto':
+            lmbd = ((grad.sum() / hess.sum()) ** 2).sum()
+        else:
+            lmbd = self.lmbd
+
+        mult = grad.shape[1] / hess.shape[1]
+
+        reg_grad = cp.sqrt((grad ** 2).sum(axis=1) + lmbd * (hess ** 2).sum(axis=1) * mult)
+
+        probs = self.get_probs(reg_grad)
+
+        build_info['data']['train']['grad'] = grad / probs[:, cp.newaxis]
+        sl = probs >= cp.random.rand(grad.shape[0], dtype=cp.float32)
+        self.indexer = cp.arange(grad.shape[0], dtype=cp.uint64)[sl]
+
+    def __call__(self, *args, **kwargs):
+
+        return self.indexer
+
+    def after_train(self, build_info):
+
+        self.indexer = None
+
+
+class ColumnImportanceSampler(Callback):
+    """
+    This class implements a sampling strategy,
+    that sample columns in proportion to thier importance at each step
+    """
+
+    def __init__(self, rate=0.5, smooth=0.1,
+                 update_freq=10, inverse=False, n_force=None, imp_type='split'):
+        """
+
+        Args:
+            rate: float, sampling rate
+            smooth: float, smoothing parameter
+            update_freq: int importance update frequency
+            inverse: inverse the probability of sampling
+            n_force: int or None, number of feats to ignore by sample (always select), counts from the end of data
+            imp_type: str, importance type
+
+        Returns:
+
+        """
+        self.rate = rate
+        self.smooth = smooth
+        self.update_freq = update_freq
+        self.inverse = inverse
+        self.n_force = n_force
+        self.imp_type = imp_type
+        self.p = None
+        self.imp = None
+
+    def update_importance(self, model):
+
+        if self.imp is None:
+            self.imp = model.get_feature_importance(self.imp_type)
+            return self.imp
+
+        for tree in model.models[-self.update_freq:]:
+            if self.imp_type == 'split':
+                self.imp += tree.feature_importance_split
+            else:
+                self.imp += tree.feature_importance_gain
+
+        return self.imp
+
+    def before_iteration(self, build_info):
+        """
+        Define what should be doe before each iteration
+        """
+        # Update feature importance
+        num_iter = build_info['num_iter']
+
+        if (num_iter % self.update_freq) == 0:
+            # update probabilities with actual importance
+            p = self.update_importance(build_info['model']) + 1e-3
+
+            if self.n_force is not None:
+                p = p[:-self.n_force]
+
+            p = cp.asarray(p) / (p.sum())
+            # inverse if needed
+            if self.inverse:
+                p = 1 - p
+                p = p / p.sum()
+            # apply smoothing
+            self.p = p * (1 - self.smooth) + cp.ones_like(p) * self.smooth / p.shape[0]
+
+    def __call__(self):
+        """
+        Method should return the array of indices, that will be used
+        to grow the tree at the current step
+        """
+        # Sample rows
+        n = self.p.shape[0]
+        index = cp.random.choice(cp.arange(n, dtype=cp.uint64),
+                                 size=int(self.rate * n), p=self.p)
+
+        if self.n_force is not None:
+            index = cp.concatenate([index, cp.arange(n, n + self.n_force, dtype=cp.uint64)])
+
+        return index
+
+    def after_train(self, build_info):
+
+        self.p = None
+        self.imp = None
```

### Comparing `py_boost-0.4.3/py_boost/utils/tl_wrapper.py` & `py_boost-0.5.0/py_boost/utils/tl_wrapper.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.3/pyproject.toml` & `py_boost-0.5.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-[tool.poetry]
-name = "Py-Boost"
-version = "0.4.3"
-description = "Python based GBDT"
-
-authors = ["Vakhrushev Anton <btbpanda@gmail.com>",
-           "Iosipoi Leonid",
-           "Sergey Kupriyanov"]
-           
-readme = "README.md"
-
-repository = "https://github.com/AILab-MLTools/Py-Boost"
-classifiers = [
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Science/Research",
-    "Development Status :: 3 - Alpha",
-    "Environment :: Console",
-    "Natural Language :: Russian",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
-
-]
-
-[tool.poetry.dependencies]
-
-python = ">=3.7, <3.11"
-
-scikit-learn = ">=1"
-numpy = "*"
-joblib = "*"
-numba = "*"
-
-pandas = ">=1"
-treelite = [
-    {version = "<3.2,>=3", python = "<3.8"},
-    {version = "^3", python = ">=3.8"}
-]
-treelite_runtime = [
-    {version = "<3.2,>=3", python = "<3.8"},
-    {version = "^3", python = ">=3.8"}
-]
-tqdm = ">=4.64.1"
-
-importlib-metadata = {version = "^1.0", python = "<3.8"}
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
+[tool.poetry]
+name = "Py-Boost"
+version = "0.5.0"
+description = "Python based GBDT"
+
+authors = ["Vakhrushev Anton <btbpanda@gmail.com>",
+    "Iosipoi Leonid",
+    "Sergey Kupriyanov"]
+
+readme = "README.md"
+
+repository = "https://github.com/sb-ai-lab/Py-Boost"
+classifiers = [
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Operating System :: OS Independent",
+    "Intended Audience :: Science/Research",
+    "Development Status :: 3 - Alpha",
+    "Environment :: Console",
+    "Natural Language :: English",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+]
+
+[tool.poetry.dependencies]
+
+python = ">=3.7, <3.11"
+
+scikit-learn = ">=1"
+numpy = "*"
+joblib = "*"
+numba = "*"
+ujson = '*'
+
+pandas = ">=1"
+onnx = ">=1.16, <2"
+onnxruntime = ">=1.16, <2"
+treelite = [
+    { version = "<3.2,>=3", python = "<3.8" },
+    { version = "^3", python = ">=3.8" }
+]
+treelite_runtime = [
+    { version = "<3.2,>=3", python = "<3.8" },
+    { version = "^3", python = ">=3.8" }
+]
+tqdm = ">=4.64.1"
+
+importlib-metadata = { version = "^1.0", python = "<3.8" }
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py_boost-0.4.3/PKG-INFO` & `py_boost-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,107 @@
 Metadata-Version: 2.1
-Name: py-boost
-Version: 0.4.3
+Name: Py-Boost
+Version: 0.5.0
 Summary: Python based GBDT
-Home-page: https://github.com/AILab-MLTools/Py-Boost
+Home-page: https://github.com/sb-ai-lab/Py-Boost
 Author: Vakhrushev Anton
 Author-email: btbpanda@gmail.com
 Requires-Python: >=3.7,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: Russian
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: importlib-metadata (>=1.0,<2.0) ; python_version < "3.8"
 Requires-Dist: joblib
 Requires-Dist: numba
 Requires-Dist: numpy
+Requires-Dist: onnx (>=1.16,<2)
+Requires-Dist: onnxruntime (>=1.16,<2)
 Requires-Dist: pandas (>=1)
 Requires-Dist: scikit-learn (>=1)
 Requires-Dist: tqdm (>=4.64.1)
 Requires-Dist: treelite (>=3,<3.2) ; python_version < "3.8"
 Requires-Dist: treelite (>=3,<4) ; python_version >= "3.8"
 Requires-Dist: treelite_runtime (>=3,<3.2) ; python_version < "3.8"
 Requires-Dist: treelite_runtime (>=3,<4) ; python_version >= "3.8"
-Project-URL: Repository, https://github.com/AILab-MLTools/Py-Boost
+Requires-Dist: ujson
+Project-URL: Repository, https://github.com/sb-ai-lab/Py-Boost
 Description-Content-Type: text/markdown
 
 # Py-boost: a research tool for exploring GBDTs
 
 Modern gradient boosting toolkits are very complex and are written in low-level programming languages. As a result,
 
-* It is hard to customize them to suit one’s needs 
+* It is hard to customize them to suit one’s needs
 * New ideas and methods are not easy to implement
 * It is difficult to understand how they work
 
-Py-boost is a Python-based gradient boosting library which aims at overcoming the aforementioned problems. 
-
-**Authors**: [Anton Vakhrushev](https://kaggle.com/btbpanda), [Leonid Iosipoi](http://iosipoi.com/), [Sergey Kupriyanov](https://www.linkedin.com/in/sergeykupriyanov).
+Py-boost is a Python-based gradient boosting library which aims at overcoming the aforementioned problems.
 
+**Authors**: [Anton Vakhrushev](https://kaggle.com/btbpanda), [Leonid Iosipoi](http://iosipoi.com/)
+, [Sergey Kupriyanov](https://www.linkedin.com/in/sergeykupriyanov).
 
 ## Py-boost Key Features
 
-**Simple**. Py-boost is a simplified gradient boosting library, but it supports all main features and hyperparameters available in other implementations.
-
-**Fast with GPU**. Despite the fact that Py-boost is written in Python, it works only on GPU and uses Python GPU libraries such as `CuPy` and `Numba`.
-
-**Efficient inference**. Since v0.4 Py-Boost is able to perform the efficient inference of tree ensembles on GPU. Moreover, ones your model is trained on GPU, it could be converted to perform the inference on CPU only machine via converting to the [treelite](https://treelite.readthedocs.io/) format with build-in wrapper (limitation - model should be trained with `target_splitter='Single'`, which is the default). 
+**Simple**. Py-boost is a simplified gradient boosting library, but it supports all main features and hyperparameters
+available in other implementations.
 
-**Easy to customize**. Py-boost can be easily customized even if one is not familiar with GPU programming (just replace np with cp).  What can be customized? Almost everything via custom callbacks. Examples: Row/Col sampling strategy, Training control, Losses/metrics, Multioutput handling strategy, Anything via custom callbacks
+**Fast with GPU**. Despite the fact that Py-boost is written in Python, it works only on GPU and uses Python GPU
+libraries such as `CuPy` and `Numba`.
 
+**Efficient inference**. Since v0.4 Py-Boost is able to perform the efficient inference of tree ensembles on GPU.
+Moreover, ones your model is trained on GPU, it could be converted to perform the inference on CPU only machine via
+converting to the [treelite](https://treelite.readthedocs.io/) format with build-in wrapper (limitation - model should
+be trained with `target_splitter='Single'`, which is the default).
+
+**ONNX compatible** Since v0.5 Py-Boost is compatible with ONNX format that allows more options the CPU inference and
+model deployment.
+
+**Easy to customize**. Py-boost can be easily customized even if one is not familiar with GPU programming (just replace
+np with cp). What can be customized? Almost everything via custom callbacks. Examples: Row/Col sampling strategy,
+Training control, Losses/metrics, Multioutput handling strategy, Anything via custom callbacks
 
 ## SketchBoost [paper](https://openreview.net/forum?id=WSxarC8t-T)
 
-**Multioutput training**. Current state-of-atr boosting toolkits provide very limited support of multioutput training. And even if this option is available, training time for such tasks as multiclass/multilabel classification and multitask regression is quite slow because of the training complexity that scales linearly with the number of outputs. To overcome the existing limitations we create **SketchBoost** algorithm that uses approximate tree structure search. As we show in [paper](https://openreview.net/forum?id=WSxarC8t-T) that strategy at least does not lead to performance decrease and often is able to improve the accuracy
-
-**SketchBoost**. You can try our sketching strategies by using `SketchBoost` class or if you want you can implement your own and pass to the `GradientBoosting` constructor as `multioutput_sketch` parameter. For the details please see [Tutorial_2_Advanced_multioutput](https://github.com/AILab-MLTools/Py-Boost/blob/master/tutorials/Tutorial_2_Advanced_multioutput.ipynb)
-
+**Multioutput training**. Current state-of-atr boosting toolkits provide very limited support of multioutput training.
+And even if this option is available, training time for such tasks as multiclass/multilabel classification and multitask
+regression is quite slow because of the training complexity that scales linearly with the number of outputs. To overcome
+the existing limitations we create **SketchBoost** algorithm that uses approximate tree structure search. As we show
+in [paper](https://openreview.net/forum?id=WSxarC8t-T) that strategy at least does not lead to performance decrease and
+often is able to improve the accuracy
+
+**SketchBoost**. You can try our sketching strategies by using `SketchBoost` class or if you want you can implement your
+own and pass to the `GradientBoosting` constructor as `multioutput_sketch` parameter. For the details please
+see [Tutorial_2_Advanced_multioutput](https://github.com/AILab-MLTools/Py-Boost/blob/master/tutorials/Tutorial_2_Advanced_multioutput.ipynb)
 
 ## Installation
 
 Before installing py-boost via pip you should have cupy installed. You can use:
 
 `pip install -U cupy-cuda110 py-boost`
 
 **Note**: replace with your cuda version! For the details see [this guide](https://docs.cupy.dev/en/stable/install.html)
 
-
 ## Quick tour
 
 Py-boost is easy to use since it has similar to scikit-learn interface. For usage example please see:
 
-* [Tutorial_1_Basics](https://github.com/AILab-MLTools/Py-Boost/blob/master/tutorials/Tutorial_1_Basics.ipynb) for simple usage examples
-* [Tutorial_2_Advanced_multioutput](https://github.com/AILab-MLTools/Py-Boost/blob/master/tutorials/Tutorial_2_Advanced_multioutput.ipynb) for advanced multioutput features
-* [Tutorial_3_Custom_features](https://github.com/AILab-MLTools/Py-Boost/blob/master/tutorials/Tutorial_3_Custom_features.ipynb) for examples of customization
+* [Tutorial_1_Basics](https://github.com/sb-ai-lab/Py-Boost/blob/master/tutorials/Tutorial_1_Basics.ipynb) for simple
+  usage examples
+* [Tutorial_2_Advanced_multioutput](https://github.com/sb-ai-lab/Py-Boost/blob/master/tutorials/Tutorial_2_Advanced_multioutput.ipynb)
+  for advanced multioutput features
+* [Tutorial_3_Custom_features](https://github.com/sb-ai-lab/Py-Boost/blob/master/tutorials/Tutorial_3_Custom_features.ipynb)
+  for examples of customization
+* [Tutorial_4_Handle_null_targets](https://github.com/sb-ai-lab/Py-Boost/blob/master/tutorials/Tutorial_4_Handle_null_targets.ipynb)
+  for the case when multioutput target contains NaNs
+* [Tutorial_5_ONNX_inference](https://github.com/sb-ai-lab/Py-Boost/blob/master/tutorials/Tutorial_5_ONNX_inference.ipynb)
+  examples of parsing and inference on CPU with ONNX
 
 More examples are coming soon
```

