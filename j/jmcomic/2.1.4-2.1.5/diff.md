# Comparing `tmp/jmcomic-2.1.4.tar.gz` & `tmp/jmcomic-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.1.4.tar", last modified: Wed Jul 19 12:54:24 2023, max compression
+gzip compressed data, was "jmcomic-2.1.5.tar", last modified: Wed Jul 26 09:44:12 2023, max compression
```

## Comparing `jmcomic-2.1.4.tar` & `jmcomic-2.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:54:24.424531 jmcomic-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-19 12:54:14.000000 jmcomic-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-19 12:54:24.424531 jmcomic-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-19 12:54:14.000000 jmcomic-2.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:54:24.424531 jmcomic-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-19 12:54:14.000000 jmcomic-2.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:54:24.420531 jmcomic-2.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:54:24.420531 jmcomic-2.1.4/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:54:24.424531 jmcomic-2.1.4/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-19 12:54:24.000000 jmcomic-2.1.4/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-19 12:54:24.000000 jmcomic-2.1.4/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:54:24.000000 jmcomic-2.1.4/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-19 12:54:24.000000 jmcomic-2.1.4/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 12:54:24.000000 jmcomic-2.1.4/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:44:12.644325 jmcomic-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 09:44:01.000000 jmcomic-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-26 09:44:12.644325 jmcomic-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-26 09:44:01.000000 jmcomic-2.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:44:12.644325 jmcomic-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-26 09:44:01.000000 jmcomic-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:44:12.640325 jmcomic-2.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:44:12.644325 jmcomic-2.1.5/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:44:12.644325 jmcomic-2.1.5/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-26 09:44:12.000000 jmcomic-2.1.5/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-26 09:44:12.000000 jmcomic-2.1.5/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:44:12.000000 jmcomic-2.1.5/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 09:44:12.000000 jmcomic-2.1.5/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 09:44:12.000000 jmcomic-2.1.5/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.1.4/LICENSE` & `jmcomic-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.4/PKG-INFO` & `jmcomic-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.4
+Version: 2.1.5
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.1.4/README.md` & `jmcomic-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.4/setup.py` & `jmcomic-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.4/src/jmcomic/api.py` & `jmcomic-2.1.5/src/jmcomic/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,126 +11,111 @@
 
     if not isinstance(jm_album_id, (str, int)):
         return download_album_batch(jm_album_id, option)
 
     option, jm_client = build_client(option)
     album: JmAlbumDetail = jm_client.get_album_detail(jm_album_id)
 
