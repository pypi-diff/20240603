# Comparing `tmp/madrin-0.0.1-py3-none-any.whl.zip` & `tmp/madrin-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4037 bytes, number of entries: 7
+Zip file size: 4562 bytes, number of entries: 7
 -rwxrwxrwx  2.0 unx       65 b- defN 24-Jun-01 18:17 madrin/__init__.py
--rwxrwxrwx  2.0 unx     4576 b- defN 24-Jun-01 18:17 madrin/madrin.py
--rwxrwxrwx  2.0 unx     1068 b- defN 24-Jun-01 18:21 madrin-0.0.1.dist-info/LICENSE
--rwxrwxrwx  2.0 unx     1620 b- defN 24-Jun-01 18:21 madrin-0.0.1.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 24-Jun-01 18:21 madrin-0.0.1.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        7 b- defN 24-Jun-01 18:21 madrin-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      526 b- defN 24-Jun-01 18:21 madrin-0.0.1.dist-info/RECORD
-7 files, 7954 bytes uncompressed, 3107 bytes compressed:  60.9%
+-rwxrwxrwx  2.0 unx     4617 b- defN 24-Jun-03 11:15 madrin/madrin.py
+-rwxrwxrwx  2.0 unx     1068 b- defN 24-Jun-03 11:16 madrin-0.0.2.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx     2626 b- defN 24-Jun-03 11:16 madrin-0.0.2.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 24-Jun-03 11:16 madrin-0.0.2.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        7 b- defN 24-Jun-03 11:16 madrin-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      526 b- defN 24-Jun-03 11:16 madrin-0.0.2.dist-info/RECORD
+7 files, 9001 bytes uncompressed, 3632 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: madrin/__init__.py
 Comment: 
 
 Filename: madrin/madrin.py
 Comment: 
 
-Filename: madrin-0.0.1.dist-info/LICENSE
+Filename: madrin-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: madrin-0.0.1.dist-info/METADATA
+Filename: madrin-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: madrin-0.0.1.dist-info/WHEEL
+Filename: madrin-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: madrin-0.0.1.dist-info/top_level.txt
+Filename: madrin-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: madrin-0.0.1.dist-info/RECORD
+Filename: madrin-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## madrin/madrin.py

```diff
@@ -86,14 +86,18 @@
         self.costs=[]
 
     def forward(self,inputs):
         for layer in self.layers:
             inputs=layer.forward(inputs)
         return inputs
 
+    def compile(self, loss, lr):
+        self.loss=loss
+        self.lr=lr
+
     def backward(self,x,y,lr):
         gradient_outputs=self.derivative_of_loss(x,y)
         for layer in reversed(self.layers):
             gradient_outputs=layer.backward(gradient_outputs,lr)
 
     def derivative_of_loss(self,samples,labels):
         outputs = self.forward(samples)
@@ -102,25 +106,24 @@
         
         elif self.loss == 'categorical_crossentropy':
             one_hot=np.zeros((labels.shape[0], self.layers[-1].activations.shape[1]))
             one_hot[np.arange(labels.shape[0]), labels] = 1
             clipped_outputs = np.clip(outputs, 1e-15, 1 - 1e-15)
             return -(one_hot/clipped_outputs)
 
-    def fit(self, x, y, lr, epochs, loss='mse'):
-        self.loss=loss
+    def fit(self, x, y, epochs):
         for i in range(epochs):
-            self.backward(x,y,lr)
+            self.backward(x,y,self.lr)
             self.costs.append(self.cost(x,y))
 
     def cost(self,samples,labels):
         outputs = self.forward(samples)
         if self.loss == 'mse':
             return np.mean(np.sum(((outputs-labels)**2),axis=1,keepdims=True))
         
         elif self.loss == 'categorical_crossentropy':
             clipped_outputs = np.clip(outputs, 1e-15, 1 - 1e-15)
             correct_class_probs = clipped_outputs[np.arange(samples.shape[0]), labels]
             return np.mean(-np.log(correct_class_probs))
         
         else:
-            print("Specify a valid loss function(mse or categorical_crossentropy)")
+            print("Specify a valid loss function(mse or categorical_crossentropy)")
```

## Comparing `madrin-0.0.1.dist-info/LICENSE` & `madrin-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `madrin-0.0.1.dist-info/RECORD` & `madrin-0.0.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 madrin/__init__.py,sha256=hdx_iOXDv6TIOvSZ9kLFq9BxLrPFATy4RL34pNLB8k8,65
-madrin/madrin.py,sha256=QC3mh50hs2833u8Jcy2vPSTJO0iQaAu7YQaO42ivbUI,4576
-madrin-0.0.1.dist-info/LICENSE,sha256=xjmTeu2PKn--NS1aSrvtSNzdu6f_cd8az--QVb7ulDY,1068
-madrin-0.0.1.dist-info/METADATA,sha256=GSanytkdatHfKU5U-G5QOFrvsLfGS8kYbVWDCAkBGxw,1620
-madrin-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-madrin-0.0.1.dist-info/top_level.txt,sha256=uhVba1Z0DrpVlE76TWIrVTYdyoU2tqYDg9VaXm51uAU,7
-madrin-0.0.1.dist-info/RECORD,,
+madrin/madrin.py,sha256=0frVmaTHA2irDLNizpQkGnjhQ0iMdZdjnitiUPAAbBw,4617
+madrin-0.0.2.dist-info/LICENSE,sha256=xjmTeu2PKn--NS1aSrvtSNzdu6f_cd8az--QVb7ulDY,1068
+madrin-0.0.2.dist-info/METADATA,sha256=7k9-OeJd6Z-p-WIO11cO3rwELlbiQTdYLTHo8XEZS5Q,2626
+madrin-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+madrin-0.0.2.dist-info/top_level.txt,sha256=uhVba1Z0DrpVlE76TWIrVTYdyoU2tqYDg9VaXm51uAU,7
+madrin-0.0.2.dist-info/RECORD,,
```

