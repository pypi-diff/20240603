# Comparing `tmp/imgori-0.3.1-py3-none-any.whl.zip` & `tmp/imgori-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,28 @@
-Zip file size: 11843 bytes, number of entries: 26
+Zip file size: 12062 bytes, number of entries: 26
 -rwxr-xr-x  2.0 unx      139 b- defN 80-Jan-01 00:00 imgori/__init__.py
 -rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 imgori/cli.py
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 imgori/commands/__init__.py
 -rw-r--r--  2.0 unx     1344 b- defN 80-Jan-01 00:00 imgori/commands/train.py
 -rwxr-xr-x  2.0 unx       72 b- defN 80-Jan-01 00:00 imgori/datasets/__init__.py
 -rw-r--r--  2.0 unx     2156 b- defN 80-Jan-01 00:00 imgori/datasets/imgori.py
 -rwxr-xr-x  2.0 unx      650 b- defN 80-Jan-01 00:00 imgori/datasets/mnist.py
 -rw-r--r--  2.0 unx      267 b- defN 80-Jan-01 00:00 imgori/datasets/utils.py
--rw-r--r--  2.0 unx     1673 b- defN 80-Jan-01 00:00 imgori/imgori.py
+-rw-r--r--  2.0 unx     1442 b- defN 80-Jan-01 00:00 imgori/imgori.py
 -rwxr-xr-x  2.0 unx      103 b- defN 80-Jan-01 00:00 imgori/nn/__init__.py
 -rw-r--r--  2.0 unx      436 b- defN 80-Jan-01 00:00 imgori/nn/efficientnet.py
 -rw-r--r--  2.0 unx      968 b- defN 80-Jan-01 00:00 imgori/nn/lenet.py
 -rw-r--r--  2.0 unx      448 b- defN 80-Jan-01 00:00 imgori/nn/mobilenet_v3.py
 -rw-r--r--  2.0 unx      202 b- defN 80-Jan-01 00:00 imgori/optim.py
 -rwxr-xr-x  2.0 unx       66 b- defN 80-Jan-01 00:00 imgori/trainers/__init__.py
--rw-r--r--  2.0 unx     4073 b- defN 80-Jan-01 00:00 imgori/trainers/imgori.py
+-rw-r--r--  2.0 unx     4054 b- defN 80-Jan-01 00:00 imgori/trainers/imgori.py
 -rw-r--r--  2.0 unx     4087 b- defN 80-Jan-01 00:00 imgori/trainers/mnist.py
 -rw-r--r--  2.0 unx       70 b- defN 80-Jan-01 00:00 imgori/trainers/trainer.py
 -rw-r--r--  2.0 unx     2398 b- defN 80-Jan-01 00:00 imgori/typing.py
--rwxr-xr-x  2.0 unx      233 b- defN 80-Jan-01 00:00 imgori/utils/__init__.py
--rw-r--r--  2.0 unx     1212 b- defN 80-Jan-01 00:00 imgori/utils/s3.py
+-rwxr-xr-x  2.0 unx      177 b- defN 80-Jan-01 00:00 imgori/utils/__init__.py
+-rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 imgori/utils/hub.py
 -rw-r--r--  2.0 unx      744 b- defN 80-Jan-01 00:00 imgori/utils/utils.py
--rw-r--r--  2.0 unx      666 b- defN 80-Jan-01 00:00 imgori-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 imgori-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 imgori-0.3.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2013 b- defN 16-Jan-01 00:00 imgori-0.3.1.dist-info/RECORD
-26 files, 24224 bytes uncompressed, 8625 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx      666 b- defN 80-Jan-01 00:00 imgori-0.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 imgori-0.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 imgori-0.3.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2014 b- defN 16-Jan-01 00:00 imgori-0.3.2.dist-info/RECORD
+26 files, 24576 bytes uncompressed, 8842 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -54,26 +54,26 @@
 
 Filename: imgori/typing.py
 Comment: 
 
 Filename: imgori/utils/__init__.py
 Comment: 
 
