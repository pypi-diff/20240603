# Comparing `tmp/multi_med_image_ml-0.0.8.tar.gz` & `tmp/multi_med_image_ml-0.0.9.tar.gz`

## Comparing `multi_med_image_ml-0.0.8.tar` & `multi_med_image_ml-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,29 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/setup.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0   332414 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/.images/logo.png
--rw-r--r--   0        0        0  2707942 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/.images/model_diagram.png
--rw-r--r--   0        0        0   328523 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/.images/regress_figure.png
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/example/example_train.py
--rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/example/example_train.sh
--rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/example/options/base_options.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/example/options/test_options.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/example/options/train_options.py
--rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/DataBaseWrapper.py
--rwxr-xr-x   0        0        0    10918 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/MedImageLoader.py
--rw-r--r--   0        0        0    19875 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/MultiInputTester.py
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/MultiInputTrainer.py
--rw-r--r--   0        0        0    10139 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/Records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/__init__.py
--rw-r--r--   0        0        0    17645 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/models.py
--rw-r--r--   0        0        0    46176 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/src/multi_med_image_ml/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/tests/unit_tests.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/tests/weights.json
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/README.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/setup.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0   332414 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/.images/logo.png
+-rw-r--r--   0        0        0  2707942 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/.images/model_diagram.png
+-rw-r--r--   0        0        0   328523 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/.images/regress_figure.png
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/example/example_train.py
+-rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/example/example_train.sh
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/example/MultiMedImageML_workflow/example_train.py
+-rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/example/MultiMedImageML_workflow/example_train.sh
+-rw-r--r--   0        0        0 18448384 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/example/MultiMedImageML_workflow/temp.pkl
+-rw-r--r--   0        0        0    47117 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/example/MultiMedImageML_workflow/results/AlzStage/loss_ims/AlzStage_loss.png
+-rw-r--r--   0        0        0    19456 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/example/MultiMedImageML_workflow/results/AlzStage/loss_ims/AlzStage_vals.npy
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/example/options/base_options.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/example/options/test_options.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/example/options/train_options.py
+-rw-r--r--   0        0        0    10580 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/src/multi_med_image_ml/DataBaseWrapper.py
+-rwxr-xr-x   0        0        0    10970 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/src/multi_med_image_ml/MedImageLoader.py
+-rw-r--r--   0        0        0    19875 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/src/multi_med_image_ml/MultiInputTester.py
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/src/multi_med_image_ml/MultiInputTrainer.py
+-rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/src/multi_med_image_ml/Records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/src/multi_med_image_ml/__init__.py
+-rw-r--r--   0        0        0    17582 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/src/multi_med_image_ml/models.py
+-rw-r--r--   0        0        0    46137 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/src/multi_med_image_ml/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/tests/unit_tests.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/tests/weights.json
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/README.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.9/PKG-INFO
```

### Comparing `multi_med_image_ml-0.0.8/.github/workflows/publish-to-pypi.yml` & `multi_med_image_ml-0.0.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.8/.images/logo.png` & `multi_med_image_ml-0.0.9/.images/logo.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.8/.images/model_diagram.png` & `multi_med_image_ml-0.0.9/.images/model_diagram.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.8/.images/regress_figure.png` & `multi_med_image_ml-0.0.9/.images/regress_figure.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.8/example/example_train.py` & `multi_med_image_ml-0.0.9/example/example_train.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.8/example/options/base_options.py` & `multi_med_image_ml-0.0.9/example/options/base_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.8/example/options/test_options.py` & `multi_med_image_ml-0.0.9/example/options/test_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.8/example/options/train_options.py` & `multi_med_image_ml-0.0.9/example/options/train_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.8/src/multi_med_image_ml/DataBaseWrapper.py` & `multi_med_image_ml-0.0.9/src/multi_med_image_ml/DataBaseWrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 	def __init__(self,
 					all_vars = None,
 					filename=None,
 					labels=[],
 					confounds=[],
 					dim=None,
 					cdim=None,
-					key_to_filename = key_to_filename_default):
+					key_to_filename = key_to_filename_default,
+					val_ranges={}):
 		self.key_to_filename = key_to_filename
 		check_key_to_filename(self.key_to_filename)
 
 		self.filename = filename
 		self.dim = dim
