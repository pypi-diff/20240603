# Comparing `tmp/bosdyn_choreography_client-4.0.1-py3-none-any.whl.zip` & `tmp/bosdyn_choreography_client-4.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 22199 bytes, number of entries: 10
--rw-r--r--  2.0 unx      330 b- defN 24-Apr-12 01:43 bosdyn/__init__.py
--rw-r--r--  2.0 unx      330 b- defN 24-Apr-12 01:43 bosdyn/choreography/__init__.py
--rw-r--r--  2.0 unx      330 b- defN 24-Apr-12 01:43 bosdyn/choreography/client/__init__.py
--rw-r--r--  2.0 unx    18438 b- defN 24-Apr-12 01:43 bosdyn/choreography/client/animation_file_conversion_helpers.py
--rw-r--r--  2.0 unx    25971 b- defN 24-Apr-12 01:43 bosdyn/choreography/client/animation_file_to_proto.py
--rw-r--r--  2.0 unx    48849 b- defN 24-Apr-12 01:43 bosdyn/choreography/client/choreography.py
--rw-r--r--  2.0 unx     1721 b- defN 24-Apr-12 01:44 bosdyn_choreography_client-4.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 01:44 bosdyn_choreography_client-4.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-12 01:44 bosdyn_choreography_client-4.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      960 b- defN 24-Apr-12 01:44 bosdyn_choreography_client-4.0.1.dist-info/RECORD
-10 files, 97028 bytes uncompressed, 20519 bytes compressed:  78.9%
+Zip file size: 22443 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      330 b- defN 24-May-28 15:21 bosdyn/__init__.py
+-rw-r--r--  2.0 unx      330 b- defN 24-May-28 15:21 bosdyn/choreography/__init__.py
+-rw-r--r--  2.0 unx      330 b- defN 24-May-28 15:21 bosdyn/choreography/client/__init__.py
+-rw-r--r--  2.0 unx    18438 b- defN 24-May-28 15:21 bosdyn/choreography/client/animation_file_conversion_helpers.py
+-rw-r--r--  2.0 unx    25971 b- defN 24-May-28 15:21 bosdyn/choreography/client/animation_file_to_proto.py
+-rw-r--r--  2.0 unx    50633 b- defN 24-May-28 15:21 bosdyn/choreography/client/choreography.py
+-rw-r--r--  2.0 unx     1721 b- defN 24-May-28 15:22 bosdyn_choreography_client-4.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 15:22 bosdyn_choreography_client-4.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-28 15:22 bosdyn_choreography_client-4.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      960 b- defN 24-May-28 15:22 bosdyn_choreography_client-4.0.2.dist-info/RECORD
+10 files, 98812 bytes uncompressed, 20763 bytes compressed:  79.0%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: bosdyn/choreography/client/animation_file_to_proto.py
 Comment: 
 
 Filename: bosdyn/choreography/client/choreography.py
 Comment: 
 
-Filename: bosdyn_choreography_client-4.0.1.dist-info/METADATA
+Filename: bosdyn_choreography_client-4.0.2.dist-info/METADATA
 Comment: 
 
-Filename: bosdyn_choreography_client-4.0.1.dist-info/WHEEL
+Filename: bosdyn_choreography_client-4.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: bosdyn_choreography_client-4.0.1.dist-info/top_level.txt
+Filename: bosdyn_choreography_client-4.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bosdyn_choreography_client-4.0.1.dist-info/RECORD
+Filename: bosdyn_choreography_client-4.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bosdyn/choreography/client/choreography.py

```diff
@@ -529,48 +529,89 @@
             self._stub.StopRecordingState,
             request,
             value_from_response=None,  # Return the complete response message
             error_from_response=common_header_errors,
             copy_request=False,
             **kwargs)
 
-    def get_choreography_sequence(self, seq_name, **kwargs):
+    def get_choreography_sequence(self, seq_name, return_animation_names_only=False, **kwargs):
         """Get a sequence currently known by the robot, response includes
             the full ChoreographySequence with the given name and any
             Animations used in the sequence.
 
             Args:
                 seq_name (string): the name of the sequence to return.
+                return_animation_names_only (bool): If True, skip returning a list of the complete 
+                    Animation protos required by the sequence and leave the 'animated_moves' field of
+                    the response empty. (The repeated string field, 'animation_names' for the list 
+                    of the names of required animations will still be returned). 
 
         Returns:
             The full GetChoreographySequenceResponse proto.
         """
 
         req = choreography_sequence_pb2.GetChoreographySequenceRequest()
         req.sequence_name = seq_name
+        req.return_animation_names_only = return_animation_names_only
         return self.call(
             self._stub.GetChoreographySequence,
             req,
             value_from_response=None,  # Return the complete response message
             error_from_response=common_header_errors,
             copy_request=False,
             **kwargs)
 
-    def get_choreography_sequence_async(self, seq_name, **kwargs):
+    def get_choreography_sequence_async(self, seq_name, return_animation_names_only=False,
+                                        **kwargs):
         """Async version of get_choreography_sequence()."""
         req = choreography_sequence_pb2.GetChoreographySequenceRequest()
         req.sequence_name = seq_name
+        req.return_animation_names_only = return_animation_names_only
         return self.call_async(
             self._stub.GetChoreographySequence,
             req,
             value_from_response=None,  # Return the complete response message
             error_from_response=common_header_errors,
             copy_request=False,
             **kwargs)
 
+    def get_animation(self, name, **kwargs):
+        """Get an animation currently known by the robot, response includes
+            the full Animation proto with the given name.
+
+            Args:
+                name (string): the name of the animation to return.
+
+        Returns:
+            The full GetAnimation proto.
+        """
+
+        req = choreography_sequence_pb2.GetAnimationRequest()
+        req.name = name
+        return self.call(
+            self._stub.GetAnimation,
+            req,
+            value_from_response=None,  # Return the complete response message
+            error_from_response=common_header_errors,
+            copy_request=False,
+            **kwargs)
+
+    def get_animation_async(self, name, **kwargs):
+        """Async version of get_animation()."""
+
+        req = choreography_sequence_pb2.GetAnimationRequest()
+        req.name = name
+        return self.call_async(
+            self._stub.GetAnimation,
+            req,
+            value_from_response=None,  # Return the complete response message
+            error_from_response=common_header_errors,
+            copy_request=False,
+            **kwargs)
+
     def save_sequence(self, seq_name, labels=[], **kwargs):
         """Save an uploaded sequence to the robot. Saved sequences are
         automatically uploaded to the robot when it boots.
 
         Returns:
             The full SaveSequenceResponse proto."""
         request = self.build_save_sequence_request(seq_name, labels)
```