-    jm_debug('album',
-             f'本子获取成功: [{album.id}], '
-             f'作者: [{album.author}], '
-             f'章节数: [{len(album)}], '
-             f'标题: [{album.title}], '
-             )
-
-    def download_photo(photo: JmPhotoDetail,
-                       debug_topic='photo',
-                       ):
-        jm_client.check_photo(photo)
-
-        jm_debug(debug_topic,
-                 f'开始下载章节: {photo.id} ({photo.album_id}[{photo.index}/{len(album)}]), '
-                 f'标题: [{photo.title}], '
-                 f'图片数为[{len(photo)}]'
-                 )
-
-        download_by_photo_detail(photo, option)
-
-        jm_debug(debug_topic,
-                 f'章节下载完成: {photo.id} ({photo.album_id}[{photo.index}/{len(album)}])'
-                 )
-
-    thread_pool_executor(
-        iter_objs=album,
-        apply_each_obj_func=download_photo,
-    )
-
-    jm_debug('album', f'本子下载完成: [{album.id}]')
-
-
-def download_album_batch(jm_album_id_iter: Union[Iterable, Generator],
-                         option=None,
-                         wait_finish=True,
-                         ) -> List[Thread]:
-    """
-    批量下载album，每个album一个线程，使用的是同一个option。
-
-    @param jm_album_id_iter: album_id的可迭代对象
-    @param option: 下载选项，为空默认是 JmOption.default()
-    @param wait_finish: 是否要等待这些下载线程全部完成
-    @return 返回值是List[Thread]，里面是每个下载漫画的线程。
-    """
-    if option is None:
-        option = JmOption.default()
-
-    return thread_pool_executor(
-        iter_objs=((album_id, option) for album_id in jm_album_id_iter),
-        apply_each_obj_func=download_album,
-        wait_finish=wait_finish,
+    option.before_album(album)
+    execute_by_condition(
+        iter_obj=album,
+        apply=lambda photo: download_by_photo_detail(photo, option),
+        count_batch=option.decide_photo_batch_count(album)
     )
+    option.after_album(album)
 
 
 def download_photo(jm_photo_id, option=None):
     """
     下载一个本子的一章，入口api
     """
     option, jm_client = build_client(option)
-    photo_detail = jm_client.get_photo_detail(jm_photo_id)
-    download_by_photo_detail(photo_detail, option)
+    photo = jm_client.get_photo_detail(jm_photo_id)
+    download_by_photo_detail(photo, option)
 
 
-def download_by_photo_detail(photo_detail: JmPhotoDetail,
-                             option=None,
-                             ):
+def download_by_photo_detail(photo: JmPhotoDetail, option=None):
     """
-    下载一个本子的一章，根据 photo_detail
-    @param photo_detail: 本子章节信息
+    下载一个本子的一章，根据 photo
+    @param photo: 本子章节信息
     @param option: 选项
     """
     option, jm_client = build_client(option)
 
     # 下载准备
     use_cache = option.download_cache
     decode_image = option.download_image_decode
-    jm_client.check_photo(photo_detail)
+    jm_client.check_photo(photo)
 
     # 下载每个图片的函数
-    def download_image(index, image: JmImageDetail, debug_topic='image'):
-        img_save_path = option.decide_image_filepath(photo_detail, index)
-        debug_tag = f'{image.aid}/{image.filename} [{index + 1}/{len(photo_detail)}]'
+    def download_image(image: JmImageDetail):
+        img_save_path = option.decide_image_filepath(image)
 
         # 已下载过，缓存命中
         if use_cache is True and file_exists(img_save_path):
-            jm_debug(debug_topic,
-                     f'图片已存在: {debug_tag} ← [{img_save_path}]'
-                     )
+            image.is_exists = True
             return
 
-        # 开始下载
+        option.before_image(image, img_save_path)
         jm_client.download_by_image_detail(
             image,
             img_save_path,
             decode_image=decode_image,
         )
+        option.after_image(image, img_save_path)
+
+    option.before_photo(photo)
+    execute_by_condition(
+        iter_obj=photo,
+        apply=download_image,
+        count_batch=option.decide_image_batch_count(photo)
+    )
+    option.before_photo(photo)
 
-        jm_debug(debug_topic,
-                 f'图片下载完成: {debug_tag}, [{image.img_url}] → [{img_save_path}]'
-                 )
 
-    batch = option.download_threading_batch_count
-    if batch <= 0:
+def download_album_batch(jm_album_id_iter: Union[Iterable, Generator],
+                         option=None,
+                         wait_finish=True,
+                         ) -> List[Thread]:
+    """
+    批量下载album，每个album一个线程，使用的是同一个option。
+
+    @param jm_album_id_iter: album_id的可迭代对象
+    @param option: 下载选项，为空默认是 JmOption.default()
+    @param wait_finish: 是否要等待这些下载线程全部完成
+    @return 返回值是List[Thread]，里面是每个下载漫画的线程。
+    """
+    if option is None:
+        option = JmOption.default()
+
+    return thread_pool_executor(
+        iter_objs=((album_id, option) for album_id in jm_album_id_iter),
+        apply_each_obj_func=download_album,
+        wait_finish=wait_finish,
+    )
+
+
+def execute_by_condition(iter_obj, apply: Callable, count_batch: int):
+    """
+    章节/图片的下载调度逻辑
+    """
+    count_real = len(iter_obj)
+
+    if count_batch >= count_real:
+        # 一图一线程
         multi_thread_launcher(
-            iter_objs=enumerate(photo_detail),
-            apply_each_obj_func=download_image,
+            iter_objs=iter_obj,
+            apply_each_obj_func=apply,
         )
     else:
+        # 创建batch个线程的线程池，当图片数>batch时要等待。
         thread_pool_executor(
-            iter_objs=enumerate(photo_detail),
-            apply_each_obj_func=download_image,
-            max_workers=batch,
+            iter_objs=iter_obj,
+            apply_each_obj_func=apply,
+            max_workers=count_batch,
         )
 
 
 def build_client(option: Optional[JmOption]) -> Tuple[JmOption, JmcomicClient]:
     """
     处理option的判空，并且创建jm_client
     """
```

### Comparing `jmcomic-2.1.4/src/jmcomic/jm_client_impl.py` & `jmcomic-2.1.5/src/jmcomic/jm_client_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def get(self, url, **kwargs):
         return self.request_with_retry(self.postman.get, url, **kwargs)
 
     def post(self, url, **kwargs):
         return self.request_with_retry(self.postman.post, url, **kwargs)
 
     def of_api_url(self, api_path, domain):
-        return f'{JmModuleConfig.PROT}{domain}{api_path}'
+        return JmcomicText.format_url(api_path, domain)
 
     def request_with_retry(self,
                            request,
                            url,
                            domain_index=0,
                            retry_count=0,
                            **kwargs,
@@ -48,17 +48,19 @@
         @param retry_count: 重试次数
         @param kwargs: 请求方法的kwargs
         """
         if domain_index >= len(self.domain_list):
             self.fallback(request, url, domain_index, retry_count, **kwargs)
 
         if url.startswith('/'):
-            # path
-            domain = self.domain_list[domain_index]
-            url = self.of_api_url(url, domain)
+            # path → url
+            url = self.of_api_url(
+                api_path=url,
+                domain=self.domain_list[domain_index],
+            )
             jm_debug('api', url)
         else:
             # 图片url
             pass
 
         if domain_index != 0 or retry_count != 0:
             jm_debug(
@@ -150,21 +152,21 @@
         # 参数校验
         photo_id = JmcomicText.parse_to_photo_id(photo_id)
 
         # 请求
         resp = self.get_jm_html(f"/photo/{photo_id}")
 
         # 用 JmcomicText 解析 html，返回实体类
-        photo_detail = JmcomicText.analyse_jm_photo_html(resp.text)
+        photo = JmcomicText.analyse_jm_photo_html(resp.text)
 
         # 一并获取该章节的所处本子
         if fetch_album is True:
-            photo_detail.from_album = self.get_album_detail(photo_detail.album_id)
+            photo.from_album = self.get_album_detail(photo.album_id)
 
-        return photo_detail
+        return photo
 
     def search_album(self, search_query, main_tag=0, page=1) -> JmSearchPage:
         params = {
             'main_tag': main_tag,
             'search_query': search_query,
             'page': page,
         }
```

### Comparing `jmcomic-2.1.4/src/jmcomic/jm_client_interface.py` & `jmcomic-2.1.5/src/jmcomic/jm_client_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -156,24 +156,36 @@
 
     def of_api_url(self, api_path, domain):
         raise NotImplementedError
 
     def enable_cache(self, debug=False):
         raise NotImplementedError
 
-    def check_photo(self, photo_detail: JmPhotoDetail):
+    def check_photo(self, photo: JmPhotoDetail):
+        """
+        photo来源有两种:
+        1. album[?]
+        2. client.get_photo_detail(?)
+
+        其中，只有[2]是可以包含下载图片的url信息的。
+        本方法会检查photo是不是[1]，
+        如果是[1]，通过请求获取[2]，然后把2中的一些重要字段更新到1中
+
+        @param photo: 被检查的JmPhotoDetail对象
+        """
         # 检查 from_album
-        if photo_detail.from_album is None:
-            photo_detail.from_album = self.get_album_detail(photo_detail.album_id)
+        if photo.from_album is None:
+            photo.from_album = self.get_album_detail(photo.album_id)
 
         # 检查 page_arr 和 data_original_domain
-        if photo_detail.page_arr is None or photo_detail.data_original_domain is None:
-            new = self.get_photo_detail(photo_detail.photo_id, False)
-            new.from_album = photo_detail.from_album
-            photo_detail.__dict__.update(new.__dict__)
+        if photo.page_arr is None or photo.data_original_domain is None:
+            new = self.get_photo_detail(photo.photo_id, False)
+            new.from_album = photo.from_album
+            photo.__dict__.update(new.__dict__)
+
 
 class JmUserClient:
 
     def login(self,
               username,
               password,
               refresh_client_cookies=True,
@@ -228,22 +240,22 @@
 
         if self.img_is_not_need_to_decode(img_url, resp):
             JmImageSupport.save_resp_img(resp, img_save_path, False)
         else:
             resp.transfer_to(img_save_path, scramble_id, decode_image, img_url)
 
     def download_by_image_detail(self,
-                                 img_detail: JmImageDetail,
+                                 image: JmImageDetail,
                                  img_save_path,
                                  decode_image=True,
                                  ):
         self.download_image(
-            img_detail.download_url,
+            image.download_url,
             img_save_path,
-            img_detail.scramble_id,
+            image.scramble_id,
             decode_image=decode_image,
         )
 
     def get_jm_image(self, img_url) -> JmImageResp:
         raise NotImplementedError
 
     @classmethod
```

### Comparing `jmcomic-2.1.4/src/jmcomic/jm_config.py` & `jmcomic-2.1.5/src/jmcomic/jm_config.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.4/src/jmcomic/jm_entity.py` & `jmcomic-2.1.5/src/jmcomic/jm_entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,65 +3,64 @@
 from .jm_config import *
 
 
 class JmBaseEntity:
     pass
 
 
-class WorkEntity(JmBaseEntity, SaveableEntity, IterableEntity):
-    when_del_save_file = False
-    after_save_print_info = True
-    attr_char = '_'
-
-    cache_getitem_result = True
-    cache_field_name = '__cache_items_dict__'
-    detail_save_base_dir = workspace()
-    detail_save_file_suffix = '.yml'
-
-    def save_base_dir(self):
-        return self.detail_save_base_dir
-
-    def save_file_name(self) -> str:
-        def jm_type():
-            # "JmAlbumDetail" -> "album"
-            cls_name = self.__class__.__name__
-            return cls_name[cls_name.index("m") + 1: cls_name.rfind("Detail")].lower()
-
-        return '[{}]{}{}'.format(jm_type(), self.id, self.detail_save_file_suffix)
+class DetailEntity(JmBaseEntity, IterableEntity):
 
     @property
     def id(self) -> str:
         raise NotImplementedError
 
-    def __len__(self):
-        raise NotImplementedError
+    @property
+    def name(self) -> str:
+        return getattr(self, 'title')
+
+    def save_to_file(self, filepath):
+        from common import PackerUtil
+        PackerUtil.pack(self, filepath)
+
+    @classmethod
+    def __jm_type__(cls):
+        # "JmAlbumDetail" -> "album" (本子)
+        # "JmPhotoDetail" -> "photo" (章节)
+        cls_name = cls.__name__
+        return cls_name[cls_name.index("m") + 1: cls_name.rfind("Detail")].lower()
 
     def __getitem__(self, item) -> Union['JmAlbumDetail', 'JmPhotoDetail']:
         raise NotImplementedError
 
+    def __str__(self):
+        return f'{self.__class__.__name__}({self.id}-{self.name})'
+
 
 class JmImageDetail(JmBaseEntity):
 
     def __init__(self,
                  aid,
                  scramble_id,
                  img_url,
                  img_file_name,
                  img_file_suffix,
                  from_photo=None,
                  query_params=None,
+                 index=-1,
                  ) -> None:
         self.aid: str = aid
         self.scramble_id: str = scramble_id
         self.img_url: str = img_url
         self.img_file_name: str = img_file_name
         self.img_file_suffix: str = img_file_suffix
 
         self.from_photo: Optional[JmPhotoDetail] = from_photo
         self.query_params: StrNone = query_params
+        self.is_exists: bool = False
+        self.index = index
 
     @property
     def filename(self) -> str:
         return self.img_file_name + self.img_file_suffix
 
     @property
     def download_url(self) -> str:
@@ -78,14 +77,15 @@
     @classmethod
     def of(cls,
            photo_id: str,
            scramble_id: str,
            data_original: str,
            from_photo=None,
            query_params=None,
+           index=-1,
            ) -> 'JmImageDetail':
         """
         该方法用于创建 JmImageDetail 对象
         """
 
         # /xxx.yyy
         # ↑   ↑
@@ -97,18 +97,27 @@
             aid=photo_id,
             scramble_id=scramble_id,
             img_url=data_original,
             img_file_name=data_original[x + 1:y],
             img_file_suffix=data_original[y:],
             from_photo=from_photo,
             query_params=query_params,
+            index=index,
         )
 
+    """
+    below help for debug method 
+    """
+
+    @property
+    def tag(self) -> str:
+        return f'{self.aid}/{self.filename} [{self.index + 1}/{len(self.from_photo)}]'
+
 
-class JmPhotoDetail(WorkEntity):
+class JmPhotoDetail(DetailEntity):
 
     def __init__(self,
                  photo_id,
                  scramble_id,
                  title,
                  keywords,
                  series_id,
@@ -205,14 +214,15 @@
 
         return JmImageDetail.of(
             self.photo_id,
             self.scramble_id,
             data_original,
             from_photo=self,
             query_params=self.data_original_query_params,
+            index=index,
         )
 
     def get_img_data_original(self, img_name: str) -> str:
         """
         根据图片名，生成图片的完整请求路径 URL
         例如：img_name = 01111.webp
         返回：https://cdn-msp2.18comic.org/media/photos/147643/01111.webp
@@ -244,15 +254,15 @@
     def __len__(self):
         return len(self.page_arr)
 
     def __iter__(self) -> Generator[JmImageDetail, Any, None]:
         return super().__iter__()
 
 
-class JmAlbumDetail(WorkEntity):
+class JmAlbumDetail(DetailEntity):
 
     def __init__(self,
                  album_id,
                  scramble_id,
                  title,
                  episode_list,
                  page_count,
@@ -284,28 +294,28 @@
         if index >= length:
             raise AssertionError(f'创建JmPhotoDetail失败，{index} >= {length}')
 
         # episode_info: ('212214', '81', '94 突然打來', '2020-08-29')
         episode_info: tuple = self.episode_list[index]
         photo_id, photo_index_of_album, photo_title, photo_pub_date = episode_info
 
-        photo_detail = JmPhotoDetail(
+        photo = JmPhotoDetail(
             photo_id=photo_id,
             scramble_id=self.scramble_id,
             title=photo_title,
             keywords='',
             series_id=self.album_id,
             sort=episode_info[1] if len(self) != 1 else 1,
             author=self.author,
             from_album=self,
             page_arr=None,
             data_original_domain=None
         )
 
-        return photo_detail, episode_info
+        return photo, episode_info
 
     @property
     def author(self):
         if len(self._author_list) >= 1:
             return self._author_list[0]
         return JmModuleConfig.default_author
 
@@ -340,15 +350,15 @@
 
         return ret
 
     def __iter__(self) -> Generator[JmPhotoDetail, Any, None]:
         return super().__iter__()
 
 
-class JmSearchPage(IterableEntity):
+class JmSearchPage(JmBaseEntity, IterableEntity):
 
     def __init__(self, album_info_list: List[Tuple[str, str, StrNone, StrNone, List[str]]]):
         # (album_id, title, category_none, label_sub_none, tag_list)
         self.album_info_list = album_info_list
 
     def __len__(self):
         return len(self.album_info_list)
```

### Comparing `jmcomic-2.1.4/src/jmcomic/jm_option.py` & `jmcomic-2.1.5/src/jmcomic/jm_option.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,50 @@
 from .jm_client_impl import *
 
 
+# noinspection PyMethodMayBeStatic
+class DownloadCallback:
+
+    def before_album(self, album: JmAlbumDetail):
+        jm_debug('album-before',
+                 f'本子获取成功: [{album.id}], '
+                 f'作者: [{album.author}], '
+                 f'章节数: [{len(album)}], '
+                 f'标题: [{album.title}], '
+                 )
+
+    def after_album(self, album: JmAlbumDetail):
+        jm_debug('album-after', f'本子下载完成: [{album.id}]')
+
+    def before_photo(self, photo: JmPhotoDetail):
+        jm_debug('photo-before',
+                 f'开始下载章节: {photo.id} ({photo.album_id}[{photo.index}/{len(photo.from_album)}]), '
+                 f'标题: [{photo.title}], '
+                 f'图片数为[{len(photo)}]'
+                 )
+
+    def after_photo(self, photo: JmPhotoDetail):
+        jm_debug('photo-after',
+                 f'章节下载完成: {photo.id} ({photo.album_id}[{photo.index}/{len(photo.from_album)}])')
+
+    def before_image(self, image: JmImageDetail, img_save_path):
+        if image.is_exists:
+            jm_debug('image-before',
+                     f'图片已存在: {image.tag} ← [{img_save_path}]'
+                     )
+        else:
+            jm_debug('image_before',
+                     f'图片准备下载: {image.tag}, [{image.img_url}] → [{img_save_path}]'
+                     )
+
+    def after_image(self, image: JmImageDetail, img_save_path):
+        jm_debug('image-after',
+                 f'图片下载完成: {image.tag}, [{image.img_url}] → [{img_save_path}]')
+
+
 class DirRule:
     rule_sample = [
         # 根目录 / Album-id / Photo-序号 /
         'Bd_Aid_Pindex',  # 禁漫网站的默认下载方式
         # 根目录 / Album-作者 / Album-标题 / Photo-序号 /
         'Bd_Aauthor_Atitle_Pindex',
         # 根目录 / Photo-序号&标题 /
@@ -95,15 +135,15 @@
     def parse_dsl(self, base_dir: str):
         for k, func in self.dsl_support.items():
             if k in base_dir:
                 base_dir = base_dir.replace(k, func(base_dir))
         return base_dir
 
 
-class JmOption:
+class JmOption(DownloadCallback):
     JM_OP_VER = '2.0'
 
     def __init__(self,
                  dir_rule: Dict,
                  download: Dict,
                  client: Dict,
                  filepath=None,
@@ -138,37 +178,44 @@
     def download_image_suffix(self):
         return self.download.image.suffix
 
     """
     下面是决定图片保存路径的方法
     """
 
-    def decide_image_save_dir(self, photo_detail) -> str:
+    # noinspection PyUnusedLocal
+    def decide_image_batch_count(self, photo: JmPhotoDetail):
+        return self.download_threading_batch_count
+
+    # noinspection PyMethodMayBeStatic
+    def decide_photo_batch_count(self, album: JmAlbumDetail):
+        return len(album)
+
+    def decide_image_save_dir(self, photo) -> str:
         # 使用 self.dir_rule 决定 save_dir
         save_dir = self.dir_rule.deside_image_save_dir(
-            photo_detail.from_album,
-            photo_detail
+            photo.from_album,
+            photo
         )
 
         mkdir_if_not_exists(save_dir)
         return save_dir
 
-    def decide_image_suffix(self, img_detail: JmImageDetail):
+    def decide_image_suffix(self, image: JmImageDetail):
         # 动图则使用原后缀
-        suffix = img_detail.img_file_suffix
+        suffix = image.img_file_suffix
         if suffix.endswith("gif"):
             return suffix
 
         # 非动图，以配置为先
         return self.download_image_suffix or suffix
 
-    def decide_image_filepath(self, photo_detail: JmPhotoDetail, index: int) -> str:
+    def decide_image_filepath(self, image: JmImageDetail) -> str:
         # 通过拼接生成绝对路径
-        save_dir = self.decide_image_save_dir(photo_detail)
-        image: JmImageDetail = photo_detail[index]
+        save_dir = self.decide_image_save_dir(image.from_photo)
         suffix = self.decide_image_suffix(image)
         return save_dir + image.img_file_name + suffix
 
     """
     下面是创建对象相关方法
     """
```

### Comparing `jmcomic-2.1.4/src/jmcomic/jm_toolkit.py` & `jmcomic-2.1.5/src/jmcomic/jm_toolkit.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,14 +148,29 @@
                 raise AssertionError(f"文本没有匹配上字段：字段名为'{field_name}'，pattern: [{pattern_value.pattern}]")
 
             # 保存字段
             field_dict[field_name] = field_value
 
         return clazz(**field_dict)
 
+    @classmethod
+    def format_photo_url(cls, photo_id, domain=None):
+        return cls.format_url(f'/photo/{cls.parse_to_photo_id(photo_id)}', domain)
+
+    @classmethod
+    def format_album_url(cls, album_id, domain=None):
+        return cls.format_url(f'/album/{cls.parse_to_album_id(album_id)}', domain)
+
+    @classmethod
+    def format_url(cls, path, domain=None):
+        if domain is None:
+            domain = JmModuleConfig.domain()
+
+        return f'{JmModuleConfig.PROT}{domain}{path}'
+
 
 class JmSearchSupport:
     # 用来缩减html的长度
     pattern_html_search_shorten_for = compile('<div class="well well-sm">([\s\S]*)'
                                               '<div class="row">[\s\S]*'
                                               '<div class="bot-per visible-xs visible-sm">')
 
@@ -202,31 +217,31 @@
             cls.open_Image(resp.content).save(filepath)
         else:
             save_resp_content(resp, filepath)
 
     @classmethod
     def save_resp_decoded_img(cls,
                               resp: Any,
-                              img_detail: JmImageDetail,
+                              image: JmImageDetail,
                               filepath: str
                               ) -> None:
         cls.decode_and_save(
-            cls.get_num_by_detail(img_detail),
+            cls.get_num_by_detail(image),
             cls.open_Image(resp.content),
             filepath
         )
 
     @classmethod
     def decode_disk_img(cls,
-                        img_detail: JmImageDetail,
+                        image: JmImageDetail,
                         img_filepath: str,
                         decoded_save_path: str
                         ) -> None:
         cls.decode_and_save(
-            cls.get_num_by_detail(img_detail),
+            cls.get_num_by_detail(image),
             cls.open_Image(img_filepath),
             decoded_save_path
         )
 
     @classmethod
     def decode_and_save(cls,
                         num: int,
```

### Comparing `jmcomic-2.1.4/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.1.5/src/jmcomic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.4
+Version: 2.1.5
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

