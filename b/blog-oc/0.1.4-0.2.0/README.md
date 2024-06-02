# Comparing `tmp/blog-oc-0.1.4.tar.gz` & `tmp/blog-oc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blog-oc-0.1.4.tar", last modified: Wed Mar  6 14:31:14 2024, max compression
+gzip compressed data, was "blog-oc-0.2.0.tar", last modified: Sun Jun  2 22:37:34 2024, max compression
```

## Comparing `blog-oc-0.1.4.tar` & `blog-oc-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-03-06 14:31:14.939574 blog-oc-0.1.4/
--rw-rw-r--   0 bast      (1000) bast      (1000)      360 2023-11-26 23:39:23.000000 blog-oc-0.1.4/LICENSE
--rw-rw-r--   0 bast      (1000) bast      (1000)      823 2024-03-06 14:31:14.939574 blog-oc-0.1.4/PKG-INFO
--rw-rw-r--   0 bast      (1000) bast      (1000)      214 2024-01-04 21:35:43.000000 blog-oc-0.1.4/README.md
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-03-06 14:31:14.939574 blog-oc-0.1.4/blog/
--rw-rw-r--   0 bast      (1000) bast      (1000)      264 2024-01-05 00:04:55.000000 blog-oc-0.1.4/blog/__init__.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     1991 2024-02-22 16:00:01.000000 blog-oc-0.1.4/blog/__main__.py
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-03-06 14:31:14.939574 blog-oc-0.1.4/blog/definitions/
--rw-rw-r--   0 bast      (1000) bast      (1000)      480 2024-01-04 21:35:43.000000 blog-oc-0.1.4/blog/definitions/category.json
--rw-rw-r--   0 bast      (1000) bast      (1000)     1101 2024-01-04 21:35:43.000000 blog-oc-0.1.4/blog/definitions/category_locale.json
--rw-rw-r--   0 bast      (1000) bast      (1000)     1195 2024-01-04 21:35:43.000000 blog-oc-0.1.4/blog/definitions/comment.json
--rw-rw-r--   0 bast      (1000) bast      (1000)     1122 2024-01-04 21:35:43.000000 blog-oc-0.1.4/blog/definitions/media.json
--rw-rw-r--   0 bast      (1000) bast      (1000)     1621 2024-01-04 21:35:43.000000 blog-oc-0.1.4/blog/definitions/post.json
--rw-rw-r--   0 bast      (1000) bast      (1000)      531 2024-01-04 21:35:43.000000 blog-oc-0.1.4/blog/definitions/post_category.json
--rw-rw-r--   0 bast      (1000) bast      (1000)     1698 2024-01-04 21:35:43.000000 blog-oc-0.1.4/blog/definitions/post_raw.json
--rw-rw-r--   0 bast      (1000) bast      (1000)      581 2024-01-04 21:35:43.000000 blog-oc-0.1.4/blog/definitions/post_tag.json
--rw-rw-r--   0 bast      (1000) bast      (1000)      590 2024-01-04 22:08:07.000000 blog-oc-0.1.4/blog/errors.py
--rw-rw-r--   0 bast      (1000) bast      (1000)      646 2024-01-05 00:04:55.000000 blog-oc-0.1.4/blog/install.py
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-03-06 14:31:14.939574 blog-oc-0.1.4/blog/media/
--rw-rw-r--   0 bast      (1000) bast      (1000)     1619 2024-01-04 21:35:43.000000 blog-oc-0.1.4/blog/media/__init__.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     6938 2024-01-04 21:35:43.000000 blog-oc-0.1.4/blog/media/s3.py
--rw-rw-r--   0 bast      (1000) bast      (1000)    25936 2024-03-06 14:25:38.000000 blog-oc-0.1.4/blog/records.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     2726 2024-03-02 17:25:21.000000 blog-oc-0.1.4/blog/rest.py
--rw-rw-r--   0 bast      (1000) bast      (1000)     7541 2024-03-02 17:25:21.000000 blog-oc-0.1.4/blog/seo.py
--rw-rw-r--   0 bast      (1000) bast      (1000)    52024 2024-03-06 14:14:21.000000 blog-oc-0.1.4/blog/service.py
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-03-06 14:31:14.939574 blog-oc-0.1.4/blog/translations/
--rw-rw-r--   0 bast      (1000) bast      (1000)      219 2024-03-02 17:25:21.000000 blog-oc-0.1.4/blog/translations/en-CA.json
--rw-rw-r--   0 bast      (1000) bast      (1000)      219 2024-03-02 17:25:21.000000 blog-oc-0.1.4/blog/translations/en-US.json
--rw-rw-r--   0 bast      (1000) bast      (1000)      245 2024-03-02 17:25:21.000000 blog-oc-0.1.4/blog/translations/fr-CA.json
-drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-03-06 14:31:14.939574 blog-oc-0.1.4/blog_oc.egg-info/
--rw-rw-r--   0 bast      (1000) bast      (1000)      823 2024-03-06 14:31:14.000000 blog-oc-0.1.4/blog_oc.egg-info/PKG-INFO
--rw-rw-r--   0 bast      (1000) bast      (1000)      751 2024-03-06 14:31:14.000000 blog-oc-0.1.4/blog_oc.egg-info/SOURCES.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        1 2024-03-06 14:31:14.000000 blog-oc-0.1.4/blog_oc.egg-info/dependency_links.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)       44 2024-03-06 14:31:14.000000 blog-oc-0.1.4/blog_oc.egg-info/entry_points.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)      216 2024-03-06 14:31:14.000000 blog-oc-0.1.4/blog_oc.egg-info/requires.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        5 2024-03-06 14:31:14.000000 blog-oc-0.1.4/blog_oc.egg-info/top_level.txt
--rw-rw-r--   0 bast      (1000) bast      (1000)        1 2024-03-06 14:31:14.000000 blog-oc-0.1.4/blog_oc.egg-info/zip-safe
--rw-rw-r--   0 bast      (1000) bast      (1000)       79 2024-03-06 14:31:14.939574 blog-oc-0.1.4/setup.cfg
--rw-rw-r--   0 bast      (1000) bast      (1000)     1219 2024-03-06 00:15:54.000000 blog-oc-0.1.4/setup.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-06-02 22:37:34.016028 blog-oc-0.2.0/
+-rw-rw-r--   0 bast      (1000) bast      (1000)      360 2023-11-26 23:39:23.000000 blog-oc-0.2.0/LICENSE
+-rw-rw-r--   0 bast      (1000) bast      (1000)      823 2024-06-02 22:37:34.016028 blog-oc-0.2.0/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)      214 2024-01-04 21:35:43.000000 blog-oc-0.2.0/README.md
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-06-02 22:37:34.016028 blog-oc-0.2.0/blog/
+-rw-rw-r--   0 bast      (1000) bast      (1000)      329 2024-05-27 20:15:37.000000 blog-oc-0.2.0/blog/__init__.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     2004 2024-05-28 18:28:33.000000 blog-oc-0.2.0/blog/__main__.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-06-02 22:37:34.016028 blog-oc-0.2.0/blog/definitions/
+-rw-rw-r--   0 bast      (1000) bast      (1000)      480 2024-01-04 21:35:43.000000 blog-oc-0.2.0/blog/definitions/category.json
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1101 2024-01-04 21:35:43.000000 blog-oc-0.2.0/blog/definitions/category_locale.json
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1195 2024-01-04 21:35:43.000000 blog-oc-0.2.0/blog/definitions/comment.json
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1122 2024-01-04 21:35:43.000000 blog-oc-0.2.0/blog/definitions/media.json
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1621 2024-01-04 21:35:43.000000 blog-oc-0.2.0/blog/definitions/post.json
+-rw-rw-r--   0 bast      (1000) bast      (1000)      531 2024-01-04 21:35:43.000000 blog-oc-0.2.0/blog/definitions/post_category.json
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1698 2024-01-04 21:35:43.000000 blog-oc-0.2.0/blog/definitions/post_raw.json
+-rw-rw-r--   0 bast      (1000) bast      (1000)      581 2024-01-04 21:35:43.000000 blog-oc-0.2.0/blog/definitions/post_tag.json
+-rw-rw-r--   0 bast      (1000) bast      (1000)      590 2024-01-04 22:08:07.000000 blog-oc-0.2.0/blog/errors.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)      646 2024-01-05 00:04:55.000000 blog-oc-0.2.0/blog/install.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-06-02 22:37:34.016028 blog-oc-0.2.0/blog/media/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1619 2024-01-04 21:35:43.000000 blog-oc-0.2.0/blog/media/__init__.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     6938 2024-01-04 21:35:43.000000 blog-oc-0.2.0/blog/media/s3.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)    30026 2024-06-02 22:34:51.000000 blog-oc-0.2.0/blog/records.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     2726 2024-03-02 17:25:21.000000 blog-oc-0.2.0/blog/rest.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     7578 2024-05-27 19:25:33.000000 blog-oc-0.2.0/blog/seo.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)    54051 2024-06-02 22:26:46.000000 blog-oc-0.2.0/blog/service.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     4893 2024-05-28 18:41:21.000000 blog-oc-0.2.0/blog/sitemap.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-06-02 22:37:34.016028 blog-oc-0.2.0/blog/translations/
+-rw-rw-r--   0 bast      (1000) bast      (1000)      219 2024-03-02 17:25:21.000000 blog-oc-0.2.0/blog/translations/en-CA.json
+-rw-rw-r--   0 bast      (1000) bast      (1000)      219 2024-03-02 17:25:21.000000 blog-oc-0.2.0/blog/translations/en-US.json
+-rw-rw-r--   0 bast      (1000) bast      (1000)      245 2024-03-02 17:25:21.000000 blog-oc-0.2.0/blog/translations/fr-CA.json
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2024-06-02 22:37:34.016028 blog-oc-0.2.0/blog_oc.egg-info/
+-rw-rw-r--   0 bast      (1000) bast      (1000)      823 2024-06-02 22:37:34.000000 blog-oc-0.2.0/blog_oc.egg-info/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)      767 2024-06-02 22:37:34.000000 blog-oc-0.2.0/blog_oc.egg-info/SOURCES.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2024-06-02 22:37:34.000000 blog-oc-0.2.0/blog_oc.egg-info/dependency_links.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)       44 2024-06-02 22:37:34.000000 blog-oc-0.2.0/blog_oc.egg-info/entry_points.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)      216 2024-06-02 22:37:34.000000 blog-oc-0.2.0/blog_oc.egg-info/requires.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        5 2024-06-02 22:37:34.000000 blog-oc-0.2.0/blog_oc.egg-info/top_level.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2024-03-06 14:31:14.000000 blog-oc-0.2.0/blog_oc.egg-info/zip-safe
+-rw-rw-r--   0 bast      (1000) bast      (1000)       79 2024-06-02 22:37:34.016028 blog-oc-0.2.0/setup.cfg
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1219 2024-05-27 20:12:38.000000 blog-oc-0.2.0/setup.py
```

### Comparing `blog-oc-0.1.4/PKG-INFO` & `blog-oc-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blog-oc
-Version: 0.1.4
+Version: 0.2.0
 Summary: Blog contains a service to manage blog posts and comments associated
 Home-page: https://ouroboroscoding.com/body/blog
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: Custom
 Project-URL: Documentation, https://ouroboroscoding.com/body/blog
 Project-URL: Source, https://github.com/ouroboroscoding/blog