## Comparing `bosdyn_choreography_client-4.0.1.dist-info/METADATA` & `bosdyn_choreography_client-4.0.2.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: bosdyn-choreography-client
-Version: 4.0.1
+Version: 4.0.2
 Summary: Boston Dynamics API client code and interfaces for choreography
 Home-page: https://dev.bostondynamics.com/
 Author: Boston Dynamics
 Author-email: support@bostondynamics.com
 Project-URL: Documentation, https://dev.bostondynamics.com/
 Project-URL: Source, https://github.com/boston-dynamics/spot-sdk/
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: bosdyn-api (==4.0.1)
-Requires-Dist: bosdyn-core (==4.0.1)
-Requires-Dist: bosdyn-client (==4.0.1)
+Requires-Dist: bosdyn-api (==4.0.2)
+Requires-Dist: bosdyn-core (==4.0.2)
+Requires-Dist: bosdyn-client (==4.0.2)
 
 <!--
 Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 
 Downloading, reproducing, distributing or otherwise using the SDK Software
 is subject to the terms and conditions of the Boston Dynamics Software
 Development Kit License (20191101-BDSDK-SL).
```

## Comparing `bosdyn_choreography_client-4.0.1.dist-info/RECORD` & `bosdyn_choreography_client-4.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 bosdyn/__init__.py,sha256=CMQioQKK1NlMk3kZuY49b_Aw-JyvDeOtuqOCAul1I0s,330
 bosdyn/choreography/__init__.py,sha256=CMQioQKK1NlMk3kZuY49b_Aw-JyvDeOtuqOCAul1I0s,330
 bosdyn/choreography/client/__init__.py,sha256=CMQioQKK1NlMk3kZuY49b_Aw-JyvDeOtuqOCAul1I0s,330
 bosdyn/choreography/client/animation_file_conversion_helpers.py,sha256=iBEqEGAZknyh8WWxtxZrzoA-o8BDJ7a5pmft0kqNCrs,18438
 bosdyn/choreography/client/animation_file_to_proto.py,sha256=-24pM175p2d0zExWqwpHbxwF26gkPPDsU1BvGHTAQr4,25971
-bosdyn/choreography/client/choreography.py,sha256=xNE2IqJxlYyTMON5HNUUNnO5rFFS7C9meLkuXjjhUS0,48849
-bosdyn_choreography_client-4.0.1.dist-info/METADATA,sha256=EhyriEu4v7FtX0T0LQNU7f77uTg1SJHvgr05v640fug,1721
-bosdyn_choreography_client-4.0.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-bosdyn_choreography_client-4.0.1.dist-info/top_level.txt,sha256=an2OWgx1ej2jFjmBjPWNQ68ZglvUfKhmXWW-WhTtDmA,7
-bosdyn_choreography_client-4.0.1.dist-info/RECORD,,
+bosdyn/choreography/client/choreography.py,sha256=tMfQ7MFSzgLHxBSFYHpBDc0uPoZr2zC90JJJpfI7sXQ,50633
+bosdyn_choreography_client-4.0.2.dist-info/METADATA,sha256=67xGEVQrYTtThR1ZENh-NbcbSLWjAMWMfmIAHl3dO0M,1721
+bosdyn_choreography_client-4.0.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+bosdyn_choreography_client-4.0.2.dist-info/top_level.txt,sha256=an2OWgx1ej2jFjmBjPWNQ68ZglvUfKhmXWW-WhTtDmA,7
+bosdyn_choreography_client-4.0.2.dist-info/RECORD,,
```

