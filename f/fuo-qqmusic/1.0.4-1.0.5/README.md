# Comparing `tmp/fuo_qqmusic-1.0.4.tar.gz` & `tmp/fuo_qqmusic-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo_qqmusic-1.0.4.tar", last modified: Tue May 21 15:48:01 2024, max compression
+gzip compressed data, was "fuo_qqmusic-1.0.5.tar", last modified: Mon Jun  3 13:36:30 2024, max compression
```

## Comparing `fuo_qqmusic-1.0.4.tar` & `fuo_qqmusic-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:48:01.814260 fuo_qqmusic-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-21 15:48:01.814260 fuo_qqmusic-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:48:01.810260 fuo_qqmusic-1.0.4/fuo_qqmusic/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23472 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:48:01.814260 fuo_qqmusic-1.0.4/fuo_qqmusic/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/excs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/provider_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/fuo_qqmusic/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:48:01.814260 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 15:48:01.000000 fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:48:01.814260 fuo_qqmusic-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 15:48:00.000000 fuo_qqmusic-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:36:30.792009 fuo_qqmusic-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-03 13:36:30.792009 fuo_qqmusic-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-06-03 13:36:22.000000 fuo_qqmusic-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:36:30.792009 fuo_qqmusic-1.0.5/fuo_qqmusic/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-03 13:36:22.000000 fuo_qqmusic-1.0.5/fuo_qqmusic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23597 2024-06-03 13:36:22.000000 fuo_qqmusic-1.0.5/fuo_qqmusic/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:36:30.792009 fuo_qqmusic-1.0.5/fuo_qqmusic/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-06-03 13:36:22.000000 fuo_qqmusic-1.0.5/fuo_qqmusic/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-06-03 13:36:22.000000 fuo_qqmusic-1.0.5/fuo_qqmusic/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-03 13:36:22.000000 fuo_qqmusic-1.0.5/fuo_qqmusic/excs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15724 2024-06-03 13:36:22.000000 fuo_qqmusic-1.0.5/fuo_qqmusic/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-06-03 13:36:22.000000 fuo_qqmusic-1.0.5/fuo_qqmusic/provider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12128 2024-06-03 13:36:22.000000 fuo_qqmusic-1.0.5/fuo_qqmusic/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:36:30.792009 fuo_qqmusic-1.0.5/fuo_qqmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-03 13:36:30.000000 fuo_qqmusic-1.0.5/fuo_qqmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-06-03 13:36:30.000000 fuo_qqmusic-1.0.5/fuo_qqmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:36:30.000000 fuo_qqmusic-1.0.5/fuo_qqmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-03 13:36:30.000000 fuo_qqmusic-1.0.5/fuo_qqmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-03 13:36:30.000000 fuo_qqmusic-1.0.5/fuo_qqmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 13:36:30.000000 fuo_qqmusic-1.0.5/fuo_qqmusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:36:30.792009 fuo_qqmusic-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-06-03 13:36:22.000000 fuo_qqmusic-1.0.5/setup.py
```

### Comparing `fuo_qqmusic-1.0.4/PKG-INFO` & `fuo_qqmusic-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo_qqmusic
-Version: 1.0.4
+Version: 1.0.5
 Summary: feeluown qqmusic plugin
 Home-page: https://github.com/feeluown/feeluown-qqmusic
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 Keywords: feeluown,plugin,qqmusic
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `fuo_qqmusic-1.0.4/README.md` & `fuo_qqmusic-1.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 ## 使用说明
 
 ### 登录
 在网页登录微信/QQ后（在任意网站），复制请求中的 cookies 至程序登录框，
 [操作示例](https://github.com/feeluown/feeluown-qqmusic/issues/6)。
 
 ## changelog
+### 1.0.5 (2024-06-03)
+- 修复搜索接口，支持搜索歌单、视频、专辑
+- 支持提供歌单的播放次数
+
 ### 1.0.4 (2024-05-21)
 - 歌手歌曲排序切换为”按热度排序”
 - 修复推荐歌单接口
 
 ### 1.0.3 (2024-04-21)
 - 适配 feeluown 4.1.3 的新主页功能
```