-Filename: imgori/utils/s3.py
+Filename: imgori/utils/hub.py
 Comment: 
 
 Filename: imgori/utils/utils.py
 Comment: 
 
-Filename: imgori-0.3.1.dist-info/METADATA
+Filename: imgori-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: imgori-0.3.1.dist-info/WHEEL
+Filename: imgori-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: imgori-0.3.1.dist-info/entry_points.txt
+Filename: imgori-0.3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: imgori-0.3.1.dist-info/RECORD
+Filename: imgori-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## imgori/imgori.py

```diff
@@ -1,49 +1,46 @@
 import torch
 from torch import nn
-from torch.hub import load_state_dict_from_url
 from torchvision.transforms._presets import ImageClassification
 
 from .nn import mobilenet_v3
 from .typing import Orientation
-from .typing import PathLike
 from .typing import PILImage
-from .utils import load_state_dict_from_s3_url
+from .utils import download_url
 
 DEFAULT_MODEL = (
     "https://github.com/narumiruna/imgori/releases/download/v0.2.7-mobilenet-v3/imgori_mobilenet_v3_small.pth"  # noqa
 )
 
 
-def load_model(model_path: PathLike, device: torch.device | str = "cpu") -> nn.Module:
-    model_path = str(model_path)
-
-    if model_path.startswith("https://"):
-        state_dict = load_state_dict_from_url(model_path, map_location=device, progress=True)
-    elif model_path.startswith("s3://"):
-        state_dict = load_state_dict_from_s3_url(model_path, map_location=device)
-    else:
-        state_dict = torch.load(model_path, map_location=device)
-
-    model = mobilenet_v3(num_classes=len(Orientation))
-    model.load_state_dict(state_dict["model"])
-    model.eval()
-    return model.to(device)
-
-
 class Imgori:
+    model: nn.Module
+    transform: ImageClassification
+
     def __init__(
         self,
-        model_path: PathLike | None = None,
+        model_path: str | None = None,
         device: torch.device | str = "cpu",
     ):
-        self.model = load_model(model_path or DEFAULT_MODEL, device)
         self.device = device
         self.transform = ImageClassification(crop_size=224, resize_size=256)
 
+        self.model = self.load_model(model_path or DEFAULT_MODEL)
+
+    def load_model(self, model_path: str) -> nn.Module:
+        if model_path.startswith(("s3://", "http://", "https://")):
+            model_path = download_url(model_path)
+
+        state_dict = torch.load(model_path, map_location=self.device)
+
+        model = mobilenet_v3(num_classes=len(Orientation))
+        model.load_state_dict(state_dict["model"])
+        model.eval()
+        return model.to(self.device)
+
     @torch.no_grad()
     def __call__(self, img: PILImage) -> Orientation:
         img_tensor = self.transform(img)
         img_tensor = img_tensor.unsqueeze(0).to(self.device)
         output = self.model(img_tensor)
         output = output.argmax(dim=1).item()
         return Orientation(output)
```

## imgori/trainers/imgori.py