+		self.val_ranges = val_ranges
 		self.labels = [] if labels is None else labels
 		self.confounds = [] if confounds is None else confounds
 		if all_vars is not None:
 			self.all_vars = all_vars
 			self.columns = set(self.all_vars.columns)
 		elif os.path.isfile(filename):
 			self.all_vars = pd.read_pickle(self.filename)
@@ -40,14 +42,28 @@
 		
 		if isinstance(self.all_vars,str) and os.path.isfile(self.all_vars)\
 			 and os.path.splitext(self.all_vars)[1] == ".pkl":
 			self.all_vars = pd.read_pickle(self.all_vars)
 	def has_im(self,im: ImageRecord):
 		fkey = self.key_to_filename(im.npy_file,reverse=True)
 		return fkey in self.all_vars.index
+	def in_val_ranges(self,fkey: str) -> bool:
+		valid = True
+		for column_name in self.val_ranges:
+			val = self.all_vars.loc[fkey,column_name]
+			if is_nan(val,inc_null_str=True):
+				return False
+			elif isinstance(val,str):
+				if val not in self.val_ranges[column_name]:
+					return False
+			elif isinstance(val,float) or isinstance(val,int):
+				min_,max_ = self.val_ranges[column_name]
+				if val < min_ or val > max_:
+					return False
+		return True
 	def build_metadata(self):
 		for l in self.labels:
 			if l not in self.all_vars.columns:
 				print("%s not in all_vars.columns" % l)
 				print(self.all_vars.columns)
 			assert(l in self.all_vars.columns)
 		for c in self.confounds:
@@ -184,15 +200,15 @@
 					break
 		
 		return val
 	def get_ID(self,npy_file):
 		id = self._get_val(npy_file,["PatientID","Patient ID"])
 		return id
 	def parse_date(self,d,date_format="%Y-%m-%d %H:%M:%S"):
-		if is_nan(d):
+		if is_nan(d,inc_null_str=True):
 			return datetime.datetime(year=1970,month=1,day=1)
 		elif is_float(d):
 			return dateutil.parser.parse(str(d))
 		else:
 			try:
 				return datetime.datetime.strptime(
 					d.replace("_"," ").split(".")[0],
@@ -205,16 +221,16 @@
 	def get_birth_date(self,npy_file: str) -> datetime.date:
 		d = self._get_val(npy_file,["BirthDTS"])
 		return self.parse_date(d)
 	
 	def loc_val(self,npy_file,c):
 		fkey = self.key_to_filename(npy_file,reverse=True)
 		try:
-			if fkey not in self.all_vars.index:
-				print("Error - %s not present in index. Adding..." % fkey)
+			#if fkey not in self.all_vars.index:
+			#	print("Error - %s not present in index. Adding..." % fkey)
 			#assert(fkey in self.all_vars.index)
 			
 			return self.all_vars.loc[fkey,c]
 		except KeyError:
 			nifti_file = get_dim_str(fkey,dim=self.dim,outtype=".nii.gz")
 			
 			if not os.path.isfile(nifti_file):
@@ -250,16 +266,17 @@
 					json_dict[item] = "_".join(
 							[str(_) for _ in sorted(json_dict[item])]
 						)
 			self.columns = self.columns.union(set(json_dict))
 			self.jdict.append(json_dict)
 			assert(len(self.jdict) > 0)
 	def get_file_list(self):
-		return [self.key_to_filename(str(_)) \
-			for _ in self.all_vars.index]
+		flist = list(filter(lambda k: self.in_val_ranges(k),
+				self.all_vars.index))
+		return [self.key_to_filename(str(_)) for _ in flist]
 	def out_dataframe(self,fkey_ass = None):
 		
 		if len(self.jdict) > 0:
 			out = pd.DataFrame(self.jdict,columns = list(self.columns))
 			out.set_index("fkey",inplace=True)
 			if len(self.all_vars) > 0:
 				self.all_vars = pd.concat([self.all_vars,out],
```

### Comparing `multi_med_image_ml-0.0.8/src/multi_med_image_ml/MedImageLoader.py` & `multi_med_image_ml-0.0.9/src/multi_med_image_ml/MedImageLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,16 @@
 				"all_vars_%s.pkl" % get_dim_str(dim=self.dim))
 		
 		self.all_vars = DataBaseWrapper(
 					filename=self.all_vars_file,
 					labels=self.label,
 					confounds=self.confounds,
 					dim=self.dim,
-					key_to_filename=key_to_filename)
+					key_to_filename=key_to_filename,
+					val_ranges=self.val_ranges)
 		if not self.pickle_input():
 			self.build_pandas_database()
 		self.all_vars.build_metadata()
 		
 		# Determine which mode the scheduler is in
 		if (self.label is not None and len(self.label) > 0):
 			self.mode = "match"