```

### Comparing `blog-oc-0.1.4/blog/__main__.py` & `blog-oc-0.2.0/blog/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,21 +48,24 @@
 	# Get the module path
 	dConfig['module'] = pathlib.Path(__file__).parent.resolve()
 
 	# Add the global prepend
 	Record_MySQL.db_prepend(config.mysql.prepend(''))
 
 	# Add the primary mysql DB
-	Record_MySQL.add_host('blog', config.mysql.hosts[dConfig['mysql_host']]({
-		'host': 'localhost',
-		'port': 3306,
-		'charset': 'utf8',
-		'user': 'root',
-		'passwd': ''
-	}))
+	Record_MySQL.add_host(
+		'blog',
+		config.mysql.hosts[dConfig['mysql_host']]({
+			'host': 'localhost',
+			'port': 3306,
+			'charset': 'utf8',
+			'user': 'root',
+			'passwd': ''
+		})
+	)
 
 	# Set the timestamp timezone
 	Record_MySQL.timestamp_timezone(
 		config.mysql.timestamp_timezone('+00:00')
 	)
 
 	# If we have no arguments
```

### Comparing `blog-oc-0.1.4/blog/definitions/category_locale.json` & `blog-oc-0.2.0/blog/definitions/category_locale.json`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/definitions/comment.json` & `blog-oc-0.2.0/blog/definitions/comment.json`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/definitions/media.json` & `blog-oc-0.2.0/blog/definitions/media.json`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/definitions/post.json` & `blog-oc-0.2.0/blog/definitions/post.json`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/definitions/post_category.json` & `blog-oc-0.2.0/blog/definitions/post_category.json`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/definitions/post_raw.json` & `blog-oc-0.2.0/blog/definitions/post_raw.json`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/definitions/post_tag.json` & `blog-oc-0.2.0/blog/definitions/post_tag.json`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/errors.py` & `blog-oc-0.2.0/blog/errors.py`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/install.py` & `blog-oc-0.2.0/blog/install.py`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/media/__init__.py` & `blog-oc-0.2.0/blog/media/__init__.py`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/media/s3.py` & `blog-oc-0.2.0/blog/media/s3.py`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/records.py` & `blog-oc-0.2.0/blog/records.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,23 @@
 __version__		= "1.0.0"
 __maintainer__	= "Chris Nasr"
 __email__		= "chris@ouroboroscoding.com"
 __created__		= "2023-11-27"
 
 # Ouroboros imports
 from config import config
+from FormatOC import Tree
 import jsonb
+from RestOC import Record_MySQL
 
 # Python imports
 import os
 import pathlib
 from typing import Dict, List
 
-# Pip imports
-from FormatOC import Tree
-from RestOC import Record_MySQL
-
 # Module variable
 _moRedis = None
 
 # Get the definitions path
 _defPath = '%s/definitions' % pathlib.Path(__file__).parent.resolve()
 
 def cache(redis=None):
@@ -409,21 +407,27 @@
 				" `p`.`_slug` = `pc`.`_slug`\n" \
 				"WHERE `p`.`_raw` = '%(id)s'" % {
 			'db': dStruct['db'],
 			'table': dStruct['table'],
 			'id': sID
 		}
 
+		print('-' * 40)
+		print(sSQL)
+
 		# Fetch the records
 		lRecords = Record_MySQL.Commands.select(
 			dStruct['host'],
 			sSQL,
 			Record_MySQL.ESelect.ALL
 		)
 
+		print('-' * 40)
+		print(lRecords)
+
 		# Go through each one
 		for d in lRecords:
 
 			# Generate the unique string
 			sSlugLocale = '%s:%s' % (d['_slug'], d['_locale'])
 
 			# Add the category to the post
@@ -584,17 +588,33 @@
 				ex = 3600
 			)
 
 			# Then immediately return as there's nothing else to do
 			return None
 
 		# Find all the associated categories and add them to the post
-		dPost['categories'] = [ d['_category'] for d in PostCategory.filter({
-			'_slug': slug
-		}, raw = [ '_category' ]) ]
+		lCategoryIDs = [
+			d['_category'] for d in PostCategory.filter({
+				'_slug': slug
+			}, raw = [ '_category' ])
+		]
+
+		# If we have no categories
+		if not lCategoryIDs:
+			dPost['categories'] = []
+
+		# Else,
+		else:
+
+			# Find the category slugs and titles for the categories associated
+			#	in the same locale as the post
+			dPost['categories'] = CategoryLocale.filter({
+				'_category': lCategoryIDs,
+				'_locale': dPost['_locale']
+			}, raw = [ '_category', 'slug', 'title' ], orderby = [ 'title' ])
 
 		# Find all the associated tags and add them to the post
 		dPost['tags'] = [ d['tag'] for d in PostTag.filter({
 			'_slug': slug
 		}, raw = [ 'tag' ]) ]
 
 		# Store the record permanently in the cache
@@ -729,27 +749,169 @@
 
 	_conf = Record_MySQL.Record.generate_config(
 		Tree.fromFile('%s/post_category.json' % _defPath),
 		override={ 'db': config.mysql.db('brain') }
 	)
 	"""Static Configuration"""
 
+	_category_key = 'blog:cat:%s'
+	"""Key used to store / fetch the cache of slugs by category / locale"""
+
 	@classmethod
 	def config(cls):
 		"""Config
 
 		Returns the configuration data associated with the record type
 
 		Returns:
 			dict
 		"""
 
 		# Return the config
 		return cls._conf
 
+	@classmethod
+	def cache_fetch(cls,
+		slug: str,
+		page: int = 0,
+		count: int = 10,
+		custom = {}
+	) -> List[str]:
+		"""Cache Fetch
+
+		Fetches the slugs of posts associated with the category
+
+		Arguments:
+			slug (str): The category to fetch the list of post slugs for
+			page (uint): The page (starting with zero) to fetch of slugs
+			count (uint): The count of slugs to return
+			custom (dict): Custom Host and DB info
+				'host' the name of the host to get/set data on
+				'append' optional postfix for dynamic DBs
+
+		Returns:
+			str[]
+		"""
+
+		# Fetch the slugs from the cache
+		sCategory = _moRedis.get(cls._category_key % slug)
+
+		# If it doesn't exist
+		if not sCategory:
+
+			# Generate and return it
+			dCategory = cls.cache_generate(slug, custom)
+			if dCategory is None:
+				return None
+
+		# If we got -1, return None
+		elif sCategory == '-1' or sCategory == b'-1':
+			return None
+
+		# Else, decode them
+		else:
+			dCategory = jsonb.decode(sCategory)
+
+		# Add the total count
+		dCategory['count'] = len(dCategory['posts'])
+
+		# Pull out the IDs specifically for the given page/count
+		iStart = page * count
+		iEnd = iStart + count
+		dCategory['posts'] = dCategory['posts'][iStart:iEnd]
+
+		# Get the individual posts and add them to the return
+		dCategory['posts'] = Post.cache_fetch(dCategory['posts'])
+
+		# Return the posts and total count
+		return dCategory
+
+	@classmethod
+	def cache_generate(cls,
+		slug: str,
+		custom = {}
+	) -> List[str]:
+		"""Cache Generate
+
+		Takes a category and generates the list of slugs available in that \
+		category and locale, then stores it in the cache for future use
+
+		Arguments:
+			slug (str): The category slug to generate the list of post slugs for
+			custom (dict): Custom Host and DB info
+				'host' the name of the host to get/set data on
+				'append' optional postfix for dynamic DBs
+
+		Returns:
+			dict
+		"""
+
+		# Get the structures
+		dStruct = cls.struct(custom)
+		dCategory = CategoryLocale.struct(custom)
+		dPost = Post.struct(custom)
+
+		# Generate the SQL to fetch all the slugs that fit the category and the
+		#	locale
+		sSQL = "SELECT `p`.`_slug`\n" \
+				"FROM `%(db)s`.`%(table)s` as `c`\n" \
+				"JOIN `%(db_cl)s`.`%(table_cl)s` as `cl`\n" \
+				"	ON `c`.`_category` = `cl`.`_category`\n" \
+				"JOIN `%(db_p)s`.`%(table_p)s` as `p`\n" \
+				"	ON `c`.`_slug` = `p`.`_slug`\n" \
+				"WHERE `cl`.`slug` = '%(slug)s'\n" \
+				"AND `cl`.`_locale` = `p`.`_locale`\n" \
+				"ORDER BY `p`.`_created` DESC" % {
+			'db': dStruct['db'],
+			'table': dStruct['table'],
+			'db_cl': dCategory['db'],
+			'table_cl': dCategory['table'],
+			'db_p': dPost['db'],
+			'table_p': dPost['table'],
+			'slug': Record_MySQL.Commands.escape(dStruct['host'], slug)
+		}
+
+		# Fetch the column of slugs
+		lSlugs = Record_MySQL.Commands.select(
+			dStruct['host'],
+			sSQL,
+			Record_MySQL.ESelect.COLUMN
+		)
+
+		# If there's nothing under that category
+		if not lSlugs:
+
+			# Mark it as not existing for an hour so that no one can overload
+			#	the DB
+			_moRedis.set(
+				cls._category_key % slug,
+				'-1',
+				ex = 3600
+			)
+
+			# Then immediately return as there's nothing else to do
+			return None
+
+		# Fetch the category info
+		dCategory = CategoryLocale.filter({
+			'slug': slug
+		}, raw = ['_category', '_locale', 'title', 'description' ], limit = 1)
+
+		# Add the post slugs to it
+		dCategory['posts'] = lSlugs
+
+		# Permanently store the data in the cache
+		_moRedis.set(
+			cls._category_key % slug,
+			jsonb.encode(dCategory)
+		)
+
+		# Return the category in case anyone needs it
+		return dCategory
+
 class PostRaw(Record_MySQL.Record):
 	"""Post Raw
 
 	Represents the raw data with all locales, categories, and tags used to \
 	make posts
 
 	Extends:
```