### Comparing `fuo_qqmusic-1.0.4/fuo_qqmusic/__init__.py` & `fuo_qqmusic-1.0.5/fuo_qqmusic/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-1.0.4/fuo_qqmusic/api.py` & `fuo_qqmusic-1.0.5/fuo_qqmusic/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,18 +120,22 @@
         return 'http://y.gtimg.cn/music/photo_new/T00{}R800x800M000{}.jpg' \
             .format(type_, mid)
 
     def search(self, keyword, type_=0, limit=20, page=1):
         # Other supported types: songlist, user, mv, qc, gedantip, zhida.
         if type_ == 0:
             key_ = 'song'
-        elif type_ == 8:
-            key_ = 'album'
-        elif type_ == 9:
+        elif type_ == 1:
             key_ = 'singer'
+        elif type_ == 2:
+            key_ = 'album'
+        elif type_ == 3:
+            key_ = 'songlist'  # playlist
+        elif type_ == 4:
+            key_ = 'mv'  # video
         else:
             raise QQIOError('invalid search type_:%d', type_)
         payload = {
             "search": {
                 "method": "DoSearchForQQMusicDesktop",
                 "module": "music.search.SearchCgiService",
                 "param": {
```

### Comparing `fuo_qqmusic-1.0.4/fuo_qqmusic/assets/icon.svg` & `fuo_qqmusic-1.0.5/fuo_qqmusic/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-1.0.4/fuo_qqmusic/provider.py` & `fuo_qqmusic-1.0.5/fuo_qqmusic/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     SupportsSongMV,
     VideoModel,
     LyricModel,
     SupportsCurrentUser,
     SupportsVideoGet,
     SupportsSongLyric,
     SupportsAlbumGet,
+    SupportsAlbumSongsReader,
     SupportsArtistGet,
     SupportsPlaylistGet,
     SupportsPlaylistSongsReader,
     SupportsRecACollectionOfSongs,
     SimpleSearchResult,
     SearchType,
     ModelType,
@@ -44,14 +45,15 @@
     SupportsVideoGet,
     SupportsSongLyric,
     SupportsAlbumGet,
     SupportsArtistGet,
     SupportsPlaylistGet,
     SupportsPlaylistSongsReader,
     SupportsRecACollectionOfSongs,
+    SupportsAlbumSongsReader,
     Protocol,
 ):
     pass
 
 
 class QQProvider(AbstractProvider, ProviderV2):
     class meta:
@@ -220,14 +222,18 @@
     def album_get(self, identifier):
         data_album = self.api.album_detail(int(identifier))
         if data_album is None:
             raise ModelNotFound
         album = _deserialize(data_album, QQAlbumSchema)
         return album
 
+    def album_create_songs_rd(self, album):
+        album = self.album_get(album.identifier)
+        return create_reader(album.songs)
+
     def user_get(self, identifier):
         data = self.api.user_detail(identifier)
         data["creator"]["fav_pid"] = data["mymusic"][0]["id"]
         # 假设使用微信登陆，从网页拿到 cookie，cookie 里面的 uin 是正确的，
         # 而这个接口返回的 uin 则可能是 0，因此手动重置一下。
         data["creator"]["uin"] = identifier
         return _deserialize(data, QQUserSchema)
@@ -270,15 +276,16 @@
                 print(card['title'], card['jumptype'])
                 if card['jumptype'] == 10014:  # 10014->playlist
                     playlists.append(
                         PlaylistModel(identifier=str(card['id']),
                                       source=SOURCE,
                                       name=card['title'],
                                       cover=card['cover'],
-                                      description=card['miscellany']['rcmdtemplate'])
+                                      description=card['miscellany']['rcmdtemplate'],
+                                      play_count=card['cnt'])
                     )
         return playlists
 
     def rec_a_collection_of_songs(self):
         # TODO: cache API result
         feed = self.api.get_recommend_feed()
         shelf = None
@@ -390,46 +397,52 @@
                 data = func(identifier, page)
 
     return SequentialReader(g(), total)
 
 
 def search(keyword, **kwargs):
     type_ = SearchType.parse(kwargs["type_"])
-    if type_ == SearchType.pl:
-        data = provider.api.search_playlists(keyword)
-        playlists = [_deserialize(playlist, _BriefPlaylistSchema) for playlist in data]
+    type_type_map = {
+        SearchType.so: 0,
+        SearchType.ar: 1,
+        SearchType.al: 2,
+        SearchType.pl: 3,
+        SearchType.vi: 4,
+    }
+    data = provider.api.search(keyword, type_=type_type_map[type_])
+    if type_ == SearchType.so:
+        songs = [_deserialize(song, QQSongSchema) for song in data]
+        return SimpleSearchResult(q=keyword, songs=songs)
+    if type_ == SearchType.ar:
+        artists = [_deserialize(artist, SearchArtistSchema) for artist in data]
+        return SimpleSearchResult(q=keyword, artists=artists)
+    elif type_ == SearchType.al:
+        albums = [_deserialize(album, SearchAlbumSchema) for album in data]
+        return SimpleSearchResult(q=keyword, albums=albums)
+    elif type_ == SearchType.pl:
+        playlists = [_deserialize(playlist, SearchPlaylistSchema) for playlist in data]
         return SimpleSearchResult(q=keyword, playlists=playlists)
-    else:
-        type_type_map = {
-            SearchType.so: 0,
-            SearchType.al: 8,
-            SearchType.ar: 9,
-        }
-        data = provider.api.search(keyword, type_=type_type_map[type_])
-        if type_ == SearchType.so:
-            songs = [_deserialize(song, QQSongSchema) for song in data]
-            return SimpleSearchResult(q=keyword, songs=songs)
-        elif type_ == SearchType.al:
-            albums = [_deserialize(album, _BriefAlbumSchema) for album in data]
-            return SimpleSearchResult(q=keyword, albums=albums)
-        else:
-            artists = [_deserialize(artist, _BriefArtistSchema) for artist in data]
-            return SimpleSearchResult(q=keyword, artists=artists)
+    elif type_ == SearchType.vi:
+        models = [_deserialize(model, SearchMVSchema) for model in data]
+        return SimpleSearchResult(q=keyword, videos=models)
 
 
 provider = QQProvider()
 provider.search = search
 
 
 from .schemas import (  # noqa
     QQSongSchema,
     QQArtistSchema,
     _ArtistSongSchema,
     _BriefAlbumSchema,
     _UserArtistSchema,
     _BriefArtistSchema,
-    _BriefPlaylistSchema,
     QQAlbumSchema,
     QQPlaylistSchema,
     QQUserSchema,
     _UserAlbumSchema,
+    SearchAlbumSchema,
+    SearchArtistSchema,
+    SearchPlaylistSchema,
+    SearchMVSchema,
 )  # noqa
```

### Comparing `fuo_qqmusic-1.0.4/fuo_qqmusic/provider_ui.py` & `fuo_qqmusic-1.0.5/fuo_qqmusic/provider_ui.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-1.0.4/fuo_qqmusic/schemas.py` & `fuo_qqmusic-1.0.5/fuo_qqmusic/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     BriefAlbumModel,
     BriefArtistModel,
     ArtistModel,
     AlbumModel,
     PlaylistModel,
     BriefPlaylistModel,
     UserModel,
+    VideoModel,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class BaseSchema(Schema):
     source = fields.Str(missing="qqmusic")
@@ -139,35 +140,81 @@
     name = fields.Str(data_key="singerName", required=True)
 
     @post_load
     def create_model(self, data, **kwargs):
         return create_model(BriefArtistModel, data, ["mid"])
 
 
+class SearchArtistSchema(_BriefArtistSchema):
+    pic_url = fields.Str(data_key="singerPic", required=True)
+
+    @post_load
+    def create_model(self, data, **kwargs):
+        data['hot_songs'] = []
+        data['description'] = ''
+        data['aliases'] = []
+        return create_model(ArtistModel, data, ["mid"])
+
+
 class _BriefAlbumSchema(Schema):
     identifier = fields.Int(data_key="albumID", required=True)
     mid = fields.Str(data_key="albumMID", required=True)
     name = fields.Str(data_key="albumName", required=True)
 
     @post_load
     def create_model(self, data, **kwargs):
         return create_model(BriefAlbumModel, data, ["mid"])
 
 
+class SearchAlbumSchema(_BriefAlbumSchema):
+    cover = fields.Str(data_key="albumPic", required=True)
+    released = fields.Str(data_key="publicTime", required=True)
+    song_count = fields.Int(required=True)
+    artists = fields.List(fields.Nested(_SongArtistSchema),
+                          data_key="singer_list",
+                          required=True)
+    @post_load
+    def create_model(self, data, **kwargs):
+        data['description'] = ''
+        data['songs'] = []
+        return create_model(AlbumModel, data, ['mid'])
+
+
 class _BriefPlaylistSchema(Schema):
     identifier = fields.Int(data_key="dissid", required=True)
     name = fields.Str(data_key="dissname", required=True)
     cover = fields.Str(data_key="imgurl", required=True)
 
     @post_load
     def create_model(self, data, **kwargs):
         data['description'] = ''
         return create_model(PlaylistModel, **data)
 
 
+class PlaylistUserSchema(Schema):
+    identifier = fields.Str(data_key="creator_uin", required=True)
+    mid = fields.Str(data_key="encrypt_uin", required=True)
+    name = fields.Str(required=True)
+    avatar_url = fields.Str(required=True, data_key="avatarUrl")
+
+    @post_load
+    def create_model(self, data, **kwargs):
+        return create_model(UserModel, data, ['mid'])
+
+
+class SearchPlaylistSchema(_BriefPlaylistSchema):
+    creator = fields.Nested("PlaylistUserSchema", required=True)
+    description = fields.Str(data_key="introduction", required=True)
+    play_count = fields.Int(data_key="listennum", required=True)
+
+    @post_load
+    def create_model(self, data, **kwargs):
+        return create_model(PlaylistModel, data)
+
+
 class QQArtistSchema(Schema):
     """歌手详情 Schema、歌曲歌手简要信息 Schema"""
 
     identifier = fields.Int(data_key="singer_id", required=True)
     mid = fields.Str(data_key="singer_mid", required=True)
     name = fields.Str(data_key="singer_name", required=True)
 
@@ -290,7 +337,23 @@
             mid=creator["encrypt_uin"],
             name=creator["nick"],
             fav_pid=creator["fav_pid"],
             avatar_url=creator["headpic"],
             playlists=playlists,
         )
         return create_model(UserModel, data, ['mid', 'fav_pid', 'playlists'])
