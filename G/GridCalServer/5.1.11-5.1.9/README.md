# Comparing `tmp/GridCalServer-5.1.11.tar.gz` & `tmp/GridCalServer-5.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridCalServer-5.1.11.tar", last modified: Mon Jun  3 10:04:37 2024, max compression
+gzip compressed data, was "GridCalServer-5.1.9.tar", last modified: Wed May 29 20:40:00 2024, max compression
```

## Comparing `GridCalServer-5.1.11.tar` & `GridCalServer-5.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-rw-r--   0 santi     (1000) santi     (1000)     2827 2024-05-30 07:29:33.971498 GridCalServer-5.1.11/GridCalServer/__version__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-05-18 10:26:44.119788 GridCalServer-5.1.11/GridCalServer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11713 2024-05-18 10:26:44.119788 GridCalServer-5.1.11/GridCalServer/LICENSE.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)     1199 2024-05-27 07:57:31.426246 GridCalServer-5.1.11/GridCalServer/run.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1535 2024-05-18 10:26:44.119788 GridCalServer-5.1.11/GridCalServer/connection_example.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4728 2024-05-27 07:57:31.426246 GridCalServer-5.1.11/GridCalServer/endpoints.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-05-21 18:33:23.335788 GridCalServer-5.1.11/GridCalServer/data/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    67646 2024-05-21 18:33:23.335788 GridCalServer-5.1.11/GridCalServer/data/GridCal_icon.ico
--rw-rw-r--   0 santi     (1000) santi     (1000)     3876 2024-05-21 18:33:23.335788 GridCalServer-5.1.11/setup.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1044 2024-06-03 10:04:37.439335 GridCalServer-5.1.11/PKG-INFO
--rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-06-03 10:04:37.439335 GridCalServer-5.1.11/setup.cfg
+-rw-rw-rw-   0        0        0     1587 2024-05-29 20:39:28.886291 GridCalServer-5.1.9/GridCalServer/connection_example.py
+-rw-rw-rw-   0        0        0     4893 2024-05-29 20:39:28.887791 GridCalServer-5.1.9/GridCalServer/endpoints.py
+-rw-rw-rw-   0        0        0    11941 2024-05-29 20:39:28.885291 GridCalServer-5.1.9/GridCalServer/LICENSE.txt
+-rw-rw-rw-   0        0        0     1237 2024-05-29 20:39:28.887791 GridCalServer-5.1.9/GridCalServer/run.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 20:39:28.885792 GridCalServer-5.1.9/GridCalServer/__init__.py
+-rw-rw-rw-   0        0        0     2890 2024-05-29 20:39:28.885792 GridCalServer-5.1.9/GridCalServer/__version__.py
+-rw-rw-rw-   0        0        0    67646 2024-05-29 20:39:28.886791 GridCalServer-5.1.9/GridCalServer/data/GridCal_icon.ico
+-rw-rw-rw-   0        0        0        0 2024-05-29 20:39:28.887291 GridCalServer-5.1.9/GridCalServer/data/__init__.py
+-rw-rw-rw-   0        0        0     3991 2024-05-29 20:39:28.888292 GridCalServer-5.1.9/setup.py
+-rw-rw-rw-   0        0        0     1071 2024-05-29 20:40:00.882621 GridCalServer-5.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2024-05-29 20:40:00.882621 GridCalServer-5.1.9/setup.cfg
```

### Comparing `GridCalServer-5.1.11/GridCalServer/__version__.py` & `GridCalServer-5.1.9/GridCalServer/__version__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-# This file is part of GridCal
-#
-# GridCal is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# GridCal is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
-import datetime
-_current_year_ = datetime.datetime.now().year
-
-# do not forget to keep a three-number version!!!
-__GridCalServer_VERSION__ = "5.1.11"
-
-url = 'https://github.com/SanPen/GridCal'
-
-about_msg = "GridCalServer v" + str(__GridCalServer_VERSION__) + '\n\n'
-
-about_msg += """
-GridCal has been carefully crafted since 2015 to 
-serve as a platform for research and consultancy. 
-Visit https://www.advancedgridinsights.com/gridcal for more details.\n"""
-
-about_msg += """
-This program is free software; you can redistribute it and/or
-modify it under the terms of the GNU Lesser General Public
-License as published by the Free Software Foundation; either
-version 3 of the License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-Lesser General Public License for more details.
-
-The source of GridCal can be found at:
-""" + url + "\n\n"
-
-copyright_msg = 'Copyright (C) 2015-' + str(_current_year_) + ' Santiago Peñate Vera'
-
-contributors_msg = 'Michel Lavoie (Transformer automation)\n'
-contributors_msg += 'Bengt Lüers (Better testing)\n'
-contributors_msg += 'Josep Fanals Batllori (HELM, Sequence Short circuit, ACOPF)\n'
-contributors_msg += 'Carlos Alegre (ACOPF)\n'
-contributors_msg += 'Laurens Bliek (MVRSM)\n'
-contributors_msg += 'Jana Soler (Better MVRSM and investments)\n'
-contributors_msg += 'Manuel Navarro Catalán (Better documentation)\n'
-contributors_msg += 'Paul Schultz (Grid Generator)\n'
-contributors_msg += 'Andrés Ramiro (Optimal net transfer capacity)\n'
-contributors_msg += 'Ameer Carlo Lubang (Sequence short-circuit)\n'
-contributors_msg += 'Fernando Postigo Marcos (Better contingencies and SRAP)\n'
-contributors_msg += ('Chavdar Ivanov, '
-                     'Bence Szirbik, '
-                     'Mate Zsebehazi (CGMES)\n')
-contributors_msg += ('Rubén Carmona Pardo, '
-                     'Julio González Mejías, '
-                     'Jesús Riquelme Santos (Contingencies and PTDF testing)\n')
-
-about_msg += copyright_msg + '\n' + contributors_msg
+# This file is part of GridCal
+#
+# GridCal is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# GridCal is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
+import datetime
+_current_year_ = datetime.datetime.now().year
+
+# do not forget to keep a three-number version!!!
+__GridCalServer_VERSION__ = "5.1.9"
+
+url = 'https://github.com/SanPen/GridCal'
+
+about_msg = "GridCalServer v" + str(__GridCalServer_VERSION__) + '\n\n'
+
+about_msg += """
+GridCal has been carefully crafted since 2015 to 
+serve as a platform for research and consultancy. 
+Visit https://www.advancedgridinsights.com/gridcal for more details.\n"""
+
+about_msg += """
+This program is free software; you can redistribute it and/or
+modify it under the terms of the GNU Lesser General Public
+License as published by the Free Software Foundation; either
+version 3 of the License, or (at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+Lesser General Public License for more details.
+
+The source of GridCal can be found at:
+""" + url + "\n\n"
+
+copyright_msg = 'Copyright (C) 2015-' + str(_current_year_) + ' Santiago Peñate Vera'
+
+contributors_msg = 'Michel Lavoie (Transformer automation)\n'
+contributors_msg += 'Bengt Lüers (Better testing)\n'
+contributors_msg += 'Josep Fanals Batllori (HELM, Sequence Short circuit, ACOPF)\n'
+contributors_msg += 'Carlos Alegre (ACOPF)\n'
+contributors_msg += 'Laurens Bliek (MVRSM)\n'
+contributors_msg += 'Jana Soler (Better MVRSM and investments)\n'
+contributors_msg += 'Manuel Navarro Catalán (Better documentation)\n'
+contributors_msg += 'Paul Schultz (Grid Generator)\n'
+contributors_msg += 'Andrés Ramiro (Optimal net transfer capacity)\n'
+contributors_msg += 'Ameer Carlo Lubang (Sequence short-circuit)\n'
+contributors_msg += 'Fernando Postigo Marcos (Better contingencies and SRAP)\n'
+contributors_msg += ('Chavdar Ivanov, '
+                     'Bence Szirbik, '
+                     'Mate Zsebehazi (CGMES)\n')
+contributors_msg += ('Rubén Carmona Pardo, '
+                     'Julio González Mejías, '
+                     'Jesús Riquelme Santos (Contingencies and PTDF testing)\n')
+
+about_msg += copyright_msg + '\n' + contributors_msg
```

### Comparing `GridCalServer-5.1.11/GridCalServer/LICENSE.txt` & `GridCalServer-5.1.9/GridCalServer/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-GridCal LICENSE  (LGPL)
---------------------------------------------------------------------------
-
-GNU LESSER GENERAL PUBLIC LICENSE
-
-Version 3, 29 June 2007
-
-Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
-
-Everyone is permitted to copy and distribute verbatim copies of this
-license document, but changing it is not allowed.
-
-This version of the GNU Lesser General Public License incorporates the terms
-and conditions of version 3 of the GNU General Public License, supplemented
-by the additional permissions listed below.
-0. Additional Definitions.
-
-As used herein, “this License” refers to version 3 of the GNU Lesser General
-Public License, and the “GNU GPL” refers to version 3 of the GNU General
-Public License.
-
-“The Library” refers to a covered work governed by this License, other than
-an Application or a Combined Work as defined below.
-
-An “Application” is any work that makes use of an interface provided by the
-Library, but which is not otherwise based on the Library. Defining a subclass
-of a class defined by the Library is deemed a mode of using an interface
-provided by the Library.
-
-A “Combined Work” is a work produced by combining or linking an Application
-with the Library. The particular version of the Library with which the
-Combined Work was made is also called the “Linked Version”.
-
-The “Minimal Corresponding Source” for a Combined Work means the Corresponding
-Source for the Combined Work, excluding any source code for portions of the
-Combined Work that, considered in isolation, are based on the Application,
-and not on the Linked Version.
-
-The “Corresponding Application Code” for a Combined Work means the object
-code and/or source code for the Application, including any data and utility
-programs needed for reproducing the Combined Work from the Application, but
-excluding the System Libraries of the Combined Work.
-
-1. Exception to Section 3 of the GNU GPL.
-
-You may convey a covered work under sections 3 and 4 of this License without
-being bound by section 3 of the GNU GPL.
-
-2. Conveying Modified Versions.
-
-If you modify a copy of the Library, and, in your modifications, a facility
-refers to a function or data to be supplied by an Application that uses the
-facility (other than as an argument passed when the facility is invoked),
-then you may convey a copy of the modified version:
-
-    a) under this License, provided that you make a good faith effort to ensure
-    that, in the event an Application does not supply the function or data, the f
-    acility still operates, and performs whatever part of its purpose remains
-    meaningful, or
-
-    b) under the GNU GPL, with none of the additional permissions of this License
-    applicable to that copy.
-
-3. Object Code Incorporating Material from Library Header Files.
-
-The object code form of an Application may incorporate material from a header
-file that is part of the Library. You may convey such object code under terms
-of your choice, provided that, if the incorporated material is not limited to
-numerical parameters, data structure layouts and accessors, or small macros,
-inline functions and templates (ten or fewer lines in length), you do both of
-the following:
-
-    a) Give prominent notice with each copy of the object code that the Library
-    is used in it and that the Library and its use are covered by this License.
-
-    b) Accompany the object code with a copy of the GNU GPL and this license
-    document.
-
-4. Combined Works.
-
-You may convey a Combined Work under terms of your choice that, taken together,
-effectively do not restrict modification of the portions of the Library contained
-in the Combined Work and reverse engineering for debugging such modifications,
-if you also do each of the following:
-
-    a) Give prominent notice with each copy of the Combined Work that the Library
-    is used in it and that the Library and its use are covered by this License.
-
-    b) Accompany the Combined Work with a copy of the GNU GPL and this license
-    document.
-
-    c) For a Combined Work that displays copyright notices during execution,
-    include the copyright notice for the Library among these notices, as well
-    as a reference directing the user to the copies of the GNU GPL and this
-    license document.
-
-    d) Do one of the following:
-        0) Convey the Minimal Corresponding Source under the terms of this License,
-        and the Corresponding Application Code in a form suitable for, and under
-        terms that permit, the user to recombine or relink the Application with a
-        modified version of the Linked Version to produce a modified Combined Work,
-        in the manner specified by section 6 of the GNU GPL for conveying
-        Corresponding Source.
-
-        1) Use a suitable shared library mechanism for linking with the Library.
-        A suitable mechanism is one that (a) uses at run time a copy of the Library
-        already present on the user's computer system, and (b) will operate properly
-        with a modified version of the Library that is interface-compatible with
-        the Linked Version.
-
-    e) Provide Installation Information, but only if you would otherwise be required
-    to provide such information under section 6 of the GNU GPL, and only to the
-    extent that such information is necessary to install and execute a modified version
-    of the Combined Work produced by recombining or relinking the Application with a
-    modified version of the Linked Version. (If you use option 4d0, the Installation
-    Information must accompany the Minimal Corresponding Source and Corresponding
-    Application Code. If you use option 4d1, you must provide the Installation
-    Information in the manner specified by section 6 of the GNU GPL for conveying
-    Corresponding Source.)
-
-5. Combined Libraries.
-
-You may place library facilities that are a work based on the Library side by side in a
-single library together with other library facilities that are not Applications and are
-not covered by this License, and convey such a combined library under terms of your
-choice, if you do both of the following:
-
-    a) Accompany the combined library with a copy of the same work based on the Library,
-    uncombined with any other library facilities, conveyed under the terms of this License.
-
-    b) Give prominent notice with the combined library that part of it is a work based on
-    the Library, and explaining where to find the accompanying uncombined form of the same
-    work.
-
-
-6. Revised Versions of the GNU Lesser General Public License.
-
-The Free Software Foundation may publish revised and/or new versions of the GNU Lesser
-General Public License from time to time. Such new versions will be similar in spirit to
-the present version, but may differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Library as you received it
-specifies that a certain numbered version of the GNU Lesser General Public License
-“or any later version” applies to it, you have the option of following the terms and
-conditions either of that published version or of any later version published by the
-Free Software Foundation. If the Library as you received it does not specify a version
-number of the GNU Lesser General Public License, you may choose any version of the GNU
-Lesser General Public License ever published by the Free Software Foundation.
-
-If the Library as you received it specifies that a proxy can decide whether future versions
-of the GNU Lesser General Public License shall apply, that proxy's public statement of
-acceptance of any version is permanent authorization for you to choose that version for
-the Library.
-
------------------------------------------------------------------------------
-Trademarks
------------------------------------------------------------------------------
-
-All trademarks mentioned in the source code or the interface belong to their
-respective owners.
-
-PSSe is a trademark of Siements PTI
-PowerFactory is a trademark of DiGSilent
-PowerWorld is a trademark of Power World Corporation
-Plexos is a Trademark of Energy Exemplar
-
------------------------------------------------------------------------------
-Linking exceptions
------------------------------------------------------------------------------
-
-Both the Bentayga and NewtonNative packages are proprietary libraries that
-are exempt of sharing the source code when linked from GridCal. Both libraries
-area optional and no GridCal functionality is curtailed by not linking Bentayga
-or Newton.
-
-The author of GridCal (Santiago Peñate-Vera) Is also the author of Bentayga
-and NewtonNative, hence the ability to make the exemptions.
-
------------------------------------------------------------------------------
-List of strict dependencies
------------------------------------------------------------------------------
-
-+--------------+------------------------------------------+
-| Package      | License                                  |
-+==============+==========================================+
-| setuptools   | MIT                                      |
-+--------------+------------------------------------------+
-| wheel        | MIT                                      |
-+--------------+------------------------------------------+
-| PySide6      | LGPL                                     |
-+--------------+------------------------------------------+
-| numpy        | BSD                                      |
-+--------------+------------------------------------------+
-| scipy        | BSD                                      |
-+--------------+------------------------------------------+
-| networkx     | BSD                                      |
-+--------------+------------------------------------------+
-| pandas       | Apache                                   |
-+--------------+------------------------------------------+
-| ortools      | Apache                                   |
-+--------------+------------------------------------------+
-| xlwt         | BSD                                      |
-+--------------+------------------------------------------+
-| xlrd         | BSD                                      |
-+--------------+------------------------------------------+
-| matplotlib   | Python Software Foundation License (PSF) |
-+--------------+------------------------------------------+
-| qtconsole    | BSD                                      |
-+--------------+------------------------------------------+
-| openpyxl     | MIT                                      |
-+--------------+------------------------------------------+
-| chardet      | LGPL                                     |
-+--------------+------------------------------------------+
-| scikit-learn | OSI approved (new BSD)                   |
-+--------------+------------------------------------------+
-| geopy        | MIT                                      |
-+--------------+------------------------------------------+
-| pytest       | MIT                                      |
-+--------------+------------------------------------------+
-| h5py         | BSD                                      |
-+--------------+------------------------------------------+
-| numba        | BSD                                      |
-+--------------+------------------------------------------+
-| folium       | MIT                                      |
-+--------------+------------------------------------------+
-| pyproj       | MIT                                      |
-+--------------+------------------------------------------+
-| rdflib       | BSD-3 clause                             |
+GridCal LICENSE  (LGPL)
+--------------------------------------------------------------------------
+
+GNU LESSER GENERAL PUBLIC LICENSE
+
+Version 3, 29 June 2007
+
+Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
+
+Everyone is permitted to copy and distribute verbatim copies of this
+license document, but changing it is not allowed.
+
+This version of the GNU Lesser General Public License incorporates the terms
+and conditions of version 3 of the GNU General Public License, supplemented
+by the additional permissions listed below.
+0. Additional Definitions.
+
+As used herein, “this License” refers to version 3 of the GNU Lesser General
+Public License, and the “GNU GPL” refers to version 3 of the GNU General
+Public License.
+
+“The Library” refers to a covered work governed by this License, other than
+an Application or a Combined Work as defined below.
+
+An “Application” is any work that makes use of an interface provided by the
+Library, but which is not otherwise based on the Library. Defining a subclass
+of a class defined by the Library is deemed a mode of using an interface
+provided by the Library.
+
+A “Combined Work” is a work produced by combining or linking an Application
+with the Library. The particular version of the Library with which the
+Combined Work was made is also called the “Linked Version”.
+
+The “Minimal Corresponding Source” for a Combined Work means the Corresponding
+Source for the Combined Work, excluding any source code for portions of the
+Combined Work that, considered in isolation, are based on the Application,
+and not on the Linked Version.
+
+The “Corresponding Application Code” for a Combined Work means the object
+code and/or source code for the Application, including any data and utility
+programs needed for reproducing the Combined Work from the Application, but
+excluding the System Libraries of the Combined Work.
+
+1. Exception to Section 3 of the GNU GPL.
+
+You may convey a covered work under sections 3 and 4 of this License without
+being bound by section 3 of the GNU GPL.
+
+2. Conveying Modified Versions.
+
+If you modify a copy of the Library, and, in your modifications, a facility
+refers to a function or data to be supplied by an Application that uses the
+facility (other than as an argument passed when the facility is invoked),
+then you may convey a copy of the modified version:
+
+    a) under this License, provided that you make a good faith effort to ensure
+    that, in the event an Application does not supply the function or data, the f
+    acility still operates, and performs whatever part of its purpose remains
+    meaningful, or
+
+    b) under the GNU GPL, with none of the additional permissions of this License
+    applicable to that copy.
+
+3. Object Code Incorporating Material from Library Header Files.
+
+The object code form of an Application may incorporate material from a header
+file that is part of the Library. You may convey such object code under terms
+of your choice, provided that, if the incorporated material is not limited to
+numerical parameters, data structure layouts and accessors, or small macros,
+inline functions and templates (ten or fewer lines in length), you do both of
+the following:
+
+    a) Give prominent notice with each copy of the object code that the Library
+    is used in it and that the Library and its use are covered by this License.
+
+    b) Accompany the object code with a copy of the GNU GPL and this license
+    document.
+
+4. Combined Works.
+
+You may convey a Combined Work under terms of your choice that, taken together,
+effectively do not restrict modification of the portions of the Library contained
+in the Combined Work and reverse engineering for debugging such modifications,
+if you also do each of the following:
+
+    a) Give prominent notice with each copy of the Combined Work that the Library
+    is used in it and that the Library and its use are covered by this License.
+
+    b) Accompany the Combined Work with a copy of the GNU GPL and this license
+    document.
+
+    c) For a Combined Work that displays copyright notices during execution,
+    include the copyright notice for the Library among these notices, as well
+    as a reference directing the user to the copies of the GNU GPL and this
+    license document.
+
+    d) Do one of the following:
+        0) Convey the Minimal Corresponding Source under the terms of this License,
+        and the Corresponding Application Code in a form suitable for, and under
+        terms that permit, the user to recombine or relink the Application with a
+        modified version of the Linked Version to produce a modified Combined Work,
+        in the manner specified by section 6 of the GNU GPL for conveying
+        Corresponding Source.
+
+        1) Use a suitable shared library mechanism for linking with the Library.
+        A suitable mechanism is one that (a) uses at run time a copy of the Library
+        already present on the user's computer system, and (b) will operate properly
+        with a modified version of the Library that is interface-compatible with
+        the Linked Version.
+
+    e) Provide Installation Information, but only if you would otherwise be required
+    to provide such information under section 6 of the GNU GPL, and only to the
+    extent that such information is necessary to install and execute a modified version
+    of the Combined Work produced by recombining or relinking the Application with a
+    modified version of the Linked Version. (If you use option 4d0, the Installation
+    Information must accompany the Minimal Corresponding Source and Corresponding
+    Application Code. If you use option 4d1, you must provide the Installation
+    Information in the manner specified by section 6 of the GNU GPL for conveying
+    Corresponding Source.)
+
+5. Combined Libraries.
+
+You may place library facilities that are a work based on the Library side by side in a
+single library together with other library facilities that are not Applications and are
+not covered by this License, and convey such a combined library under terms of your
+choice, if you do both of the following:
+
+    a) Accompany the combined library with a copy of the same work based on the Library,
+    uncombined with any other library facilities, conveyed under the terms of this License.
+
+    b) Give prominent notice with the combined library that part of it is a work based on
+    the Library, and explaining where to find the accompanying uncombined form of the same
+    work.
+
+
+6. Revised Versions of the GNU Lesser General Public License.
+
+The Free Software Foundation may publish revised and/or new versions of the GNU Lesser
+General Public License from time to time. Such new versions will be similar in spirit to
+the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Library as you received it
+specifies that a certain numbered version of the GNU Lesser General Public License
+“or any later version” applies to it, you have the option of following the terms and
+conditions either of that published version or of any later version published by the
+Free Software Foundation. If the Library as you received it does not specify a version
+number of the GNU Lesser General Public License, you may choose any version of the GNU
+Lesser General Public License ever published by the Free Software Foundation.
+
+If the Library as you received it specifies that a proxy can decide whether future versions
+of the GNU Lesser General Public License shall apply, that proxy's public statement of
+acceptance of any version is permanent authorization for you to choose that version for
+the Library.
+
+-----------------------------------------------------------------------------
+Trademarks
+-----------------------------------------------------------------------------
+
+All trademarks mentioned in the source code or the interface belong to their
+respective owners.
+
+PSSe is a trademark of Siements PTI
+PowerFactory is a trademark of DiGSilent
+PowerWorld is a trademark of Power World Corporation
+Plexos is a Trademark of Energy Exemplar
+
+-----------------------------------------------------------------------------
+Linking exceptions
+-----------------------------------------------------------------------------
+
+Both the Bentayga and NewtonNative packages are proprietary libraries that
+are exempt of sharing the source code when linked from GridCal. Both libraries
+area optional and no GridCal functionality is curtailed by not linking Bentayga
+or Newton.
+
+The author of GridCal (Santiago Peñate-Vera) Is also the author of Bentayga
+and NewtonNative, hence the ability to make the exemptions.
+
+-----------------------------------------------------------------------------
+List of strict dependencies
+-----------------------------------------------------------------------------
+
++--------------+------------------------------------------+
+| Package      | License                                  |
++==============+==========================================+
+| setuptools   | MIT                                      |
++--------------+------------------------------------------+
+| wheel        | MIT                                      |
++--------------+------------------------------------------+
+| PySide6      | LGPL                                     |
++--------------+------------------------------------------+
+| numpy        | BSD                                      |
++--------------+------------------------------------------+
+| scipy        | BSD                                      |
++--------------+------------------------------------------+
+| networkx     | BSD                                      |
++--------------+------------------------------------------+
+| pandas       | Apache                                   |
++--------------+------------------------------------------+
+| ortools      | Apache                                   |
++--------------+------------------------------------------+
+| xlwt         | BSD                                      |
++--------------+------------------------------------------+
+| xlrd         | BSD                                      |
++--------------+------------------------------------------+
+| matplotlib   | Python Software Foundation License (PSF) |
++--------------+------------------------------------------+
+| qtconsole    | BSD                                      |
++--------------+------------------------------------------+
+| openpyxl     | MIT                                      |
++--------------+------------------------------------------+
+| chardet      | LGPL                                     |
++--------------+------------------------------------------+
+| scikit-learn | OSI approved (new BSD)                   |
++--------------+------------------------------------------+
+| geopy        | MIT                                      |
++--------------+------------------------------------------+
+| pytest       | MIT                                      |
++--------------+------------------------------------------+
+| h5py         | BSD                                      |
++--------------+------------------------------------------+
+| numba        | BSD                                      |
++--------------+------------------------------------------+
+| folium       | MIT                                      |
++--------------+------------------------------------------+
+| pyproj       | MIT                                      |
++--------------+------------------------------------------+
+| rdflib       | BSD-3 clause                             |
 +--------------+------------------------------------------+