```diff
@@ -2,16 +2,16 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from mlconfig import register
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import LRScheduler
 from torch.utils.data import DataLoader
-from torchmetrics import Accuracy
 from torchmetrics import MeanMetric
+from torchmetrics.classification import MulticlassAccuracy
 from tqdm import tqdm
 from tqdm import trange
 
 from ..typing import PathLike
 from .trainer import Trainer
 
 
@@ -34,15 +34,15 @@
         self.scheduler = scheduler
         self.train_loader = train_loader
         self.valid_loader = valid_loader
         self.num_epochs = num_epochs
         self.num_classes = num_classes
 
         self.state = {"epoch": 1}
-        self.metrics = {"best_acc": 0}
+        self.metrics = {"best_acc": 0.0}
 
     def fit(self) -> None:
         start_epoch = self.state["epoch"]
         for epoch in trange(start_epoch, self.num_epochs + 1):
             self.train()
             self.validate()
             self.scheduler.step()
@@ -55,63 +55,63 @@
             tqdm.write(format_string)
 
             self.state["epoch"] = epoch + 1
 
     def train(self) -> None:
         self.model.train()
 
-        loss_metric = MeanMetric().to(self.device)
-        acc_metric = Accuracy(task="multiclass", num_classes=self.num_classes).to(self.device)
+        loss_metric = MeanMetric()
+        acc_metric = MulticlassAccuracy(num_classes=self.num_classes)
 
         for x, y in tqdm(self.train_loader):
             x = x.to(self.device)
             y = y.to(self.device)
 
             output = self.model(x)
             loss = F.cross_entropy(output, y)
 
             self.optimizer.zero_grad()
             loss.backward()
             self.optimizer.step()
 
-            loss_metric.update(loss, weight=x.size(0))
-            acc_metric.update(output, y)
+            loss_metric.update(loss.cpu(), weight=x.size(0))
+            acc_metric.update(output.cpu(), y.cpu())
 
         self.metrics.update(
-            train_loss=loss_metric.compute().item(),
-            train_acc=acc_metric.compute().item(),
+            train_loss=float(loss_metric.compute()),
+            train_acc=float(acc_metric.compute()),
         )
 
         del loss_metric
         del acc_metric
 
     @torch.no_grad()
     def validate(self) -> None:
         self.model.eval()
 
-        loss_metric = MeanMetric().to(self.device)
-        acc_metric = Accuracy(task="multiclass", num_classes=self.num_classes).to(self.device)
+        loss_metric = MeanMetric()
+        acc_metric = MulticlassAccuracy(num_classes=self.num_classes)
 
         for x, y in tqdm(self.valid_loader):
             x = x.to(self.device)
             y = y.to(self.device)
 
             output = self.model(x)
             loss = F.cross_entropy(output, y)
 
-            loss_metric.update(loss, weight=x.size(0))
-            acc_metric.update(output, y)
+            loss_metric.update(loss.cpu(), weight=x.size(0))
+            acc_metric.update(output.cpu(), y.cpu())
 
-        valid_acc = acc_metric.compute().item()
+        valid_acc = float(acc_metric.compute())
         if valid_acc > self.metrics["best_acc"]:
             self.metrics["best_acc"] = valid_acc
             self.save_checkpoint("best.pth")
 
         self.metrics.update(
-            valid_loss=loss_metric.compute().item(),
+            valid_loss=float(loss_metric.compute()),
             valid_acc=valid_acc,
         )
 
         del loss_metric
         del acc_metric
 
     def save_checkpoint(self, f: PathLike) -> None:
```

## imgori/utils/__init__.py

```diff
@@ -1,7 +1,6 @@
-from .s3 import download_file_from_s3_url
-from .s3 import load_state_dict_from_s3_url
+from .hub import download_url
 from .utils import load_json
 from .utils import load_yaml
 from .utils import manual_seed
 from .utils import save_json
 from .utils import save_yaml
```