### Comparing `blog-oc-0.1.4/blog/rest.py` & `blog-oc-0.2.0/blog/rest.py`

 * *Files identical despite different names*

### Comparing `blog-oc-0.1.4/blog/seo.py` & `blog-oc-0.2.0/blog/seo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding=utf8
-""" Blog REST
+""" Blog SEO
 
-Handles starting the REST server using the Blog service
+Handles fetching OpenGraph / SEO related data associated with blog posts
 """
 
 __author__		= "Chris Nasr"
 __version__		= "1.0.0"
 __copyright__	= "Ouroboros Coding Inc."
 __email__		= "chris@ouroboroscoding.com"
 __created__		= "2023-11-27"
@@ -42,49 +42,49 @@
 		object
 	"""
 
 	_translations = {}
 
 	def __init__(self,
 		url_root: str = '/blog/',
-		uri_post: str = 'p/',
-		uri_category: str = 'c/',
-		uri_tag: str = 't/',
+		url_post: str = 'p/',
+		url_category: str = 'c/',
+		url_tag: str = 't/',
 		page_count: int | Dict[str, int] = 10,
 		title_prefix: str = undefined,
 		title_suffix: str = undefined,
 	):
 		"""Constructor
 
 		Creates the instance and initialises member variables
 
 		Arguments:
-			locale (str): The locale to use
 			url_root (str): The root of all URLS
-			uri_post (str): The post URI prefix
-			uri_tag (str): The tag URI prefix
+			url_post (str): The post folder prefix
+			url_category (str): The category folder prefix
+			url_tag (str): The tag folder prefix
 			page_count (int | dict): The number of posts per page for all \
 				types, or a dict of { category, post, tag } with an int for \
 				each
 			title_prefix (str): Optional, the text to put before the title
 			title_suffix (str): Optional, the text to put after the title
 
 		Returns:
 			BlogSeo
 		"""
 
 		# Store the root, post, and tag prefixes
 		self._url = {
-			'cat_prefix': uri_category,
-			'cat_length': len(uri_category),
-			'post_prefix': uri_post,
-			'post_length': len(uri_post),
+			'cat_prefix': url_category,
+			'cat_length': len(url_category),
+			'post_prefix': url_post,
+			'post_length': len(url_post),
 			'root_length': len(url_root),
-			'tag_prefix': uri_tag,
-			'tag_length': len(uri_tag)
+			'tag_prefix': url_tag,
+			'tag_length': len(url_tag)
 		}
 
 		# Store the page count options
 		#	If we got an int, apply it to all types
 		if isinstance(page_count, int):
 			self._counts = {
 				'category': page_count,
```

### Comparing `blog-oc-0.1.4/blog/service.py` & `blog-oc-0.2.0/blog/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1369,14 +1369,15 @@
 		bChanges = False
 
 		# Init possible errors, a dict of slugs to locales, and a list of
 		#	locales with tags that need to be regenerated
 		lErrors = []
 		lsTagLocales = set()
 		lsPostsLocales = set()
+		dLocalesCategories = {}
 		dLocalesTags = {}
 		dSlugs = {}
 
 		# Go through each locale
 		for k in oRaw['locales']:
 			if oRaw['locales'][k]['slug'] in dSlugs:
 				lErrors.append(
@@ -1436,37 +1437,54 @@
 		# Do we have any published posts left?
 		if dPosts:
 
 			# Go through each post that no longer has a counterpoint in the raw
 			#	data
 			for d in dPosts:
 
+				# Fetch all the categories that will be deleted
+				lCategories = [ d['_category'] for d in PostCategory.filter({
+					'_slug': d['_slug']
+				}, raw = [ '_category' ]) ]
+
+				# If there's any
+				if lCategories:
+
+					# Delete them
+					PostCategory.delete_get(d['_slug'], index = '_slug')
+
+					# Add them to the corresponding locale
+					try:
+						dLocalesCategories[d['_locale']].update(lCategories)
+					except KeyError:
+						dLocalesCategories[d['_locale']] = set(lCategories)
+
 				# Fetch all the tags that will be deleted
 				lTags = [ d['tag'] for d in PostTag.filter({
 					'_slug': d['_slug']
 				}, raw = [ 'tag' ]) ]
 
 				# If there's any
 				if lTags:
 
 					# Delete them
 					PostTag.delete_get(d['_slug'], index = '_slug')
 
 					# Add them to the corresponding locale
-					try: dLocalesTags[d['_locale']].update(lTags)
-					except KeyError: dLocalesTags[d['_locale']] = set(lTags)
+					try:
+						dLocalesTags[d['_locale']].update(lTags)
+					except KeyError:
+						dLocalesTags[d['_locale']] = set(lTags)
 
 				# Add the locale to the tag and posts lists so we regenerate
 				#	them
 				lsTagLocales.add(d['_locale'])
 				lsPostsLocales.add(d['_locale'])
 
-				# Delete all categories, tags, and the post itself based on the
-				#	slug
-				PostCategory.delete_get(d['_slug'], index = '_slug')
+				# Delete the post itself
 				Post.delete_get(d['_slug'])
 
 				# Delete it from the cache
 				Post.cache_delete(d['_slug'])
 
 			# Something changed
 			bChanges = True
@@ -1489,19 +1507,28 @@
 					'_locale': sLocale,
 					'title': dLocale['title'],
 					'content': dLocale['content'],
 					'meta': 'meta' in dLocale and dLocale['meta'] or {},
 					'locales': oRaw.localesToSlugs(sLocale)
 				}))
 