```

### Comparing `GridCalServer-5.1.11/GridCalServer/run.py` & `GridCalServer-5.1.9/GridCalServer/run.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# This file is part of GridCal.
-#
-# GridCal is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# GridCal is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
-import os
-import sys
-import uvicorn
-
-PACKAGE_PARENT = '..'
-SCRIPT_DIR = os.path.dirname(os.path.realpath(os.path.join(os.getcwd(), os.path.expanduser(__file__))))
-sys.path.append(os.path.normpath(os.path.join(SCRIPT_DIR, PACKAGE_PARENT)))
-from GridCalServer.__version__ import about_msg
-from GridCalServer.endpoints import app
-
-
-
-def start_server():
-    """
-
-    :return:
-    """
-
-    uvicorn.run(app, host="0.0.0.0", port=8000, ssl_keyfile="key.pem", ssl_certfile="cert.pem")
-
-
-if __name__ == "__main__":
-    print(about_msg)
-    start_server()
+# This file is part of GridCal.
+#
+# GridCal is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# GridCal is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
+import os
+import sys
+import uvicorn
+
+PACKAGE_PARENT = '..'
+SCRIPT_DIR = os.path.dirname(os.path.realpath(os.path.join(os.getcwd(), os.path.expanduser(__file__))))
+sys.path.append(os.path.normpath(os.path.join(SCRIPT_DIR, PACKAGE_PARENT)))
+from GridCalServer.__version__ import about_msg
+from GridCalServer.endpoints import app
+
+
+
+def start_server():
+    """
+
+    :return:
+    """
+
+    uvicorn.run(app, host="0.0.0.0", port=8000, ssl_keyfile="key.pem", ssl_certfile="cert.pem")
+
+
+if __name__ == "__main__":
+    print(about_msg)
+    start_server()
```

### Comparing `GridCalServer-5.1.11/GridCalServer/connection_example.py` & `GridCalServer-5.1.9/GridCalServer/connection_example.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import os
-import asyncio
-import websockets
-from typing import Callable
-
-
-async def send_large_file(file_path: str,
-                          websocket: websockets.WebSocketClientProtocol,
-                          progress_func: Callable[[float], None] = None) -> None:
-    """
-    Send a large file via web-socket
-    :param file_path: local file path
-    :param websocket: web socket instance
-    :param progress_func: Progress function
-    :return: None
-    """
-    # Get the size of the file
-    file_size = os.path.getsize(file_path)
-    bytes_sent = 0
-
-    # Open the file in binary mode
-    with open(file_path, "rb") as file:
-        # Read the file in chunks
-        while True:
-            # Read 4KB of data
-            data = file.read(4096)
-            if not data:
-                break  # End of file
-
-            # Send the chunk over the WebSocket
-            await websocket.send(data)
-
-            # Update bytes sent
-            bytes_sent += len(data)
-
-            # Calculate progress
-            progress = (bytes_sent / file_size) * 100
-
-            if progress_func is not None:
-                progress_func(progress)
-
-
-async def connect_and_send(file_path: str, url: str = 'ws://localhost:8000/ws'):
-    """
-    Connect and send data to web-socket
-    """
-    async with websockets.connect(url) as websocket:
-        await send_large_file(file_path, websocket)
-
-
-if __name__ == '__main__':
-    asyncio.get_event_loop().run_until_complete(connect_and_send(file_path="my_file.dat", url="ws://localhost:8000"))
+import os
+import asyncio
+import websockets
+from typing import Callable
+
+
+async def send_large_file(file_path: str,
+                          websocket: websockets.WebSocketClientProtocol,
+                          progress_func: Callable[[float], None] = None) -> None:
+    """
+    Send a large file via web-socket
+    :param file_path: local file path
+    :param websocket: web socket instance
+    :param progress_func: Progress function
+    :return: None
+    """
+    # Get the size of the file
+    file_size = os.path.getsize(file_path)
+    bytes_sent = 0
+
+    # Open the file in binary mode
+    with open(file_path, "rb") as file:
+        # Read the file in chunks
+        while True:
+            # Read 4KB of data
+            data = file.read(4096)
+            if not data:
+                break  # End of file
+
+            # Send the chunk over the WebSocket
+            await websocket.send(data)
+
+            # Update bytes sent
+            bytes_sent += len(data)
+
+            # Calculate progress
+            progress = (bytes_sent / file_size) * 100
+
+            if progress_func is not None:
+                progress_func(progress)
+
+
+async def connect_and_send(file_path: str, url: str = 'ws://localhost:8000/ws'):
+    """
+    Connect and send data to web-socket
+    """
+    async with websockets.connect(url) as websocket:
+        await send_large_file(file_path, websocket)
+
+
+if __name__ == '__main__':
+    asyncio.get_event_loop().run_until_complete(connect_and_send(file_path="my_file.dat", url="ws://localhost:8000"))
```

### Comparing `GridCalServer-5.1.11/GridCalServer/endpoints.py` & `GridCalServer-5.1.9/GridCalServer/endpoints.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-# GridCal
-# Copyright (C) 2015 - 2024 Santiago Peñate Vera
-#
-# This program is free software; you can redistribute it and/or
-# modify it under the terms of the GNU Lesser General Public
-# License as published by the Free Software Foundation; either
-# version 3 of the License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# Lesser General Public License for more details.
-#
-# You should have received a copy of the GNU Lesser General Public License
-# along with this program; if not, write to the Free Software Foundation,
-# Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-import os
-import json
-from typing import Dict
-from hashlib import sha256
-from fastapi import FastAPI, Header, HTTPException, BackgroundTasks
-from fastapi.responses import FileResponse
-from starlette.responses import StreamingResponse
-from GridCalEngine.IO.gridcal.remote import RemoteInstruction, RemoteJob
-from GridCalEngine.IO.gridcal.pack_unpack import parse_gridcal_data
-
-app = FastAPI()
-
-# Store WebSocket connections in a set
-__connections__ = set()
-
-# GC_FOLDER = get_create_gridcal_folder()
-# GC_SERVER_FILE = os.path.join(GC_FOLDER, "server_config.json")
-SECRET_KEY = ""
-
-JOBS_LIST: Dict[str, RemoteJob] = dict()
-
-
-def verify_api_key(api_key: str = Header(None)):
-    """
-    Define a function to verify the API key
-    :param api_key:
-    """
-    if api_key is None:
-        raise HTTPException(status_code=401, detail="API Key is missing")
-
-    # Hash the provided API key using the same algorithm and compare with the stored hash
-    hashed_api_key = sha256(api_key.encode()).hexdigest()
-    if hashed_api_key != SECRET_KEY:
-        raise HTTPException(status_code=403, detail="Invalid API Key")
-
-
-@app.get("/")
-async def read_root():
-    """
-    Root
-    :return: string
-    """
-    return {"message": "GridCal server running", "status": "ok"}
-
-
-@app.get('/favicon.ico', include_in_schema=False)
-async def favicon():
-    """
-
-    :return:
-    """
-    return FileResponse(os.path.join(os.path.dirname(__file__), "data", "GridCal_icon.ico"))
-
-
-async def stream_load_json(json_data):
-    """
-
-    :param json_data:
-    :return:
-    """
-
-    async def generate():
-        """
-
-        """
-        yield json.dumps(json_data).encode()
-
-    return StreamingResponse(generate())
-
-
-async def process_json_data(json_data: Dict[str, Dict[str, Dict[str, str]]]):
-    """
-    Action called on the upload
-    :param json_data: the grid info generated with 'gather_model_as_jsons_for_communication'
-    """
-    circuit = parse_gridcal_data(data=json_data)
-    print(f'Circuit loaded alright nbus{circuit.get_bus_number()}, nbr{circuit.get_branch_number()}')
-
-    if 'instruction' in json_data:
-        instruction = RemoteInstruction(data=json_data['instruction'])
-
-        job = RemoteJob(grid=circuit, instruction=instruction)
-
-        # register the job
-        JOBS_LIST[job.id_tag] = job
-
-        print("Job data\n", job.get_data())
-
-    else:
-        print('No Instruction found\n\n', json_data)
-
-
-@app.post("/upload/")
-async def upload_json_background(json_data: dict, background_tasks: BackgroundTasks):
-    """
-
-    :param json_data:
-    :param background_tasks:
-    :return:
-    """
-    background_tasks.add_task(stream_load_json, json_data)
-    background_tasks.add_task(process_json_data, json_data)
-
-    return {"message": "JSON data streaming initiated"}
-
-
-@app.get("/jobs_list")
-async def jobs_list():
-    """
-    Root
-    :return: string
-    """
-    return [job.get_data() for id_tag, job in JOBS_LIST.items()]
-
-
-@app.delete("/jobs/{job_id}")
-async def delete_job(job_id: str):
-    """
-    Delete a specific job by ID
-    :param job_id: The ID of the job to delete
-    :return: A message indicating the result
-    """
-    if job_id in JOBS_LIST:
-        del JOBS_LIST[job_id]
-        return {"message": f"Job {job_id} deleted successfully"}
-    else:
-        raise HTTPException(status_code=404, detail="Job not found")
-
-
-@app.post("/jobs/{job_id}/cancel")
-async def cancel_job(job_id: str):
-    """
-    Cancel a specific job by ID
-    :param job_id: The ID of the job to cancel
-    :return: A message indicating the result
-    """
-    job = JOBS_LIST.get(job_id)
-    if not job:
-        raise HTTPException(status_code=404, detail="Job not found")
-
-    job.cancel()
-    return {"message": f"Job {job_id} canceled successfully"}
-
-
-if __name__ == "__main__":
-    import uvicorn
-
-    # uvicorn.run(app, host="0.0.0.0", port=8000, ssl_keyfile="key.pem", ssl_certfile="cert.pem")
-    uvicorn.run(app, host="0.0.0.0", port=8000)
+# GridCal
+# Copyright (C) 2015 - 2024 Santiago Peñate Vera
+#
+# This program is free software; you can redistribute it and/or
+# modify it under the terms of the GNU Lesser General Public
+# License as published by the Free Software Foundation; either
+# version 3 of the License, or (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public License
+# along with this program; if not, write to the Free Software Foundation,
+# Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+import os
+import json
+from typing import Dict
+from hashlib import sha256
+from fastapi import FastAPI, Header, HTTPException, BackgroundTasks
+from fastapi.responses import FileResponse
+from starlette.responses import StreamingResponse
+from GridCalEngine.IO.gridcal.remote import RemoteInstruction, RemoteJob
+from GridCalEngine.IO.gridcal.pack_unpack import parse_gridcal_data
+
+app = FastAPI()
+
+# Store WebSocket connections in a set
+__connections__ = set()
+
+# GC_FOLDER = get_create_gridcal_folder()
+# GC_SERVER_FILE = os.path.join(GC_FOLDER, "server_config.json")
+SECRET_KEY = ""
+
+JOBS_LIST: Dict[str, RemoteJob] = dict()
+
+
+def verify_api_key(api_key: str = Header(None)):
+    """
+    Define a function to verify the API key
+    :param api_key:
+    """
+    if api_key is None:
+        raise HTTPException(status_code=401, detail="API Key is missing")
+
+    # Hash the provided API key using the same algorithm and compare with the stored hash
+    hashed_api_key = sha256(api_key.encode()).hexdigest()
+    if hashed_api_key != SECRET_KEY:
+        raise HTTPException(status_code=403, detail="Invalid API Key")
+
+
+@app.get("/")
+async def read_root():
+    """
+    Root
+    :return: string
+    """
+    return {"message": "GridCal server running", "status": "ok"}
+
+
+@app.get('/favicon.ico', include_in_schema=False)
+async def favicon():
+    """
+
+    :return:
+    """
+    return FileResponse(os.path.join(os.path.dirname(__file__), "data", "GridCal_icon.ico"))
+
+
+async def stream_load_json(json_data):
+    """
+
+    :param json_data:
+    :return:
+    """
+
+    async def generate():
+        """
+
+        """
+        yield json.dumps(json_data).encode()
+
+    return StreamingResponse(generate())
+
+
+async def process_json_data(json_data: Dict[str, Dict[str, Dict[str, str]]]):
+    """
+    Action called on the upload
+    :param json_data: the grid info generated with 'gather_model_as_jsons_for_communication'
+    """
+    circuit = parse_gridcal_data(data=json_data)
+    print(f'Circuit loaded alright nbus{circuit.get_bus_number()}, nbr{circuit.get_branch_number()}')
+
+    if 'instruction' in json_data:
+        instruction = RemoteInstruction(data=json_data['instruction'])
+
+        job = RemoteJob(grid=circuit, instruction=instruction)
+
+        # register the job
+        JOBS_LIST[job.id_tag] = job
+
+        print("Job data\n", job.get_data())
+
+    else:
+        print('No Instruction found\n\n', json_data)
+
+
+@app.post("/upload/")
+async def upload_json_background(json_data: dict, background_tasks: BackgroundTasks):
+    """
+
+    :param json_data:
+    :param background_tasks:
+    :return:
+    """
+    background_tasks.add_task(stream_load_json, json_data)
+    background_tasks.add_task(process_json_data, json_data)
+
+    return {"message": "JSON data streaming initiated"}
+
+
+@app.get("/jobs_list")
+async def jobs_list():
+    """
+    Root
+    :return: string
+    """
+    return [job.get_data() for id_tag, job in JOBS_LIST.items()]
+
+
+@app.delete("/jobs/{job_id}")
+async def delete_job(job_id: str):
+    """
+    Delete a specific job by ID
+    :param job_id: The ID of the job to delete
+    :return: A message indicating the result
+    """
+    if job_id in JOBS_LIST:
+        del JOBS_LIST[job_id]
+        return {"message": f"Job {job_id} deleted successfully"}
+    else:
+        raise HTTPException(status_code=404, detail="Job not found")
+
+
+@app.post("/jobs/{job_id}/cancel")
+async def cancel_job(job_id: str):
+    """
+    Cancel a specific job by ID
+    :param job_id: The ID of the job to cancel
+    :return: A message indicating the result
+    """
+    job = JOBS_LIST.get(job_id)
+    if not job:
+        raise HTTPException(status_code=404, detail="Job not found")
+
+    job.cancel()
+    return {"message": f"Job {job_id} canceled successfully"}
+
+
+if __name__ == "__main__":
+    import uvicorn
+
+    # uvicorn.run(app, host="0.0.0.0", port=8000, ssl_keyfile="key.pem", ssl_certfile="cert.pem")
+    uvicorn.run(app, host="0.0.0.0", port=8000)
```

### Comparing `GridCalServer-5.1.11/GridCalServer/data/GridCal_icon.ico` & `GridCalServer-5.1.9/GridCalServer/data/GridCal_icon.ico`

 * *Files identical despite different names*

### Comparing `GridCalServer-5.1.11/setup.py` & `GridCalServer-5.1.9/setup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-# This file is part of GridCal.g
-#
-# GridCal is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# GridCal is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
-"""
-A setuptools based setup module.
-See:
-https://packaging.python.org/guides/distributing-packages-using-setuptools/
-https://github.com/pypa/sampleproject
-"""
-
-# Always prefer setuptools over distutils
-from setuptools import setup, find_packages
-import os
-
-from GridCalServer.__version__ import __GridCalServer_VERSION__
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-long_description = '''# GridCal
-
-This software aims to be a complete platform for power systems research and simulation.
-
-[Watch the video https](https://youtu.be/SY66WgLGo54)
-
-[Check out the documentation](https://gridcal.readthedocs.io)
-
-
-## Installation
-
-pip install GridCalServer
-
-For more options (including a standalone setup one), follow the
-[installation instructions]( https://gridcal.readthedocs.io/en/latest/getting_started/install.html)
-from the project's [documentation](https://gridcal.readthedocs.io)
-'''
-
-description = 'GridCal is a Power Systems simulation program intended for professional use and research'
-
-base_path = os.path.join('GridCalServer')
-
-pkgs_to_exclude = ['docs', 'research', 'tests', 'tutorials', 'GridCalEngine']
-
-packages = find_packages(exclude=pkgs_to_exclude)
-
-# ... so we have to do the filtering ourselves
-packages2 = list()
-for package in packages:
-    elms = package.split('.')
-    excluded = False
-    for exclude in pkgs_to_exclude:
-        if exclude in elms:
-            excluded = True
-
-    if not excluded:
-        packages2.append(package)
-
-package_data = {'GridCalServer': ['*.md',
-                                  '*.rst',
-                                  'LICENSE.txt',
-                                  'setup.py',
-                                  'data/GridCal_icon.ico'],
-                }
-
-dependencies = ['setuptools>=41.0.1',
-                'wheel>=0.37.2',
-                "fastapi",
-                "uvicorn",
-                "websockets",
-                "GridCalEngine==" + __GridCalServer_VERSION__,  # the GridCalEngine version must be exactly the same
-                ]
-
-extras_require = {
-    'gch5 files': ["tables"]  # this is for h5 compatibility
-}
-# Arguments marked as "Required" below must be included for upload to PyPI.
-# Fields marked as "Optional" may be commented out.
-
-setup(
-    name='GridCalServer',  # Required
-    version=__GridCalServer_VERSION__,  # Required
-    license='LGPL',
-    description=description,  # Optional
-    long_description=long_description,  # Optional
-    long_description_content_type='text/markdown',  # Optional (see note above)
-    url='https://github.com/SanPen/GridCal',  # Optional
-    author='Santiago Peñate Vera et. Al.',  # Optional
-    author_email='santiago@gridcal.org',  # Optional
-    classifiers=[
-        'License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)',
-        'Programming Language :: Python :: 3.8',
-    ],
-    keywords='power systems planning',  # Optional
-    packages=packages2,  # Required
-    include_package_data=True,
-    python_requires='>=3.8',
-    install_requires=dependencies,
-    extras_require=extras_require,
-    package_data=package_data,
-    entry_points={
-        'console_scripts': [
-            'gridcalserver = GridCalServer.run:start_server',
-        ],
-    },
-)
+# This file is part of GridCal.g
+#
+# GridCal is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# GridCal is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
+"""
+A setuptools based setup module.
+See:
+https://packaging.python.org/guides/distributing-packages-using-setuptools/
+https://github.com/pypa/sampleproject
+"""
+
+# Always prefer setuptools over distutils
+from setuptools import setup, find_packages
+import os
+
+from GridCalServer.__version__ import __GridCalServer_VERSION__
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+long_description = '''# GridCal
+
+This software aims to be a complete platform for power systems research and simulation.
+
+[Watch the video https](https://youtu.be/SY66WgLGo54)
+
+[Check out the documentation](https://gridcal.readthedocs.io)
+
+
+## Installation
+
+pip install GridCalServer
+
+For more options (including a standalone setup one), follow the
+[installation instructions]( https://gridcal.readthedocs.io/en/latest/getting_started/install.html)
+from the project's [documentation](https://gridcal.readthedocs.io)
+'''
+
+description = 'GridCal is a Power Systems simulation program intended for professional use and research'
+
+base_path = os.path.join('GridCalServer')
+
+pkgs_to_exclude = ['docs', 'research', 'tests', 'tutorials', 'GridCalEngine']
+
+packages = find_packages(exclude=pkgs_to_exclude)
+
+# ... so we have to do the filtering ourselves
+packages2 = list()
+for package in packages:
+    elms = package.split('.')
+    excluded = False
+    for exclude in pkgs_to_exclude:
+        if exclude in elms:
+            excluded = True
+
+    if not excluded:
+        packages2.append(package)
+
+package_data = {'GridCalServer': ['*.md',
+                                  '*.rst',
+                                  'LICENSE.txt',
+                                  'setup.py',
+                                  'data/GridCal_icon.ico'],
+                }
+
+dependencies = ['setuptools>=41.0.1',
+                'wheel>=0.37.2',
+                "fastapi",
+                "uvicorn",
+                "websockets",
+                "GridCalEngine==" + __GridCalServer_VERSION__,  # the GridCalEngine version must be exactly the same
+                ]
+
+extras_require = {
+    'gch5 files': ["tables"]  # this is for h5 compatibility
+}
+# Arguments marked as "Required" below must be included for upload to PyPI.
+# Fields marked as "Optional" may be commented out.
+
+setup(
+    name='GridCalServer',  # Required
+    version=__GridCalServer_VERSION__,  # Required
+    license='LGPL',
+    description=description,  # Optional
+    long_description=long_description,  # Optional
+    long_description_content_type='text/markdown',  # Optional (see note above)
+    url='https://github.com/SanPen/GridCal',  # Optional
+    author='Santiago Peñate Vera et. Al.',  # Optional
+    author_email='santiago@gridcal.org',  # Optional
+    classifiers=[
+        'License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)',
+        'Programming Language :: Python :: 3.8',
+    ],
+    keywords='power systems planning',  # Optional
+    packages=packages2,  # Required
+    include_package_data=True,
+    python_requires='>=3.8',
+    install_requires=dependencies,
+    extras_require=extras_require,
+    package_data=package_data,
+    entry_points={
+        'console_scripts': [
+            'gridcalserver = GridCalServer.run:start_server',
+        ],
+    },
+)
```

### Comparing `GridCalServer-5.1.11/PKG-INFO` & `GridCalServer-5.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1
-Name: GridCalServer
-Version: 5.1.11
-Summary: GridCal is a Power Systems simulation program intended for professional use and research
-Home-page: https://github.com/SanPen/GridCal
-Author: Santiago Peñate Vera et. Al.
-Author-email: santiago@gridcal.org
-License: LGPL
-Keywords: power systems planning
-Classifier:  License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
-Classifier:  Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: gch5 files
-
-# GridCal 
-This software aims to be a complete platform for power systems research and simulation.)
-
-[Watch the video https](https://youtu.be/SY66WgLGo54)
-[Check out the documentation](https://gridcal.readthedocs.io)
-
-## Installation
-
-pip install GridCal
-
-For more options (including a standalone setup one), follow the
-[installation instructions]( https://gridcal.readthedocs.io/en/latest/getting_started/install.html)
-from the project's [documentation](https://gridcal.readthedocs.io)
-
+Metadata-Version: 2.1
+Name: GridCalServer
+Version: 5.1.9
+Summary: GridCal is a Power Systems simulation program intended for professional use and research
+Home-page: https://github.com/SanPen/GridCal
+Author: Santiago Peñate Vera et. Al.
+Author-email: santiago@gridcal.org
+License: LGPL
+Keywords: power systems planning
+Classifier:  License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
+Classifier:  Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: gch5 files
+
+# GridCal 
+This software aims to be a complete platform for power systems research and simulation.)
+
+[Watch the video https](https://youtu.be/SY66WgLGo54)
+[Check out the documentation](https://gridcal.readthedocs.io)
+
+## Installation
+
+pip install GridCal
+
+For more options (including a standalone setup one), follow the
+[installation instructions]( https://gridcal.readthedocs.io/en/latest/getting_started/install.html)
+from the project's [documentation](https://gridcal.readthedocs.io)
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+iso-8859-1
```