## Comparing `imgori-0.3.1.dist-info/METADATA` & `imgori-0.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgori
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `imgori-0.3.1.dist-info/RECORD` & `imgori-0.3.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 imgori/cli.py,sha256=9-LsBqnc0-ncex4EbIOHEAGPw5xBXZ57pHZW1R7a1Pk,50
 imgori/commands/__init__.py,sha256=tNKqfMuVB5L96buP08z08lQhgFmW-OSxvVuodpRbQfM,25
 imgori/commands/train.py,sha256=8-K4aToL4z4mwRQ4AUL7ENwkqQ06SEuMhEu2fkBMfAQ,1344
 imgori/datasets/__init__.py,sha256=4IEJ1jDWbYPWQhyS0-aU3r4m5hJ58pZn0DSiYqnZyhc,72
 imgori/datasets/imgori.py,sha256=OgfwW0sa1NgI7jibg7DPhO11BuMaxU7VOydlhjETANA,2156
 imgori/datasets/mnist.py,sha256=eAk2Ecyp51Xu84Y-RJi5VYiyBpTosX2IvsKpBiE3Fls,650
 imgori/datasets/utils.py,sha256=2fEk28jop1QgfwhiniYtEvbVdr3fE-DMDq9y0m8SVNM,267
-imgori/imgori.py,sha256=N0Oy-fv1P_H-4hs-z_heu3PvswJw75oKCJ48HbeASbk,1673
+imgori/imgori.py,sha256=Exbqh14-jcAeUpry2Omg7DB2SLzfGmKXijvC2VhXtOc,1442
 imgori/nn/__init__.py,sha256=Kc8dsNIqvRWAD0N9tkvLsqRL29ePjCEYQHaeQzG2U9k,103
 imgori/nn/efficientnet.py,sha256=QvKjk1q-CpdIesgOKUNtSjsdmPsXSxllWd1_8o_RMXc,436
 imgori/nn/lenet.py,sha256=g5gz1u_RAFSLuDvnMqDg2ZejoQk9lNBIZqCh-LP0Ws0,968
 imgori/nn/mobilenet_v3.py,sha256=eFENzM9P2ZJHNQ3UurqLAoRZgJargYPB7th_HdcM0hs,448
 imgori/optim.py,sha256=E_eXbOhpeYRqr70ghXTYLB7GeyNBsiTv3ycw2fe1VWU,202
 imgori/trainers/__init__.py,sha256=LA1hhnTzmv_EpMtqivqmMrIR6JLXFFlWBRFcASwiaGY,66
-imgori/trainers/imgori.py,sha256=cCUgTc2HkLOVSvzvLxVQpTHF3ImoG77AmfKHlk5w4zU,4073
+imgori/trainers/imgori.py,sha256=eLk4ZO6zf34yD6_IeRjvzbLe8HBzfQHzj8msZdzVteo,4054
 imgori/trainers/mnist.py,sha256=2DAhfGS5BYr9Bf9JVK_8FxwXbycvGansGqtAXfmieYI,4087
 imgori/trainers/trainer.py,sha256=72H5BlWgjYNV1YOwiePjP-PlSANx-kzz3jhCItsZxJs,70
 imgori/typing.py,sha256=2dVGFx8tHvn69yBb587pnvOFTaGGq0-XTGakXq1NUyM,2398
-imgori/utils/__init__.py,sha256=Z6XbCnKBP5UGMxt60JvwNu69XDJkVSHHZSW1SManhCA,233
-imgori/utils/s3.py,sha256=JA6NeafTO4JtGsbuohNKfKSEK7m9Mf9QPxzAUZJAN2c,1212
+imgori/utils/__init__.py,sha256=wqulxmCuvT01DRCF_BliRm0hLj9trYlKjloNRc2xpF0,177
+imgori/utils/hub.py,sha256=JUw7RM_GtGja2OKNxwjpxOb55s9CbdEcMpo04xkLSyc,1869
 imgori/utils/utils.py,sha256=cnfH6VaOeBzZNVfsEIesXG6eTP1RgivFW5qjk_msOxg,744
-imgori-0.3.1.dist-info/METADATA,sha256=7NX_Macj919FXCtpwdR9SdzhC4HYegrsxjwQwlWUvuk,666
-imgori-0.3.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-imgori-0.3.1.dist-info/entry_points.txt,sha256=RBRze5SLMBGEr6NDoc_nszbzHABf-V8Wl_-VYMRwwic,41
-imgori-0.3.1.dist-info/RECORD,,
+imgori-0.3.2.dist-info/METADATA,sha256=kJcocgMUc9aQioqDH9dG3HYkMjTCpaVc8wVquSDuD2s,666
+imgori-0.3.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+imgori-0.3.2.dist-info/entry_points.txt,sha256=RBRze5SLMBGEr6NDoc_nszbzHABf-V8Wl_-VYMRwwic,41
+imgori-0.3.2.dist-info/RECORD,,
```