-				# Extend the categories for each one found in the raw data
-				lCategories.extend([ PostCategory({
-					'_slug': dLocale['slug'],
-					'_category': s
-				}) for s in oRaw['categories'] ])
+				# If we have categories
+				if oRaw['categories']:
+
+					# Extend the set for each one found in the raw data
+					lCategories.extend([ PostCategory({
+						'_slug': dLocale['slug'],
+						'_category': s
+					}) for s in oRaw['categories'] ])
+
+					# Add them to the locale for regenerating
+					try:
+						dLocalesTags[sLocale].update(oRaw['categories'])
+					except KeyError:
+						dLocalesTags[sLocale] = set(oRaw['categories'])
 
 				# If we have tags in this post
 				if dLocale['tags']:
 
 					# Extend the tags for each one found in the raw data
 					lTags.extend([ PostTag({
 						'_slug': dLocale['slug'],
@@ -1541,15 +1568,16 @@
 		# If we have any to update
 		if lUpdate:
 
 			# Go through each post to update
 			for dPost, dLocale in lUpdate:
 
 				# Remove the categories and tags
-				lCategories = dPost.pop('categories').sort()
+				lCategories = dPost.pop('categories')
+				lCategories.sort()
 				lTags = dPost.pop('tags')
 
 				# Create the Post instance
 				oPost = Post(dPost)
 
 				# Go through each field and update it
 				for k in [ 'title', 'content', 'meta' ]:
@@ -1570,28 +1598,42 @@
 
 					# Something changed
 					bChanges = True
 
 					# Delete the existing ones
 					PostCategory.delete_get(dPost['_slug'], index = '_slug')
 
+					# Add the deleted tags to the locale for regenerating
+					try:
+						dLocalesCategories[oPost['_locale']].update(lCategories)
+					except KeyError:
+						dLocalesCategories[oPost['_locale']] = set(lCategories)
+
 					# And add the new ones (if there are any)
 					lNewCats = [ PostCategory({
 						'_slug': dPost['_slug'],
 						'_category': s
 					}) for s in oRaw['categories'] ]
 					if lNewCats:
+
+						# Insert the new categories
 						PostCategory.create_many(lNewCats)
 
+						# Add the new categories to the locale for regenerating
+						try:
+							dLocalesCategories[oPost['_locale']].update(
+								oRaw['categories']
+							)
+						except KeyError:
+							dLocalesCategories[oPost['_locale']] = \
+								set(oRaw['categories'])
+
 				# If the tags have changed
 				if lTags != dLocale['tags']:
 
-					print('lTags: %s' % lTags)
-					print('dLocale[\'tags\']: %s' % dLocale['tags'])
-
 					# Something changed
 					bChanges = True
 
 					# Delete the existing ones
 					PostTag.delete_get(dPost['_slug'], index = '_slug')
 
 					# Add the deleted tags to the locale for regenerating
@@ -1632,14 +1674,32 @@
 		for sLocale in lsTagLocales:
 			PostTag.all_locale_cache_generate(sLocale)
 
 		# Go through each locale and regenerate the posts
 		for sLocale in lsPostsLocales:
 			Post.locale_cache_generate(sLocale)
 
+		# Go through each locale and category and regenerate the corresponding
+		#	slugs
+		for sLocale in dLocalesCategories:
+
+			# Fetch the slugs for the given categories
+			dCatSlugs = {
+				d['_category']: d['slug'] for d in CategoryLocale.filter({
+					'_category': list(dLocalesCategories[sLocale]),
+					'_locale': sLocale
+				}, raw = [ '_category', 'slug' ])
+			}
+
+			# Regenerate the corresponding slugs
+			for sCategoryID in dLocalesCategories[sLocale]:
+				PostCategory.cache_generate(
+					dCatSlugs[sCategoryID]
+				)
+
 		# Go through each locale and tag and regenerate the corresponding slugs
 		for sLocale in dLocalesTags:
 			for sTag in dLocalesTags[sLocale]:
 				PostTag.locale_cache_generate(sTag, sLocale)
 
 		# If anything got added, removed, or updated
 		if bChanges:
@@ -1856,16 +1916,14 @@
 				'_created': d['_created'],
 				'_updated': d['_updated'],
 				'locales': {
 					d['_locale']: { 'title': d['title']}
 				}
 			}
 
-		print(dRaw)
-
 		# Return the values in the raw
 		return Response(
 			list(dRaw.values())
 		)
 
 	def category_read(self, req: dict) -> Response:
 		"""Category read
@@ -1876,45 +1934,72 @@
 			req (dict): The request details, which can include 'data', \
 				'environment', and 'session'
 
 		Returns:
 			Services.Response
 		"""
 
-		# If the slug is not passed
-		if 'slug' not in req['data']:
-			return Error(errors.DATA_FIELDS, [ [ 'slug', 'missing' ] ])
-
-		# Find the category by slug
-		dCategory = CategoryLocale.filter({
-			'slug': req['data']['slug']
-		}, raw = ['_category', '_locale', 'title', 'description' ], limit = 1)
+		# Init errors
+		lErrors = []
+
+		# If the locale or tag is missing is missing
+		try: evaluate(req['data'], [ 'locale', 'slug' ])
+		except ValueError as e:
+			lErrors.extend([ [ s, 'missing' ] for s in e.args ])
+
+		# If the page is missing
+		if 'page' not in req['data']:
+			iPage = 1
 
-		# If it doesn't exist, 404
-		if not dCategory:
-			return Error(
-				errors.DB_NO_RECORD, [ req['data']['slug'], 'category_locale' ]
-			)
+		# Else, we got a page
+		else:
 
-		# Find the other locale slugs and add them to the category
-		dCategory['locales'] = {
-			d['_locale']: d['slug'] \
-			for d in CategoryLocale.filter({
-				'_category': dCategory['_category'],
-				'_locale': { 'neq': dCategory['_locale'] }
-			}, raw = [ '_locale', 'slug' ]) }
-
-		# Get all the associated posts and add them to the category
-		dCategory['posts'] = Post.by_category(
-			dCategory['_locale'],
-			dCategory['_category']
+			# Try to convert it
+			try:
+				iPage = int(req['data']['page'])
+			except ValueError as e:
+				lErrors.append([ 'page', 'invalid' ])
+
+			# If it's less than 1, reject it
+			if iPage < 1:
+				lErrors.append([ 'page', 'invalid' ])
+
+		# If the count is missing
+		if 'count' not in req['data']:
+			iCount = 10
+
+		# Else, we got a count
+		else:
+
+			# Try to convert it
+			try: iCount = int(req['data']['count'])
+			except ValueError as e:
+				lErrors.append([ 'count', 'invalid' ])
+
+			# If it's less than 1, reject it
+			if iPage < 1:
+				lErrors.append([ 'count', 'invalid' ])
+
+		# If there's any errors
+		if lErrors:
+			return Error(errors.DATA_FIELDS, lErrors)
+
+		# Fetch the associated posts from the cache
+		dPosts = PostCategory.cache_fetch(
+			req['data']['slug'],
+			iPage - 1,
+			iCount
 		)
 
-		# Return the category
-		return Response(dCategory)
+		# If shortened data is requested
+		if 'shorten' in req['data'] and req['data']['shorten']:
+			self._shorten(dPosts['posts'], req['data']['shorten'])
+
+		# Return the posts and total count
+		return Response(dPosts)
 
 	def post_read(self, req: dict) -> Response:
 		"""Post read
 
 		Finds the post by slug, then returns all related info
 
 		Arguments:
```

### Comparing `blog-oc-0.1.4/blog_oc.egg-info/PKG-INFO` & `blog-oc-0.2.0/blog_oc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blog-oc
-Version: 0.1.4
+Version: 0.2.0
 Summary: Blog contains a service to manage blog posts and comments associated
 Home-page: https://ouroboroscoding.com/body/blog
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: Custom
 Project-URL: Documentation, https://ouroboroscoding.com/body/blog
 Project-URL: Source, https://github.com/ouroboroscoding/blog
```

### Comparing `blog-oc-0.1.4/blog_oc.egg-info/SOURCES.txt` & `blog-oc-0.2.0/blog_oc.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 blog/__main__.py
 blog/errors.py
 blog/install.py
 blog/records.py
 blog/rest.py
 blog/seo.py
 blog/service.py
+blog/sitemap.py
 blog/definitions/category.json
 blog/definitions/category_locale.json
 blog/definitions/comment.json
 blog/definitions/media.json
 blog/definitions/post.json
 blog/definitions/post_category.json
 blog/definitions/post_raw.json
```

### Comparing `blog-oc-0.1.4/setup.py` & `blog-oc-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as oF:
 	long_description=oF.read()
 
 setup(
 	name='blog-oc',
-	version='0.1.4',
+	version='0.2.0',
 	description='Blog contains a service to manage blog posts and comments associated',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://ouroboroscoding.com/body/blog',
 	project_urls={
 		'Documentation': 'https://ouroboroscoding.com/body/blog',
 		'Source': 'https://github.com/ouroboroscoding/blog',
```