+
+
+class SearchMVSchema(Schema):
+    # 使用 mv_id 字段的话，目前拿不到播放 url，用 v_id  比较合适
+    identifier = fields.Str(data_key="v_id", required=True)
+    title = fields.Str(data_key="mv_name", required=True)
+    artists = fields.List(fields.Nested("_SongArtistSchema"),
+                          data_key="singer_list",
+                          required=True)
+    duration = fields.Int(required=True)
+    cover = fields.Str(data_key="mv_pic_url", required=True)
+    play_count = fields.Int(required=True)
+
+    @post_load
+    def create_model(self, data, **kwargs):
+        return create_model(VideoModel, data)
```

### Comparing `fuo_qqmusic-1.0.4/fuo_qqmusic.egg-info/PKG-INFO` & `fuo_qqmusic-1.0.5/fuo_qqmusic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo-qqmusic
-Version: 1.0.4
+Version: 1.0.5
 Summary: feeluown qqmusic plugin
 Home-page: https://github.com/feeluown/feeluown-qqmusic
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 Keywords: feeluown,plugin,qqmusic
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `fuo_qqmusic-1.0.4/setup.py` & `fuo_qqmusic-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup
 
 
 setup(
     name='fuo_qqmusic',
-    version='1.0.4',
+    version='1.0.5',
     description='feeluown qqmusic plugin',
     author='Cosven',
     author_email='yinshaowen241@gmail.com',
     packages=[
         'fuo_qqmusic',
     ],
     package_data={
```

