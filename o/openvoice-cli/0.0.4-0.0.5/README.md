# Comparing `tmp/openvoice_cli-0.0.4.tar.gz` & `tmp/openvoice_cli-0.0.5.tar.gz`

## Comparing `openvoice_cli-0.0.4.tar` & `openvoice_cli-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,33 @@
--rw-r--r--   0        0        0    15278 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/ORGINAL_LICENSE
--rw-r--r--   0        0        0   345644 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/out.wav
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/requirements.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/torch_install_command.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/__init__.py
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/__main__.py
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/api.py
--rw-r--r--   0        0        0    16835 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/attentions.py
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/commons.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/downloader.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/mel_processing.py
--rw-r--r--   0        0        0    16692 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/models.py
--rw-r--r--   0        0        0    19630 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/modules.py
--rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/se_extractor.py
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/transforms.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/openvoice_cli/utils.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/.gitignore
--rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 openvoice_cli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    15611 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/ORGINAL_LICENSE
+-rw-r--r--   0        0        0  1002030 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/female.wav
+-rw-r--r--   0        0        0   762126 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/male.wav
+-rw-r--r--   0        0        0   500780 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/out.wav
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/torch_install_command.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/__init__.py
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/__main__.py
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/api.py
+-rw-r--r--   0        0        0    16833 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/attentions.py
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/commons.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/downloader.py
+-rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/mel_processing.py
+-rw-r--r--   0        0        0    17337 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/models.py
+-rw-r--r--   0        0        0    19626 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/modules.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/se_extractor.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/transforms.py
+-rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/utils.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/checkpoints/base_speakers/ses/en-au.pth
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/checkpoints/base_speakers/ses/en-br.pth
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/checkpoints/base_speakers/ses/en-default.pth
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/checkpoints/base_speakers/ses/en-india.pth
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/checkpoints/base_speakers/ses/en-newest.pth
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/checkpoints/base_speakers/ses/en-us.pth
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/checkpoints/base_speakers/ses/es.pth
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/checkpoints/base_speakers/ses/fr.pth
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/checkpoints/base_speakers/ses/jp.pth
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/checkpoints/base_speakers/ses/kr.pth
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/openvoice_cli/checkpoints/base_speakers/ses/zh.pth
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/.gitignore
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 openvoice_cli-0.0.5/PKG-INFO
```

### Comparing `openvoice_cli-0.0.4/ORGINAL_LICENSE` & `openvoice_cli-0.0.5/ORGINAL_LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,333 +1,333 @@
-Creative Commons Attribution-NonCommercial 4.0 International Public
-License
-
-By exercising the Licensed Rights (defined below), You accept and agree
-to be bound by the terms and conditions of this Creative Commons
-Attribution-NonCommercial 4.0 International Public License ("Public
-License"). To the extent this Public License may be interpreted as a
-contract, You are granted the Licensed Rights in consideration of Your
-acceptance of these terms and conditions, and the Licensor grants You
-such rights in consideration of benefits the Licensor receives from
-making the Licensed Material available under these terms and
-conditions.
-
-
-Section 1 -- Definitions.
-
-  a. Adapted Material means material subject to Copyright and Similar
-     Rights that is derived from or based upon the Licensed Material
-     and in which the Licensed Material is translated, altered,
-     arranged, transformed, or otherwise modified in a manner requiring
-     permission under the Copyright and Similar Rights held by the
-     Licensor. For purposes of this Public License, where the Licensed
-     Material is a musical work, performance, or sound recording,
-     Adapted Material is always produced where the Licensed Material is
-     synched in timed relation with a moving image.
-
-  b. Adapter's License means the license You apply to Your Copyright
-     and Similar Rights in Your contributions to Adapted Material in
-     accordance with the terms and conditions of this Public License.
-
-  c. Copyright and Similar Rights means copyright and/or similar rights
-     closely related to copyright including, without limitation,
-     performance, broadcast, sound recording, and Sui Generis Database
-     Rights, without regard to how the rights are labeled or
-     categorized. For purposes of this Public License, the rights
-     specified in Section 2(b)(1)-(2) are not Copyright and Similar
-     Rights.
-  d. Effective Technological Measures means those measures that, in the
-     absence of proper authority, may not be circumvented under laws
-     fulfilling obligations under Article 11 of the WIPO Copyright
-     Treaty adopted on December 20, 1996, and/or similar international
-     agreements.
-
-  e. Exceptions and Limitations means fair use, fair dealing, and/or
-     any other exception or limitation to Copyright and Similar Rights
-     that applies to Your use of the Licensed Material.
-
-  f. Licensed Material means the artistic or literary work, database,
-     or other material to which the Licensor applied this Public
-     License.
-
-  g. Licensed Rights means the rights granted to You subject to the
-     terms and conditions of this Public License, which are limited to
-     all Copyright and Similar Rights that apply to Your use of the
-     Licensed Material and that the Licensor has authority to license.
-
-  h. Licensor means the individual(s) or entity(ies) granting rights
-     under this Public License.
-
-  i. NonCommercial means not primarily intended for or directed towards
-     commercial advantage or monetary compensation. For purposes of
-     this Public License, the exchange of the Licensed Material for
-     other material subject to Copyright and Similar Rights by digital
-     file-sharing or similar means is NonCommercial provided there is
-     no payment of monetary compensation in connection with the
-     exchange.
-
-  j. Share means to provide material to the public by any means or
-     process that requires permission under the Licensed Rights, such
-     as reproduction, public display, public performance, distribution,
-     dissemination, communication, or importation, and to make material
-     available to the public including in ways that members of the
-     public may access the material from a place and at a time
-     individually chosen by them.
-
-  k. Sui Generis Database Rights means rights other than copyright
-     resulting from Directive 96/9/EC of the European Parliament and of
-     the Council of 11 March 1996 on the legal protection of databases,
-     as amended and/or succeeded, as well as other essentially
-     equivalent rights anywhere in the world.
-
-  l. You means the individual or entity exercising the Licensed Rights
-     under this Public License. Your has a corresponding meaning.
-
-
-Section 2 -- Scope.
-
-  a. License grant.
-
-       1. Subject to the terms and conditions of this Public License,
-          the Licensor hereby grants You a worldwide, royalty-free,
-          non-sublicensable, non-exclusive, irrevocable license to
-          exercise the Licensed Rights in the Licensed Material to:
-
-            a. reproduce and Share the Licensed Material, in whole or
-               in part, for NonCommercial purposes only; and
-
-            b. produce, reproduce, and Share Adapted Material for
-               NonCommercial purposes only.
-
-       2. Exceptions and Limitations. For the avoidance of doubt, where
-          Exceptions and Limitations apply to Your use, this Public
-          License does not apply, and You do not need to comply with
-          its terms and conditions.
-
-       3. Term. The term of this Public License is specified in Section
-          6(a).
-
-       4. Media and formats; technical modifications allowed. The
-          Licensor authorizes You to exercise the Licensed Rights in
-          all media and formats whether now known or hereafter created,
-          and to make technical modifications necessary to do so. The
-          Licensor waives and/or agrees not to assert any right or
-          authority to forbid You from making technical modifications
-          necessary to exercise the Licensed Rights, including
-          technical modifications necessary to circumvent Effective
-          Technological Measures. For purposes of this Public License,
-          simply making modifications authorized by this Section 2(a)
-          (4) never produces Adapted Material.
-
-       5. Downstream recipients.
-
-            a. Offer from the Licensor -- Licensed Material. Every
-               recipient of the Licensed Material automatically
-               receives an offer from the Licensor to exercise the
-               Licensed Rights under the terms and conditions of this
-               Public License.
-
-            b. No downstream restrictions. You may not offer or impose
-               any additional or different terms or conditions on, or
-               apply any Effective Technological Measures to, the
-               Licensed Material if doing so restricts exercise of the
-               Licensed Rights by any recipient of the Licensed
-               Material.
-
-       6. No endorsement. Nothing in this Public License constitutes or
-          may be construed as permission to assert or imply that You
-          are, or that Your use of the Licensed Material is, connected
-          with, or sponsored, endorsed, or granted official status by,
-          the Licensor or others designated to receive attribution as
-          provided in Section 3(a)(1)(A)(i).
-
-  b. Other rights.
-
-       1. Moral rights, such as the right of integrity, are not
-          licensed under this Public License, nor are publicity,
-          privacy, and/or other similar personality rights; however, to
-          the extent possible, the Licensor waives and/or agrees not to
-          assert any such rights held by the Licensor to the limited
-          extent necessary to allow You to exercise the Licensed
-          Rights, but not otherwise.
-
-       2. Patent and trademark rights are not licensed under this
-          Public License.
-
-       3. To the extent possible, the Licensor waives any right to
-          collect royalties from You for the exercise of the Licensed
-          Rights, whether directly or through a collecting society
-          under any voluntary or waivable statutory or compulsory
-          licensing scheme. In all other cases the Licensor expressly
-          reserves any right to collect such royalties, including when
-          the Licensed Material is used other than for NonCommercial
-          purposes.
-
-
-Section 3 -- License Conditions.
-
-Your exercise of the Licensed Rights is expressly made subject to the
-following conditions.
-
-  a. Attribution.
-
-       1. If You Share the Licensed Material (including in modified
-          form), You must:
-
-            a. retain the following if it is supplied by the Licensor
-               with the Licensed Material:
-
-                 i. identification of the creator(s) of the Licensed
-                    Material and any others designated to receive
-                    attribution, in any reasonable manner requested by
-                    the Licensor (including by pseudonym if
-                    designated);
-
-                ii. a copyright notice;
-
-               iii. a notice that refers to this Public License;
-
-                iv. a notice that refers to the disclaimer of
-                    warranties;
-
-                 v. a URI or hyperlink to the Licensed Material to the
-                    extent reasonably practicable;
-
-            b. indicate if You modified the Licensed Material and
-               retain an indication of any previous modifications; and
-
-            c. indicate the Licensed Material is licensed under this
-               Public License, and include the text of, or the URI or
-               hyperlink to, this Public License.
-
-       2. You may satisfy the conditions in Section 3(a)(1) in any
-          reasonable manner based on the medium, means, and context in
-          which You Share the Licensed Material. For example, it may be
-          reasonable to satisfy the conditions by providing a URI or
-          hyperlink to a resource that includes the required
-          information.
-
-       3. If requested by the Licensor, You must remove any of the
-          information required by Section 3(a)(1)(A) to the extent
-          reasonably practicable.
-
-       4. If You Share Adapted Material You produce, the Adapter's
-          License You apply must not prevent recipients of the Adapted
-          Material from complying with this Public License.
-
-
-Section 4 -- Sui Generis Database Rights.
-
-Where the Licensed Rights include Sui Generis Database Rights that
-apply to Your use of the Licensed Material:
-
-  a. for the avoidance of doubt, Section 2(a)(1) grants You the right
-     to extract, reuse, reproduce, and Share all or a substantial
-     portion of the contents of the database for NonCommercial purposes
-     only;
-
-  b. if You include all or a substantial portion of the database
-     contents in a database in which You have Sui Generis Database
-     Rights, then the database in which You have Sui Generis Database
-     Rights (but not its individual contents) is Adapted Material; and
-
-  c. You must comply with the conditions in Section 3(a) if You Share
-     all or a substantial portion of the contents of the database.
-
-For the avoidance of doubt, this Section 4 supplements and does not
-replace Your obligations under this Public License where the Licensed
-Rights include other Copyright and Similar Rights.
-
-
-Section 5 -- Disclaimer of Warranties and Limitation of Liability.
-
-  a. UNLESS OTHERWISE SEPARATELY UNDERTAKEN BY THE LICENSOR, TO THE
-     EXTENT POSSIBLE, THE LICENSOR OFFERS THE LICENSED MATERIAL AS-IS
-     AND AS-AVAILABLE, AND MAKES NO REPRESENTATIONS OR WARRANTIES OF
-     ANY KIND CONCERNING THE LICENSED MATERIAL, WHETHER EXPRESS,
-     IMPLIED, STATUTORY, OR OTHER. THIS INCLUDES, WITHOUT LIMITATION,
-     WARRANTIES OF TITLE, MERCHANTABILITY, FITNESS FOR A PARTICULAR
-     PURPOSE, NON-INFRINGEMENT, ABSENCE OF LATENT OR OTHER DEFECTS,
-     ACCURACY, OR THE PRESENCE OR ABSENCE OF ERRORS, WHETHER OR NOT
-     KNOWN OR DISCOVERABLE. WHERE DISCLAIMERS OF WARRANTIES ARE NOT
-     ALLOWED IN FULL OR IN PART, THIS DISCLAIMER MAY NOT APPLY TO YOU.
-
-  b. TO THE EXTENT POSSIBLE, IN NO EVENT WILL THE LICENSOR BE LIABLE
-     TO YOU ON ANY LEGAL THEORY (INCLUDING, WITHOUT LIMITATION,
-     NEGLIGENCE) OR OTHERWISE FOR ANY DIRECT, SPECIAL, INDIRECT,
-     INCIDENTAL, CONSEQUENTIAL, PUNITIVE, EXEMPLARY, OR OTHER LOSSES,
-     COSTS, EXPENSES, OR DAMAGES ARISING OUT OF THIS PUBLIC LICENSE OR
-     USE OF THE LICENSED MATERIAL, EVEN IF THE LICENSOR HAS BEEN
-     ADVISED OF THE POSSIBILITY OF SUCH LOSSES, COSTS, EXPENSES, OR
-     DAMAGES. WHERE A LIMITATION OF LIABILITY IS NOT ALLOWED IN FULL OR
-     IN PART, THIS LIMITATION MAY NOT APPLY TO YOU.
-
-  c. The disclaimer of warranties and limitation of liability provided
-     above shall be interpreted in a manner that, to the extent
-     possible, most closely approximates an absolute disclaimer and
-     waiver of all liability.
-
-
-Section 6 -- Term and Termination.
-
-  a. This Public License applies for the term of the Copyright and
-     Similar Rights licensed here. However, if You fail to comply with
-     this Public License, then Your rights under this Public License
-     terminate automatically.
-
-  b. Where Your right to use the Licensed Material has terminated under
-     Section 6(a), it reinstates:
-
-       1. automatically as of the date the violation is cured, provided
-          it is cured within 30 days of Your discovery of the
-          violation; or
-
-       2. upon express reinstatement by the Licensor.
-
-     For the avoidance of doubt, this Section 6(b) does not affect any
-     right the Licensor may have to seek remedies for Your violations
-     of this Public License.
-
-  c. For the avoidance of doubt, the Licensor may also offer the
-     Licensed Material under separate terms or conditions or stop
-     distributing the Licensed Material at any time; however, doing so
-     will not terminate this Public License.
-
-  d. Sections 1, 5, 6, 7, and 8 survive termination of this Public
-     License.
-
-
-Section 7 -- Other Terms and Conditions.
-
-  a. The Licensor shall not be bound by any additional or different
-     terms or conditions communicated by You unless expressly agreed.
-
-  b. Any arrangements, understandings, or agreements regarding the
-     Licensed Material not stated herein are separate from and
-     independent of the terms and conditions of this Public License.
-
-
-Section 8 -- Interpretation.
-
-  a. For the avoidance of doubt, this Public License does not, and
-     shall not be interpreted to, reduce, limit, restrict, or impose
-     conditions on any use of the Licensed Material that could lawfully
-     be made without permission under this Public License.
-
-  b. To the extent possible, if any provision of this Public License is
-     deemed unenforceable, it shall be automatically reformed to the
-     minimum extent necessary to make it enforceable. If the provision
-     cannot be reformed, it shall be severed from this Public License
-     without affecting the enforceability of the remaining terms and
-     conditions.
-
-  c. No term or condition of this Public License will be waived and no
-     failure to comply consented to unless expressly agreed to by the
-     Licensor.
-
-  d. Nothing in this Public License constitutes or may be interpreted
-     as a limitation upon, or waiver of, any privileges and immunities
-     that apply to the Licensor or You, including from the legal
-     processes of any jurisdiction or authority.
-
-=======================================================================
-
+Creative Commons Attribution-NonCommercial 4.0 International Public
+License
+
+By exercising the Licensed Rights (defined below), You accept and agree
+to be bound by the terms and conditions of this Creative Commons
+Attribution-NonCommercial 4.0 International Public License ("Public
+License"). To the extent this Public License may be interpreted as a
+contract, You are granted the Licensed Rights in consideration of Your
+acceptance of these terms and conditions, and the Licensor grants You
+such rights in consideration of benefits the Licensor receives from
+making the Licensed Material available under these terms and
+conditions.
+
+
+Section 1 -- Definitions.
+
+  a. Adapted Material means material subject to Copyright and Similar
+     Rights that is derived from or based upon the Licensed Material
+     and in which the Licensed Material is translated, altered,
+     arranged, transformed, or otherwise modified in a manner requiring
+     permission under the Copyright and Similar Rights held by the
+     Licensor. For purposes of this Public License, where the Licensed
+     Material is a musical work, performance, or sound recording,
+     Adapted Material is always produced where the Licensed Material is
+     synched in timed relation with a moving image.
+
+  b. Adapter's License means the license You apply to Your Copyright
+     and Similar Rights in Your contributions to Adapted Material in
+     accordance with the terms and conditions of this Public License.
+
+  c. Copyright and Similar Rights means copyright and/or similar rights
+     closely related to copyright including, without limitation,
+     performance, broadcast, sound recording, and Sui Generis Database
+     Rights, without regard to how the rights are labeled or
+     categorized. For purposes of this Public License, the rights
+     specified in Section 2(b)(1)-(2) are not Copyright and Similar
+     Rights.
+  d. Effective Technological Measures means those measures that, in the
+     absence of proper authority, may not be circumvented under laws
+     fulfilling obligations under Article 11 of the WIPO Copyright
+     Treaty adopted on December 20, 1996, and/or similar international
+     agreements.
+
+  e. Exceptions and Limitations means fair use, fair dealing, and/or
+     any other exception or limitation to Copyright and Similar Rights
+     that applies to Your use of the Licensed Material.
+
+  f. Licensed Material means the artistic or literary work, database,
+     or other material to which the Licensor applied this Public
+     License.
+
+  g. Licensed Rights means the rights granted to You subject to the
+     terms and conditions of this Public License, which are limited to
+     all Copyright and Similar Rights that apply to Your use of the
+     Licensed Material and that the Licensor has authority to license.
+
+  h. Licensor means the individual(s) or entity(ies) granting rights
+     under this Public License.
+
+  i. NonCommercial means not primarily intended for or directed towards
+     commercial advantage or monetary compensation. For purposes of
+     this Public License, the exchange of the Licensed Material for
+     other material subject to Copyright and Similar Rights by digital
+     file-sharing or similar means is NonCommercial provided there is
+     no payment of monetary compensation in connection with the
+     exchange.
+
+  j. Share means to provide material to the public by any means or
+     process that requires permission under the Licensed Rights, such
+     as reproduction, public display, public performance, distribution,
+     dissemination, communication, or importation, and to make material
+     available to the public including in ways that members of the
+     public may access the material from a place and at a time
+     individually chosen by them.
+
+  k. Sui Generis Database Rights means rights other than copyright
+     resulting from Directive 96/9/EC of the European Parliament and of
+     the Council of 11 March 1996 on the legal protection of databases,
+     as amended and/or succeeded, as well as other essentially
+     equivalent rights anywhere in the world.
+
+  l. You means the individual or entity exercising the Licensed Rights
+     under this Public License. Your has a corresponding meaning.
+
+
+Section 2 -- Scope.
+
+  a. License grant.
+
+       1. Subject to the terms and conditions of this Public License,
+          the Licensor hereby grants You a worldwide, royalty-free,
+          non-sublicensable, non-exclusive, irrevocable license to
+          exercise the Licensed Rights in the Licensed Material to:
+
+            a. reproduce and Share the Licensed Material, in whole or
+               in part, for NonCommercial purposes only; and
+
+            b. produce, reproduce, and Share Adapted Material for
+               NonCommercial purposes only.
+
+       2. Exceptions and Limitations. For the avoidance of doubt, where
+          Exceptions and Limitations apply to Your use, this Public
+          License does not apply, and You do not need to comply with
+          its terms and conditions.
+
+       3. Term. The term of this Public License is specified in Section
+          6(a).
+
+       4. Media and formats; technical modifications allowed. The
+          Licensor authorizes You to exercise the Licensed Rights in
+          all media and formats whether now known or hereafter created,
+          and to make technical modifications necessary to do so. The
+          Licensor waives and/or agrees not to assert any right or
+          authority to forbid You from making technical modifications
+          necessary to exercise the Licensed Rights, including
+          technical modifications necessary to circumvent Effective
+          Technological Measures. For purposes of this Public License,
+          simply making modifications authorized by this Section 2(a)
+          (4) never produces Adapted Material.
+
+       5. Downstream recipients.
+
+            a. Offer from the Licensor -- Licensed Material. Every
+               recipient of the Licensed Material automatically
+               receives an offer from the Licensor to exercise the
+               Licensed Rights under the terms and conditions of this
+               Public License.
+
+            b. No downstream restrictions. You may not offer or impose
+               any additional or different terms or conditions on, or
+               apply any Effective Technological Measures to, the
+               Licensed Material if doing so restricts exercise of the
+               Licensed Rights by any recipient of the Licensed
+               Material.
+
+       6. No endorsement. Nothing in this Public License constitutes or
+          may be construed as permission to assert or imply that You
+          are, or that Your use of the Licensed Material is, connected
+          with, or sponsored, endorsed, or granted official status by,
+          the Licensor or others designated to receive attribution as
+          provided in Section 3(a)(1)(A)(i).
+
+  b. Other rights.
+
+       1. Moral rights, such as the right of integrity, are not
+          licensed under this Public License, nor are publicity,
+          privacy, and/or other similar personality rights; however, to
+          the extent possible, the Licensor waives and/or agrees not to
+          assert any such rights held by the Licensor to the limited
+          extent necessary to allow You to exercise the Licensed
+          Rights, but not otherwise.
+
+       2. Patent and trademark rights are not licensed under this
+          Public License.
+
+       3. To the extent possible, the Licensor waives any right to
+          collect royalties from You for the exercise of the Licensed
+          Rights, whether directly or through a collecting society
+          under any voluntary or waivable statutory or compulsory
+          licensing scheme. In all other cases the Licensor expressly
+          reserves any right to collect such royalties, including when
+          the Licensed Material is used other than for NonCommercial
+          purposes.
+
+
+Section 3 -- License Conditions.
+
+Your exercise of the Licensed Rights is expressly made subject to the
+following conditions.
+
+  a. Attribution.
+
+       1. If You Share the Licensed Material (including in modified
+          form), You must:
+
+            a. retain the following if it is supplied by the Licensor
+               with the Licensed Material:
+
+                 i. identification of the creator(s) of the Licensed
+                    Material and any others designated to receive
+                    attribution, in any reasonable manner requested by
+                    the Licensor (including by pseudonym if
+                    designated);
+
+                ii. a copyright notice;
+
+               iii. a notice that refers to this Public License;
+
+                iv. a notice that refers to the disclaimer of
+                    warranties;
+
+                 v. a URI or hyperlink to the Licensed Material to the
+                    extent reasonably practicable;
+
+            b. indicate if You modified the Licensed Material and
+               retain an indication of any previous modifications; and
+
+            c. indicate the Licensed Material is licensed under this
+               Public License, and include the text of, or the URI or
+               hyperlink to, this Public License.
+
+       2. You may satisfy the conditions in Section 3(a)(1) in any
+          reasonable manner based on the medium, means, and context in
+          which You Share the Licensed Material. For example, it may be
+          reasonable to satisfy the conditions by providing a URI or
+          hyperlink to a resource that includes the required
+          information.
+
+       3. If requested by the Licensor, You must remove any of the
+          information required by Section 3(a)(1)(A) to the extent
+          reasonably practicable.
+
+       4. If You Share Adapted Material You produce, the Adapter's
+          License You apply must not prevent recipients of the Adapted
+          Material from complying with this Public License.
+
+
+Section 4 -- Sui Generis Database Rights.
+
+Where the Licensed Rights include Sui Generis Database Rights that
+apply to Your use of the Licensed Material:
+
+  a. for the avoidance of doubt, Section 2(a)(1) grants You the right
+     to extract, reuse, reproduce, and Share all or a substantial
+     portion of the contents of the database for NonCommercial purposes
+     only;
+
+  b. if You include all or a substantial portion of the database
+     contents in a database in which You have Sui Generis Database
+     Rights, then the database in which You have Sui Generis Database
+     Rights (but not its individual contents) is Adapted Material; and
+
+  c. You must comply with the conditions in Section 3(a) if You Share
+     all or a substantial portion of the contents of the database.
+
+For the avoidance of doubt, this Section 4 supplements and does not
+replace Your obligations under this Public License where the Licensed
+Rights include other Copyright and Similar Rights.
+
+
+Section 5 -- Disclaimer of Warranties and Limitation of Liability.
+
+  a. UNLESS OTHERWISE SEPARATELY UNDERTAKEN BY THE LICENSOR, TO THE
+     EXTENT POSSIBLE, THE LICENSOR OFFERS THE LICENSED MATERIAL AS-IS
+     AND AS-AVAILABLE, AND MAKES NO REPRESENTATIONS OR WARRANTIES OF
+     ANY KIND CONCERNING THE LICENSED MATERIAL, WHETHER EXPRESS,
+     IMPLIED, STATUTORY, OR OTHER. THIS INCLUDES, WITHOUT LIMITATION,
+     WARRANTIES OF TITLE, MERCHANTABILITY, FITNESS FOR A PARTICULAR
+     PURPOSE, NON-INFRINGEMENT, ABSENCE OF LATENT OR OTHER DEFECTS,
+     ACCURACY, OR THE PRESENCE OR ABSENCE OF ERRORS, WHETHER OR NOT
+     KNOWN OR DISCOVERABLE. WHERE DISCLAIMERS OF WARRANTIES ARE NOT
+     ALLOWED IN FULL OR IN PART, THIS DISCLAIMER MAY NOT APPLY TO YOU.
+
+  b. TO THE EXTENT POSSIBLE, IN NO EVENT WILL THE LICENSOR BE LIABLE
+     TO YOU ON ANY LEGAL THEORY (INCLUDING, WITHOUT LIMITATION,
+     NEGLIGENCE) OR OTHERWISE FOR ANY DIRECT, SPECIAL, INDIRECT,
+     INCIDENTAL, CONSEQUENTIAL, PUNITIVE, EXEMPLARY, OR OTHER LOSSES,
+     COSTS, EXPENSES, OR DAMAGES ARISING OUT OF THIS PUBLIC LICENSE OR
+     USE OF THE LICENSED MATERIAL, EVEN IF THE LICENSOR HAS BEEN
+     ADVISED OF THE POSSIBILITY OF SUCH LOSSES, COSTS, EXPENSES, OR
+     DAMAGES. WHERE A LIMITATION OF LIABILITY IS NOT ALLOWED IN FULL OR
+     IN PART, THIS LIMITATION MAY NOT APPLY TO YOU.
+
+  c. The disclaimer of warranties and limitation of liability provided
+     above shall be interpreted in a manner that, to the extent
+     possible, most closely approximates an absolute disclaimer and
+     waiver of all liability.
+
+
+Section 6 -- Term and Termination.
+
+  a. This Public License applies for the term of the Copyright and
+     Similar Rights licensed here. However, if You fail to comply with
+     this Public License, then Your rights under this Public License
+     terminate automatically.
+
+  b. Where Your right to use the Licensed Material has terminated under
+     Section 6(a), it reinstates:
+
+       1. automatically as of the date the violation is cured, provided
+          it is cured within 30 days of Your discovery of the
+          violation; or
+
+       2. upon express reinstatement by the Licensor.
+
+     For the avoidance of doubt, this Section 6(b) does not affect any
+     right the Licensor may have to seek remedies for Your violations
+     of this Public License.
+
+  c. For the avoidance of doubt, the Licensor may also offer the
+     Licensed Material under separate terms or conditions or stop
+     distributing the Licensed Material at any time; however, doing so
+     will not terminate this Public License.
+
+  d. Sections 1, 5, 6, 7, and 8 survive termination of this Public
+     License.
+
+
+Section 7 -- Other Terms and Conditions.
+
+  a. The Licensor shall not be bound by any additional or different
+     terms or conditions communicated by You unless expressly agreed.
+
+  b. Any arrangements, understandings, or agreements regarding the
+     Licensed Material not stated herein are separate from and
+     independent of the terms and conditions of this Public License.
+
+
+Section 8 -- Interpretation.
+
+  a. For the avoidance of doubt, this Public License does not, and
+     shall not be interpreted to, reduce, limit, restrict, or impose
+     conditions on any use of the Licensed Material that could lawfully
+     be made without permission under this Public License.
+
+  b. To the extent possible, if any provision of this Public License is
+     deemed unenforceable, it shall be automatically reformed to the
+     minimum extent necessary to make it enforceable. If the provision
+     cannot be reformed, it shall be severed from this Public License
+     without affecting the enforceability of the remaining terms and
+     conditions.
+
+  c. No term or condition of this Public License will be waived and no
+     failure to comply consented to unless expressly agreed to by the
+     Licensor.
+
+  d. Nothing in this Public License constitutes or may be interpreted
+     as a limitation upon, or waiver of, any privileges and immunities
+     that apply to the Licensor or You, including from the legal
+     processes of any jurisdiction or authority.
+
+=======================================================================
+
```

### Comparing `openvoice_cli-0.0.4/openvoice_cli/__main__.py` & `openvoice_cli-0.0.5/openvoice_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `openvoice_cli-0.0.4/openvoice_cli/api.py` & `openvoice_cli-0.0.5/openvoice_cli/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,137 +1,139 @@
-import torch
-import numpy as np
-import re
-import soundfile
-import openvoice_cli.utils as utils
-import os
-import librosa
-from openvoice_cli.mel_processing import spectrogram_torch
-from openvoice_cli.models import SynthesizerTrn
-
-
-class OpenVoiceBaseClass(object):
-    def __init__(self, 
-                config_path, 
-                device='cuda:0'):
-        if 'cuda' in device:
-            assert torch.cuda.is_available()
-
-        hps = utils.get_hparams_from_file(config_path)
-
-        model = SynthesizerTrn(
-            len(getattr(hps, 'symbols', [])),
-            hps.data.filter_length // 2 + 1,
-            n_speakers=hps.data.n_speakers,
-            **hps.model,
-        ).to(device)
-
-        model.eval()
-        self.model = model
-        self.hps = hps
-        self.device = device
-
-    def load_ckpt(self, ckpt_path):
-        checkpoint_dict = torch.load(ckpt_path, map_location=torch.device(self.device))
-        a, b = self.model.load_state_dict(checkpoint_dict['model'], strict=False)
-        print("Loaded checkpoint '{}'".format(ckpt_path))
-        print('missing/unexpected keys:', a, b)
-
-class ToneColorConverter(OpenVoiceBaseClass):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        if kwargs.get('enable_watermark', True):
-            import wavmark
-            self.watermark_model = wavmark.load_model().to(self.device)
-        else:
-            self.watermark_model = None
-
-    def extract_se(self, ref_wav_list, se_save_path=None):
-        if isinstance(ref_wav_list, str):
-            ref_wav_list = [ref_wav_list]
-        
-        device = self.device
-        hps = self.hps
-        gs = []
-        
-        for fname in ref_wav_list:
-            audio_ref, sr = librosa.load(fname, sr=hps.data.sampling_rate)
-            y = torch.FloatTensor(audio_ref)
-            y = y.to(device)
-            y = y.unsqueeze(0)
-            y = spectrogram_torch(y, hps.data.filter_length,
-                                        hps.data.sampling_rate, hps.data.hop_length, hps.data.win_length,
-                                        center=False).to(device)
-            with torch.no_grad():
-                g = self.model.ref_enc(y.transpose(1, 2)).unsqueeze(-1)
-                gs.append(g.detach())
-        gs = torch.stack(gs).mean(0)
-
-        if se_save_path is not None:
-            os.makedirs(os.path.dirname(se_save_path), exist_ok=True)
-            torch.save(gs.cpu(), se_save_path)
-
-        return gs
-
-    def convert(self, audio_src_path, src_se, tgt_se, output_path=None, tau=0.3, message="default"):
-        hps = self.hps
-        # load audio
-        audio, sample_rate = librosa.load(audio_src_path, sr=hps.data.sampling_rate)
-        audio = torch.tensor(audio).float()
-        
-        with torch.no_grad():
-            y = torch.FloatTensor(audio).to(self.device)
-            y = y.unsqueeze(0)
-            spec = spectrogram_torch(y, hps.data.filter_length,
-                                    hps.data.sampling_rate, hps.data.hop_length, hps.data.win_length,
-                                    center=False).to(self.device)
-            spec_lengths = torch.LongTensor([spec.size(-1)]).to(self.device)
-            audio = self.model.voice_conversion(spec, spec_lengths, sid_src=src_se, sid_tgt=tgt_se, tau=tau)[0][
-                        0, 0].data.cpu().float().numpy()
-            audio = self.add_watermark(audio, message)
-            if output_path is None:
-                return audio
-            else:
-                soundfile.write(output_path, audio, hps.data.sampling_rate)
-    
-    def add_watermark(self, audio, message):
-        if self.watermark_model is None:
-            return audio
-        device = self.device
-        bits = utils.string_to_bits(message).reshape(-1)
-        n_repeat = len(bits) // 32
-
-        K = 16000
-        coeff = 2
-        for n in range(n_repeat):
-            trunck = audio[(coeff * n) * K: (coeff * n + 1) * K]
-            if len(trunck) != K:
-                print('Audio too short, fail to add watermark')
-                break
-            message_npy = bits[n * 32: (n + 1) * 32]
-            
-            with torch.no_grad():
-                signal = torch.FloatTensor(trunck).to(device)[None]
-                message_tensor = torch.FloatTensor(message_npy).to(device)[None]
-                signal_wmd_tensor = self.watermark_model.encode(signal, message_tensor)
-                signal_wmd_npy = signal_wmd_tensor.detach().cpu().squeeze()
-            audio[(coeff * n) * K: (coeff * n + 1) * K] = signal_wmd_npy
-        return audio
-
-    def detect_watermark(self, audio, n_repeat):
-        bits = []
-        K = 16000
-        coeff = 2
-        for n in range(n_repeat):
-            trunck = audio[(coeff * n) * K: (coeff * n + 1) * K]
-            if len(trunck) != K:
-                print('Audio too short, fail to detect watermark')
-                return 'Fail'
-            with torch.no_grad():
-                signal = torch.FloatTensor(trunck).to(self.device).unsqueeze(0)
-                message_decoded_npy = (self.watermark_model.decode(signal) >= 0.5).int().detach().cpu().numpy().squeeze()
-            bits.append(message_decoded_npy)
-        bits = np.stack(bits).reshape(-1, 8)
-        message = utils.bits_to_string(bits)
-        return message
-    
+import torch
+import numpy as np
+import re
+import soundfile
+import openvoice_cli.utils as utils
+import os
+import librosa
+from openvoice_cli.mel_processing import spectrogram_torch
+from openvoice_cli.models import SynthesizerTrn
+
+
+class OpenVoiceBaseClass(object):
+    def __init__(self, 
+                config_path, 
+                device='cuda:0'):
+        if 'cuda' in device:
+            assert torch.cuda.is_available()
+
+        hps = utils.get_hparams_from_file(config_path)
+
+        model = SynthesizerTrn(
+            len(getattr(hps, 'symbols', [])),
+            hps.data.filter_length // 2 + 1,
+            n_speakers=hps.data.n_speakers,
+            **hps.model,
+        ).to(device)
+
+        model.eval()
+        self.model = model
+        self.hps = hps
+        self.device = device
+
+    def load_ckpt(self, ckpt_path):
+        checkpoint_dict = torch.load(ckpt_path, map_location=torch.device(self.device))
+        a, b = self.model.load_state_dict(checkpoint_dict['model'], strict=False)
+        print("Loaded checkpoint '{}'".format(ckpt_path))
+        print('missing/unexpected keys:', a, b)
+
+class ToneColorConverter(OpenVoiceBaseClass):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        if kwargs.get('enable_watermark', True):
+            import wavmark
+            self.watermark_model = wavmark.load_model().to(self.device)
+        else:
+            self.watermark_model = None
+        self.version = getattr(self.hps, '_version_', "v1")
+
+
+
+    def extract_se(self, ref_wav_list, se_save_path=None):
+        if isinstance(ref_wav_list, str):
+            ref_wav_list = [ref_wav_list]
+        
+        device = self.device
+        hps = self.hps
+        gs = []
+        
+        for fname in ref_wav_list:
+            audio_ref, sr = librosa.load(fname, sr=hps.data.sampling_rate)
+            y = torch.FloatTensor(audio_ref)
+            y = y.to(device)
+            y = y.unsqueeze(0)
+            y = spectrogram_torch(y, hps.data.filter_length,
+                                        hps.data.sampling_rate, hps.data.hop_length, hps.data.win_length,
+                                        center=False).to(device)
+            with torch.no_grad():
+                g = self.model.ref_enc(y.transpose(1, 2)).unsqueeze(-1)
+                gs.append(g.detach())
+        gs = torch.stack(gs).mean(0)
+
+        if se_save_path is not None:
+            os.makedirs(os.path.dirname(se_save_path), exist_ok=True)
+            torch.save(gs.cpu(), se_save_path)
+
+        return gs
+
+    def convert(self, audio_src_path, src_se, tgt_se, output_path=None, tau=0.3, message="default"):
+        hps = self.hps
+        # load audio
+        audio, sample_rate = librosa.load(audio_src_path, sr=hps.data.sampling_rate)
+        audio = torch.tensor(audio).float()
+        
+        with torch.no_grad():
+            y = torch.FloatTensor(audio).to(self.device)
+            y = y.unsqueeze(0)
+            spec = spectrogram_torch(y, hps.data.filter_length,
+                                    hps.data.sampling_rate, hps.data.hop_length, hps.data.win_length,
+                                    center=False).to(self.device)
+            spec_lengths = torch.LongTensor([spec.size(-1)]).to(self.device)
+            audio = self.model.voice_conversion(spec, spec_lengths, sid_src=src_se, sid_tgt=tgt_se, tau=tau)[0][
+                        0, 0].data.cpu().float().numpy()
+            audio = self.add_watermark(audio, message)
+            if output_path is None:
+                return audio
+            else:
+                soundfile.write(output_path, audio, hps.data.sampling_rate)
+    
+    def add_watermark(self, audio, message):
+        if self.watermark_model is None:
+            return audio
+        device = self.device
+        bits = utils.string_to_bits(message).reshape(-1)
+        n_repeat = len(bits) // 32
+
+        K = 16000
+        coeff = 2
+        for n in range(n_repeat):
+            trunck = audio[(coeff * n) * K: (coeff * n + 1) * K]
+            if len(trunck) != K:
+                print('Audio too short, fail to add watermark')
+                break
+            message_npy = bits[n * 32: (n + 1) * 32]
+            
+            with torch.no_grad():
+                signal = torch.FloatTensor(trunck).to(device)[None]
+                message_tensor = torch.FloatTensor(message_npy).to(device)[None]
+                signal_wmd_tensor = self.watermark_model.encode(signal, message_tensor)
+                signal_wmd_npy = signal_wmd_tensor.detach().cpu().squeeze()
+            audio[(coeff * n) * K: (coeff * n + 1) * K] = signal_wmd_npy
+        return audio
+
+    def detect_watermark(self, audio, n_repeat):
+        bits = []
+        K = 16000
+        coeff = 2
+        for n in range(n_repeat):
+            trunck = audio[(coeff * n) * K: (coeff * n + 1) * K]
+            if len(trunck) != K:
+                print('Audio too short, fail to detect watermark')
+                return 'Fail'
+            with torch.no_grad():
+                signal = torch.FloatTensor(trunck).to(self.device).unsqueeze(0)
+                message_decoded_npy = (self.watermark_model.decode(signal) >= 0.5).int().detach().cpu().numpy().squeeze()
+            bits.append(message_decoded_npy)
+        bits = np.stack(bits).reshape(-1, 8)
+        message = utils.bits_to_string(bits)
+        return message
```

### Comparing `openvoice_cli-0.0.4/openvoice_cli/attentions.py` & `openvoice_cli-0.0.5/openvoice_cli/attentions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -458,8 +458,8 @@
     def _same_padding(self, x):
         if self.kernel_size == 1:
             return x
         pad_l = (self.kernel_size - 1) // 2
         pad_r = self.kernel_size // 2
         padding = [[0, 0], [0, 0], [pad_l, pad_r]]
         x = F.pad(x, commons.convert_pad_shape(padding))
-        return x
+        return x
```

### Comparing `openvoice_cli-0.0.4/openvoice_cli/commons.py` & `openvoice_cli-0.0.5/openvoice_cli/commons.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -153,8 +153,8 @@
     total_norm = 0
     for p in parameters:
         param_norm = p.grad.data.norm(norm_type)
         total_norm += param_norm.item() ** norm_type
         if clip_value is not None:
             p.grad.data.clamp_(min=-clip_value, max=clip_value)
     total_norm = total_norm ** (1.0 / norm_type)
-    return total_norm
+    return total_norm
```

### Comparing `openvoice_cli-0.0.4/openvoice_cli/downloader.py` & `openvoice_cli-0.0.5/openvoice_cli/downloader.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 def download_checkpoint(dest_dir):
     # Define paths
     model_path = Path(dest_dir)
 
     # Define files and their corresponding URLs
     files_to_download = {
-         "checkpoint.pth": f"https://huggingface.co/myshell-ai/OpenVoice/resolve/main/checkpoints/converter/checkpoint.pth?download=true",
-         "config.json": f"https://huggingface.co/myshell-ai/OpenVoice/raw/main/checkpoints/converter/config.json",
+         "checkpoint.pth": f"https://huggingface.co/daswer123/openvoice-tunner-v2/resolve/main/checkpoint.pth?download=true",
+         "config.json": f"https://huggingface.co/daswer123/openvoice-tunner-v2/raw/main/config.json",
     }
 
     # Check and create directories
     create_directory_if_not_exists(model_path)
 
     # Download files if they don't exist
     for filename, url in files_to_download.items():
```

### Comparing `openvoice_cli-0.0.4/openvoice_cli/mel_processing.py` & `openvoice_cli-0.0.5/openvoice_cli/mel_processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,182 +1,184 @@
-import torch
-import torch.utils.data
-from librosa.filters import mel as librosa_mel_fn
-
-MAX_WAV_VALUE = 32768.0
-
-def dynamic_range_compression_torch(x, C=1, clip_val=1e-5):
-    """
-    PARAMS
-    ------
-    C: compression factor
-    """
-    return torch.log(torch.clamp(x, min=clip_val) * C)
-
-
-def dynamic_range_decompression_torch(x, C=1):
-    """
-    PARAMS
-    ------
-    C: compression factor used to compress
-    """
-    return torch.exp(x) / C
-
-
-def spectral_normalize_torch(magnitudes):
-    output = dynamic_range_compression_torch(magnitudes)
-    return output
-
-
-def spectral_de_normalize_torch(magnitudes):
-    output = dynamic_range_decompression_torch(magnitudes)
-    return output
-
-
-mel_basis = {}
-hann_window = {}
-
-
-def spectrogram_torch(y, n_fft, sampling_rate, hop_size, win_size, center=False):
-    if torch.min(y) < -1.1:
-        print("min value is ", torch.min(y))
-    if torch.max(y) > 1.1:
-        print("max value is ", torch.max(y))
-
-    global hann_window
-    dtype_device = str(y.dtype) + "_" + str(y.device)
-    wnsize_dtype_device = str(win_size) + "_" + dtype_device
-    if wnsize_dtype_device not in hann_window:
-        hann_window[wnsize_dtype_device] = torch.hann_window(win_size).to(
-            dtype=y.dtype, device=y.device
-        )
-
-    y = torch.nn.functional.pad(
-        y.unsqueeze(1),
-        (int((n_fft - hop_size) / 2), int((n_fft - hop_size) / 2)),
-        mode="reflect",
-    )
-    y = y.squeeze(1)
-
-    spec = torch.stft(
-        y,
-        n_fft,
-        hop_length=hop_size,
-        win_length=win_size,
-        window=hann_window[wnsize_dtype_device],
-        center=center,
-        pad_mode="reflect",
-        normalized=False,
-        onesided=True,
-        return_complex=False,
-    )
-
-    spec = torch.sqrt(spec.pow(2).sum(-1) + 1e-6)
-    return spec
-
-
-def spectrogram_torch_conv(y, n_fft, sampling_rate, hop_size, win_size, center=False):
-    # if torch.min(y) < -1.:
-    #     print('min value is ', torch.min(y))
-    # if torch.max(y) > 1.:
-    #     print('max value is ', torch.max(y))
-
-    global hann_window
-    dtype_device = str(y.dtype) + '_' + str(y.device)
-    wnsize_dtype_device = str(win_size) + '_' + dtype_device
-    if wnsize_dtype_device not in hann_window:
-        hann_window[wnsize_dtype_device] = torch.hann_window(win_size).to(dtype=y.dtype, device=y.device)
-
-    y = torch.nn.functional.pad(y.unsqueeze(1), (int((n_fft-hop_size)/2), int((n_fft-hop_size)/2)), mode='reflect')
-    
-    # ******************** original ************************#
-    # y = y.squeeze(1)
-    # spec1 = torch.stft(y, n_fft, hop_length=hop_size, win_length=win_size, window=hann_window[wnsize_dtype_device],
-    #                   center=center, pad_mode='reflect', normalized=False, onesided=True, return_complex=False)
-
-    # ******************** ConvSTFT ************************#
-    freq_cutoff = n_fft // 2 + 1
-    fourier_basis = torch.view_as_real(torch.fft.fft(torch.eye(n_fft)))
-    forward_basis = fourier_basis[:freq_cutoff].permute(2, 0, 1).reshape(-1, 1, fourier_basis.shape[1])
-    forward_basis = forward_basis * torch.as_tensor(librosa.util.pad_center(torch.hann_window(win_size), size=n_fft)).float()
-
-    import torch.nn.functional as F
-
-    # if center:
-    #     signal = F.pad(y[:, None, None, :], (n_fft // 2, n_fft // 2, 0, 0), mode = 'reflect').squeeze(1)
-    assert center is False
-
-    forward_transform_squared = F.conv1d(y, forward_basis.to(y.device), stride = hop_size)
-    spec2 = torch.stack([forward_transform_squared[:, :freq_cutoff, :], forward_transform_squared[:, freq_cutoff:, :]], dim = -1)
-
-
-    # ******************** Verification ************************#
-    spec1 = torch.stft(y.squeeze(1), n_fft, hop_length=hop_size, win_length=win_size, window=hann_window[wnsize_dtype_device],
-                      center=center, pad_mode='reflect', normalized=False, onesided=True, return_complex=False)
-    assert torch.allclose(spec1, spec2, atol=1e-4)
-
-    spec = torch.sqrt(spec2.pow(2).sum(-1) + 1e-6)
-    return spec
-
-
-def spec_to_mel_torch(spec, n_fft, num_mels, sampling_rate, fmin, fmax):
-    global mel_basis
-    dtype_device = str(spec.dtype) + "_" + str(spec.device)
-    fmax_dtype_device = str(fmax) + "_" + dtype_device
-    if fmax_dtype_device not in mel_basis:
-        mel = librosa_mel_fn(sampling_rate, n_fft, num_mels, fmin, fmax)
-        mel_basis[fmax_dtype_device] = torch.from_numpy(mel).to(
-            dtype=spec.dtype, device=spec.device
-        )
-    spec = torch.matmul(mel_basis[fmax_dtype_device], spec)
-    spec = spectral_normalize_torch(spec)
-    return spec
-
-
-def mel_spectrogram_torch(
-    y, n_fft, num_mels, sampling_rate, hop_size, win_size, fmin, fmax, center=False
-):
-    if torch.min(y) < -1.0:
-        print("min value is ", torch.min(y))
-    if torch.max(y) > 1.0:
-        print("max value is ", torch.max(y))
-
-    global mel_basis, hann_window
-    dtype_device = str(y.dtype) + "_" + str(y.device)
-    fmax_dtype_device = str(fmax) + "_" + dtype_device
-    wnsize_dtype_device = str(win_size) + "_" + dtype_device
-    if fmax_dtype_device not in mel_basis:
-        mel = librosa_mel_fn(sampling_rate, n_fft, num_mels, fmin, fmax)
-        mel_basis[fmax_dtype_device] = torch.from_numpy(mel).to(
-            dtype=y.dtype, device=y.device
-        )
-    if wnsize_dtype_device not in hann_window:
-        hann_window[wnsize_dtype_device] = torch.hann_window(win_size).to(
-            dtype=y.dtype, device=y.device
-        )
-
-    y = torch.nn.functional.pad(
-        y.unsqueeze(1),
-        (int((n_fft - hop_size) / 2), int((n_fft - hop_size) / 2)),
-        mode="reflect",
-    )
-    y = y.squeeze(1)
-
-    spec = torch.stft(
-        y,
-        n_fft,
-        hop_length=hop_size,
-        win_length=win_size,
-        window=hann_window[wnsize_dtype_device],
-        center=center,
-        pad_mode="reflect",
-        normalized=False,
-        onesided=True,
-        return_complex=False,
-    )
-
-    spec = torch.sqrt(spec.pow(2).sum(-1) + 1e-6)
-
-    spec = torch.matmul(mel_basis[fmax_dtype_device], spec)
-    spec = spectral_normalize_torch(spec)
-
+import librosa
+import torch
+import torch.utils.data
+from librosa.filters import mel as librosa_mel_fn
+
+MAX_WAV_VALUE = 32768.0
+
+
+def dynamic_range_compression_torch(x, C=1, clip_val=1e-5):
+    """
+    PARAMS
+    ------
+    C: compression factor
+    """
+    return torch.log(torch.clamp(x, min=clip_val) * C)
+
+
+def dynamic_range_decompression_torch(x, C=1):
+    """
+    PARAMS
+    ------
+    C: compression factor used to compress
+    """
+    return torch.exp(x) / C
+
+
+def spectral_normalize_torch(magnitudes):
+    output = dynamic_range_compression_torch(magnitudes)
+    return output
+
+
+def spectral_de_normalize_torch(magnitudes):
+    output = dynamic_range_decompression_torch(magnitudes)
+    return output
+
+
+mel_basis = {}
+hann_window = {}
+
+
+def spectrogram_torch(y, n_fft, sampling_rate, hop_size, win_size, center=False):
+    if torch.min(y) < -1.1:
+        print("min value is ", torch.min(y))
+    if torch.max(y) > 1.1:
+        print("max value is ", torch.max(y))
+
+    global hann_window
+    dtype_device = str(y.dtype) + "_" + str(y.device)
+    wnsize_dtype_device = str(win_size) + "_" + dtype_device
+    if wnsize_dtype_device not in hann_window:
+        hann_window[wnsize_dtype_device] = torch.hann_window(win_size).to(
+            dtype=y.dtype, device=y.device
+        )
+
+    y = torch.nn.functional.pad(
+        y.unsqueeze(1),
+        (int((n_fft - hop_size) / 2), int((n_fft - hop_size) / 2)),
+        mode="reflect",
+    )
+    y = y.squeeze(1)
+
+    spec = torch.stft(
+        y,
+        n_fft,
+        hop_length=hop_size,
+        win_length=win_size,
+        window=hann_window[wnsize_dtype_device],
+        center=center,
+        pad_mode="reflect",
+        normalized=False,
+        onesided=True,
+        return_complex=False,
+    )
+
+    spec = torch.sqrt(spec.pow(2).sum(-1) + 1e-6)
+    return spec
+
+
+def spectrogram_torch_conv(y, n_fft, sampling_rate, hop_size, win_size, center=False):
+    # if torch.min(y) < -1.:
+    #     print('min value is ', torch.min(y))
+    # if torch.max(y) > 1.:
+    #     print('max value is ', torch.max(y))
+
+    global hann_window
+    dtype_device = str(y.dtype) + '_' + str(y.device)
+    wnsize_dtype_device = str(win_size) + '_' + dtype_device
+    if wnsize_dtype_device not in hann_window:
+        hann_window[wnsize_dtype_device] = torch.hann_window(win_size).to(dtype=y.dtype, device=y.device)
+
+    y = torch.nn.functional.pad(y.unsqueeze(1), (int((n_fft-hop_size)/2), int((n_fft-hop_size)/2)), mode='reflect')
+    
+    # ******************** original ************************#
+    # y = y.squeeze(1)
+    # spec1 = torch.stft(y, n_fft, hop_length=hop_size, win_length=win_size, window=hann_window[wnsize_dtype_device],
+    #                   center=center, pad_mode='reflect', normalized=False, onesided=True, return_complex=False)
+
+    # ******************** ConvSTFT ************************#
+    freq_cutoff = n_fft // 2 + 1
+    fourier_basis = torch.view_as_real(torch.fft.fft(torch.eye(n_fft)))
+    forward_basis = fourier_basis[:freq_cutoff].permute(2, 0, 1).reshape(-1, 1, fourier_basis.shape[1])
+    forward_basis = forward_basis * torch.as_tensor(librosa.util.pad_center(torch.hann_window(win_size), size=n_fft)).float()
+
+    import torch.nn.functional as F
+
+    # if center:
+    #     signal = F.pad(y[:, None, None, :], (n_fft // 2, n_fft // 2, 0, 0), mode = 'reflect').squeeze(1)
+    assert center is False
+
+    forward_transform_squared = F.conv1d(y, forward_basis.to(y.device), stride = hop_size)
+    spec2 = torch.stack([forward_transform_squared[:, :freq_cutoff, :], forward_transform_squared[:, freq_cutoff:, :]], dim = -1)
+
+
+    # ******************** Verification ************************#
+    spec1 = torch.stft(y.squeeze(1), n_fft, hop_length=hop_size, win_length=win_size, window=hann_window[wnsize_dtype_device],
+                      center=center, pad_mode='reflect', normalized=False, onesided=True, return_complex=False)
+    assert torch.allclose(spec1, spec2, atol=1e-4)
+
+    spec = torch.sqrt(spec2.pow(2).sum(-1) + 1e-6)
+    return spec
+
+
+def spec_to_mel_torch(spec, n_fft, num_mels, sampling_rate, fmin, fmax):
+    global mel_basis
+    dtype_device = str(spec.dtype) + "_" + str(spec.device)
+    fmax_dtype_device = str(fmax) + "_" + dtype_device
+    if fmax_dtype_device not in mel_basis:
+        mel = librosa_mel_fn(sampling_rate, n_fft, num_mels, fmin, fmax)
+        mel_basis[fmax_dtype_device] = torch.from_numpy(mel).to(
+            dtype=spec.dtype, device=spec.device
+        )
+    spec = torch.matmul(mel_basis[fmax_dtype_device], spec)
+    spec = spectral_normalize_torch(spec)
+    return spec
+
+
+def mel_spectrogram_torch(
+    y, n_fft, num_mels, sampling_rate, hop_size, win_size, fmin, fmax, center=False
+):
+    if torch.min(y) < -1.0:
+        print("min value is ", torch.min(y))
+    if torch.max(y) > 1.0:
+        print("max value is ", torch.max(y))
+
+    global mel_basis, hann_window
+    dtype_device = str(y.dtype) + "_" + str(y.device)
+    fmax_dtype_device = str(fmax) + "_" + dtype_device
+    wnsize_dtype_device = str(win_size) + "_" + dtype_device
+    if fmax_dtype_device not in mel_basis:
+        mel = librosa_mel_fn(sampling_rate, n_fft, num_mels, fmin, fmax)
+        mel_basis[fmax_dtype_device] = torch.from_numpy(mel).to(
+            dtype=y.dtype, device=y.device
+        )
+    if wnsize_dtype_device not in hann_window:
+        hann_window[wnsize_dtype_device] = torch.hann_window(win_size).to(
+            dtype=y.dtype, device=y.device
+        )
+
+    y = torch.nn.functional.pad(
+        y.unsqueeze(1),
+        (int((n_fft - hop_size) / 2), int((n_fft - hop_size) / 2)),
+        mode="reflect",
+    )
+    y = y.squeeze(1)
+
+    spec = torch.stft(
+        y,
+        n_fft,
+        hop_length=hop_size,
+        win_length=win_size,
+        window=hann_window[wnsize_dtype_device],
+        center=center,
+        pad_mode="reflect",
+        normalized=False,
+        onesided=True,
+        return_complex=False,
+    )
+
+    spec = torch.sqrt(spec.pow(2).sum(-1) + 1e-6)
+
+    spec = torch.matmul(mel_basis[fmax_dtype_device], spec)
+    spec = spectral_normalize_torch(spec)
+
     return spec
```

### Comparing `openvoice_cli-0.0.4/openvoice_cli/modules.py` & `openvoice_cli-0.0.5/openvoice_cli/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import openvoice_cli.commons as commons
 from openvoice_cli.commons import init_weights, get_padding
 from openvoice_cli.transforms import piecewise_rational_quadratic_transform
 from openvoice_cli.attentions import Encoder
 
 LRELU_SLOPE = 0.1
 
-
 class LayerNorm(nn.Module):
     def __init__(self, channels, eps=1e-5):
         super().__init__()
         self.channels = channels
         self.eps = eps
 
         self.gamma = nn.Parameter(torch.ones(channels))
@@ -591,8 +590,8 @@
         )
 
         x = torch.cat([x0, x1], 1) * x_mask
         logdet = torch.sum(logabsdet * x_mask, [1, 2])
         if not reverse:
             return x, logdet
         else:
-            return x
+            return x
```

### Comparing `openvoice_cli-0.0.4/openvoice_cli/se_extractor.py` & `openvoice_cli-0.0.5/openvoice_cli/se_extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import librosa
 from whisper_timestamped.transcribe import get_audio_tensor, get_vad_segments
 
 model_size = "medium"
 # Run on GPU with FP16
 model = None
 def split_audio_whisper(audio_path, audio_name, target_dir='processed'):
-    print("whisper")
     global model
     if model is None:
         model = WhisperModel(model_size, device="cuda", compute_type="float16")
     audio = AudioSegment.from_file(audio_path)
     max_len = len(audio)
 
     target_folder = os.path.join(target_dir, audio_name)
@@ -125,27 +124,29 @@
     hash_value = hash_object.digest()
     # Convert the hash value to base64
     base64_value = base64.b64encode(hash_value)
     return base64_value.decode('utf-8')[:16].replace('/', '_^')
 
 def get_se(audio_path, vc_model, target_dir='processed', vad=True):
     device = vc_model.device
+    version = vc_model.version
+    print("OpenVoice version:", version)
 
-    audio_name = f"{os.path.basename(audio_path).rsplit('.', 1)[0]}_{hash_numpy_array(audio_path)}"
+    audio_name = f"{os.path.basename(audio_path).rsplit('.', 1)[0]}_{version}_{hash_numpy_array(audio_path)}"
     se_path = os.path.join(target_dir, audio_name, 'se.pth')
 
-    if os.path.isfile(se_path):
-        se = torch.load(se_path).to(device)
-        return se, audio_name
-    if os.path.isdir(audio_path):
-        wavs_folder = audio_path
-    elif vad:
+    # if os.path.isfile(se_path):
+    #     se = torch.load(se_path).to(device)
+    #     return se, audio_name
+    # if os.path.isdir(audio_path):
+    #     wavs_folder = audio_path
+    
+    if vad:
         wavs_folder = split_audio_vad(audio_path, target_dir=target_dir, audio_name=audio_name)
     else:
         wavs_folder = split_audio_whisper(audio_path, target_dir=target_dir, audio_name=audio_name)
     
     audio_segs = glob(f'{wavs_folder}/*.wav')
     if len(audio_segs) == 0:
         raise NotImplementedError('No audio segments found!')
     
-    return vc_model.extract_se(audio_segs, se_save_path=se_path), audio_name
-
+    return vc_model.extract_se(audio_segs, se_save_path=se_path), audio_name
```

### Comparing `openvoice_cli-0.0.4/openvoice_cli/transforms.py` & `openvoice_cli-0.0.5/openvoice_cli/transforms.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -202,8 +202,8 @@
         derivative_numerator = input_delta.pow(2) * (
             input_derivatives_plus_one * theta.pow(2)
             + 2 * input_delta * theta_one_minus_theta
             + input_derivatives * (1 - theta).pow(2)
         )
         logabsdet = torch.log(derivative_numerator) - 2 * torch.log(denominator)
 
-        return outputs, logabsdet
+        return outputs, logabsdet
```

### Comparing `openvoice_cli-0.0.4/README.md` & `openvoice_cli-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,36 +27,34 @@
 
 Simple installation :
 
 ```bash
 pip install openvoice-cli
 ```
 
-**Attention is used Pytorch version 1.13.1 higher unfortunately can not, waiting for an update from the authors of openvoice**
-
 This will install all the necessary dependencies, including a **CPU support only** version of PyTorch
 
 I recommend that you install the **GPU version** to improve processing speed ( up to 3 times faster )
 
 Read the end of the README to learn how to install.
 
 ### Windows
 ```bash
 python -m venv venv
 venv\Scripts\activate
 pip install openvoice-cli
-pip install torch==1.13.1+cu117 torchaudio==0.13.1+cu117 --index-url https://download.pytorch.org/whl/cu117
+pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
 ```
 
 ### Linux
 ```bash
 python -m venv venv
 source venv\bin\activate
 pip install openvoice-cli
-pip install torch==1.13.1+cu117 torchaudio==0.13.1+cu117 --index-url https://download.pytorch.org/whl/cu117
+pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
 ```
 
 ## Usage
 
 This tool supports both single file and batch processing for audio tone color conversion using a reference audio file. Below are the commands for each mode of operation:
 
 ### Single File Processing
```

### Comparing `openvoice_cli-0.0.4/pyproject.toml` & `openvoice_cli-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openvoice-cli"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="daswer123", email="daswerq123@gmail.com" },
 ]
 description = "Use OpenVoice 2 stage via console or python scripts"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `openvoice_cli-0.0.4/PKG-INFO` & `openvoice_cli-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openvoice-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: Use OpenVoice 2 stage via console or python scripts
 Project-URL: Homepage, https://github.com/daswer123/OpenVoice-cli
 Project-URL: Bug Tracker, https://github.com/daswer123/OpenVoice-cli/issues
 Author-email: daswer123 <daswerq123@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -49,36 +49,34 @@
 
 Simple installation :
 
 ```bash
 pip install openvoice-cli
 ```
 
-**Attention is used Pytorch version 1.13.1 higher unfortunately can not, waiting for an update from the authors of openvoice**
-
 This will install all the necessary dependencies, including a **CPU support only** version of PyTorch
 
 I recommend that you install the **GPU version** to improve processing speed ( up to 3 times faster )
 
 Read the end of the README to learn how to install.
 
 ### Windows
 ```bash
 python -m venv venv
 venv\Scripts\activate
 pip install openvoice-cli
-pip install torch==1.13.1+cu117 torchaudio==0.13.1+cu117 --index-url https://download.pytorch.org/whl/cu117
+pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
 ```
 
 ### Linux
 ```bash
 python -m venv venv
 source venv\bin\activate
 pip install openvoice-cli
-pip install torch==1.13.1+cu117 torchaudio==0.13.1+cu117 --index-url https://download.pytorch.org/whl/cu117
+pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
 ```
 
 ## Usage
 
 This tool supports both single file and batch processing for audio tone color conversion using a reference audio file. Below are the commands for each mode of operation:
 
 ### Single File Processing
```