@@ -300,15 +301,15 @@
 					self.file_list_dict[self.tl()][b]
 				try:
 					if self.cache: assert self.all_vars is not None
 					img = im.get_image(augment=self.augment)
 					temp.append(im)
 					self.index += 1
 					break
-				except ImageFileError:
+				except (ImageFileError, ValueError) as e:
 					self.file_list_dict[self.tl()][b] = \
 						self.file_list_dict[self.tl()][b][1:]
 					continue
 		if len(temp) != self.batch_size:
 			print(len(temp))
 			print(temp)
 			print(self.batch_size)
```

### Comparing `multi_med_image_ml-0.0.8/src/multi_med_image_ml/MultiInputTester.py` & `multi_med_image_ml-0.0.9/src/multi_med_image_ml/MultiInputTester.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.8/src/multi_med_image_ml/MultiInputTrainer.py` & `multi_med_image_ml-0.0.9/src/multi_med_image_ml/MultiInputTrainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 		self.one_step = True
 				
 		# Outputs images of the loss function over time
 		self.loss_image_dir = loss_image_dir
 		if self.loss_image_dir is not None:
 			os.makedirs(self.loss_image_dir,exist_ok=True)
 			self.loss_image_file = os.path.join(self.loss_image_dir,
-											f"{self.name}_loss.jpg")
+											f"{self.name}_loss.png")
 			self.loss_vals_file  = os.path.join(self.loss_image_dir,
 											f"{self.name}_vals.npy")
 			self.pids_read = set()
 			self.x_files_read = set()
 			if os.path.isfile(self.loss_vals_file):
 				_ = np.load(self.loss_vals_file)
 				self.xs,self.ys,self.ys_2,self.ys_c_dud = \
```

### Comparing `multi_med_image_ml-0.0.8/src/multi_med_image_ml/Records.py` & `multi_med_image_ml-0.0.9/src/multi_med_image_ml/Records.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,16 @@
 		elif self.get_image_type() == "nifti":
 			self.image = nb.load(self.filename).get_fdata()
 		elif self.get_image_type() == "npy":
 			self.image = np.load(self.filename)
 		elif self.get_image_type() == "dicom":
 			self.image = dicom.dcmread(self.filename).pixel_array
 		else:
+			print("Error in %s" % self.filename)
+			print("Error in %s" % self.npy_file)
 			raise Exception("Unsupported image type: %s"%self.get_image_type())
 		self.image = resize_np(self.image,self.dim)
 		if self.cache and not os.path.isfile(self.cached_record):
 			np.save(self.cached_record,self.image)
 		if self.all_vars is not None:
 			self.all_vars.add_json(nifti_file=self.filename)
 		if self.dtype == "torch":
```

### Comparing `multi_med_image_ml-0.0.8/src/multi_med_image_ml/models.py` & `multi_med_image_ml-0.0.9/src/multi_med_image_ml/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 	arr = np.zeros((d,))
 	pos = int(age / max_age * 1000)
 	for i in range(d):
 		arr[i] = time_index(i,pos,d)
 	return arr
 
 def get_age_encoding(date,birthdate,d=512):
+	if date is None or birthdate is None:
+		return np.zeros((d,0))
 	age = date.year - birthdate.year
 	return get_age_arr(age,d=d)
 
 # https://stackoverflow.com/questions/26685067/represent-a-hash-string-to-binary-in-python
 # Two functions to encode strings as binary arrays
 def text_to_bin(text, n_bin=32,d=512):
 	if text is None: text=""
@@ -398,22 +400,18 @@
 				if len(x.get_static_inputs()[0]) > 0:
 					static_inputs = [_[0] for _ in x.get_static_inputs()]
 					if self.n_stat_inputs != len(static_inputs):
 						raise Exception(
 					"Number of static inputs not equal to input: %d != %d"\
 						 % (len(static_inputs),self.n_stat_inputs))
 				dates1 = x.get_exam_dates()
-				for d in dates1:
-					if d is None:
-						raise Exception("Dates cannot be none")
 				bdates = x.get_birth_dates()
-				for b in bdates:
-					if b is None:
-						raise Exception("Birth dates cannot be none")
-				bdate1 = bdates[0]
+				for i,b in enumerate(bdates):
+					if b is not None:
+						bdate1 = b
 				x = x.get_image()
 				assert(torch.is_tensor(x))
 				
 			if (self.encode_age and (dates is None or bdate is None)):
 				raise Exception("Need dates as input to encode age")
 			if x.size(0) > self.n_dyn_inputs:
 				raise Exception(
```

### Comparing `multi_med_image_ml-0.0.8/src/multi_med_image_ml/utils.py` & `multi_med_image_ml-0.0.9/src/multi_med_image_ml/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,16 +334,14 @@
 		nifti_data = nifti_data.astype(np.float32)
 	if len(nifti_data.shape) != len(dim):
 		nifti_data = np.squeeze(nifti_data)
 		if len(nifti_data.shape) != len(dim):
 			nifti_data = np.squeeze(np.mean(nifti_data,axis=-1))
 		assert(len(nifti_data.shape) == len(dim))
 	if nifti_data.shape != tuple(dim):
-		print(nifti_data.shape)
-		print(dim)
 		zp = [dim[i]/nifti_data.shape[i] for i in range(len(dim))]
 		nifti_data = ndimage.zoom(nifti_data,zp)
 	return nifti_data
 
 # Prime number functions used in the data matching schemes
 def prime(i, primes):
 	for prime in primes:
```

### Comparing `multi_med_image_ml-0.0.8/tests/unit_tests.py` & `multi_med_image_ml-0.0.9/tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.8/README.md` & `multi_med_image_ml-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.8/pyproject.toml` & `multi_med_image_ml-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "multi_med_image_ml"
 
-version = "0.0.8"
+version = "0.0.9"
 
 dependencies = [
   "numpy",
   "scipy",
   "torch",
   "torchvision",
   "opencv-python>=4.5.4",
```

### Comparing `multi_med_image_ml-0.0.8/PKG-INFO` & `multi_med_image_ml-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: multi_med_image_ml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Deep learning library to encode multiple brain images and other electronic health record data in disease detection.
 Project-URL: Homepage, https://github.com/mleming/MultiMedImageML
 Author-email: Matt Leming <mleming@mgh.harvard.edu>
 Maintainer-email: Matt Leming <mleming@mgh.harvard.edu>
 License: MIT License
 Keywords: biomedical,deep learning,ehr,machine learning,mri,pytorch
 Requires-Python: >=3.8
```

