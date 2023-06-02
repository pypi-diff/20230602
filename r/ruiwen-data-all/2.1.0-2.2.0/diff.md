# Comparing `tmp/ruiwen_data_all-2.1.0.tar.gz` & `tmp/ruiwen_data_all-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruiwen_data_all-2.1.0.tar", last modified: Mon Apr 10 13:30:21 2023, max compression
+gzip compressed data, was "ruiwen_data_all-2.2.0.tar", last modified: Fri Jun  2 12:24:54 2023, max compression
```

## Comparing `ruiwen_data_all-2.1.0.tar` & `ruiwen_data_all-2.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 13:30:21.645341 ruiwen_data_all-2.1.0/
--rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 13:30:21.643772 ruiwen_data_all-2.1.0/PKG-INFO
--rw-r--r--   0 xiaochuan   (501) staff       (20)      673 2023-04-10 13:30:11.000000 ruiwen_data_all-2.1.0/pyproject.toml
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 13:30:21.636912 ruiwen_data_all-2.1.0/ruiwen_data_all/
--rw-r--r--   0 xiaochuan   (501) staff       (20)    35999 2023-04-10 13:25:36.000000 ruiwen_data_all-2.1.0/ruiwen_data_all/__init__.py
-drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-04-10 13:30:21.642656 ruiwen_data_all-2.1.0/ruiwen_data_all.egg-info/
--rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-04-10 13:30:21.000000 ruiwen_data_all-2.1.0/ruiwen_data_all.egg-info/PKG-INFO
--rw-r--r--   0 xiaochuan   (501) staff       (20)      236 2023-04-10 13:30:21.000000 ruiwen_data_all-2.1.0/ruiwen_data_all.egg-info/SOURCES.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)        1 2023-04-10 13:30:21.000000 ruiwen_data_all-2.1.0/ruiwen_data_all.egg-info/dependency_links.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       53 2023-04-10 13:30:21.000000 ruiwen_data_all-2.1.0/ruiwen_data_all.egg-info/requires.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       16 2023-04-10 13:30:21.000000 ruiwen_data_all-2.1.0/ruiwen_data_all.egg-info/top_level.txt
--rw-r--r--   0 xiaochuan   (501) staff       (20)       38 2023-04-10 13:30:21.646007 ruiwen_data_all-2.1.0/setup.cfg
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-06-02 12:24:54.409652 ruiwen_data_all-2.2.0/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-06-02 12:24:54.409144 ruiwen_data_all-2.2.0/PKG-INFO
+-rw-r--r--   0 xiaochuan   (501) staff       (20)      673 2023-06-02 12:23:55.000000 ruiwen_data_all-2.2.0/pyproject.toml
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-06-02 12:24:54.397580 ruiwen_data_all-2.2.0/ruiwen_data_all/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)    36326 2023-06-02 12:18:29.000000 ruiwen_data_all-2.2.0/ruiwen_data_all/__init__.py
+drwxr-xr-x   0 xiaochuan   (501) staff       (20)        0 2023-06-02 12:24:54.408161 ruiwen_data_all-2.2.0/ruiwen_data_all.egg-info/
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       59 2023-06-02 12:24:54.000000 ruiwen_data_all-2.2.0/ruiwen_data_all.egg-info/PKG-INFO
+-rw-r--r--   0 xiaochuan   (501) staff       (20)      236 2023-06-02 12:24:54.000000 ruiwen_data_all-2.2.0/ruiwen_data_all.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)        1 2023-06-02 12:24:54.000000 ruiwen_data_all-2.2.0/ruiwen_data_all.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       53 2023-06-02 12:24:54.000000 ruiwen_data_all-2.2.0/ruiwen_data_all.egg-info/requires.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       16 2023-06-02 12:24:54.000000 ruiwen_data_all-2.2.0/ruiwen_data_all.egg-info/top_level.txt
+-rw-r--r--   0 xiaochuan   (501) staff       (20)       38 2023-06-02 12:24:54.409886 ruiwen_data_all-2.2.0/setup.cfg
```

### Comparing `ruiwen_data_all-2.1.0/pyproject.toml` & `ruiwen_data_all-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ruiwen_data_all"
-version = "2.1.0"
+version = "2.2.0"
 dependencies = [
   "redis",
   "requests",
   "asyncio",
   "urllib3",
   "pymongo",
   "w3lib",
@@ -17,14 +17,14 @@
 #python3 -m build
 #上传 win
 #twine upload dist/*
 #上传 mac
 #python3 -m twine upload dist/*
 #安装库
 #pip install --upgrade setuptools
-#pip install ruiwen-data-all==2.0.3
+#pip install ruiwen-data-all==2.1.0
 #pip install setuptools==57.5.0 -i https://pypi.tuna.tsinghua.edu.cn/simple
 #docker ps -a
 #docker exec -it 3a3afa942911 bash
 #pip install -U requests[socks]  socks5代理
 #pip install --index https://mirrors.ustc.edu.cn/pypi/web/simple/ virtualenv
```

### Comparing `ruiwen_data_all-2.1.0/ruiwen_data_all/__init__.py` & `ruiwen_data_all-2.2.0/ruiwen_data_all/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,21 +138,23 @@
                         txt_cn = {'quchong_md5': hashlib.md5(txt.encode(encoding='utf-8')).hexdigest(),
                                   'chaxun_md5': key_pd_md5, 'title': title_html, 'content': txt}
                         # 判断是否有栏目然后存储数据
                         if "(" in title_html and ")" in title_html:
                             try:
                                 self.mongo_db['fanwen']['daishenhe'].insert_one(txt_cn)
                                 self.redis_sql.sadd('fanwen_daishenhe_title_all', str([title_html, key_pd_md5]))
-                            except:
+                            except Exception as e:
+                                # print('写入数据报错为：',e)
                                 pass
                         else:
                             try:
                                 self.mongo_db['fanwen']['daishenhe_wufenlei'].insert_one(txt_cn)
                                 self.redis_sql.sadd('fanwen_daishenhe_wufenlei_title_all', str([title_html, key_pd_md5]))
-                            except:
+                            except Exception as e:
+                                # print('写入数据报错为：', e)
                                 pass
                         # 存储爬取过的url
                         self.redis_sql.sadd('%s_yu_quchong' % self.url_ku, url2)
         except Exception as e:
             print('出错了，错误为：%s'%e)
 
     # 中文转数字
@@ -626,24 +628,25 @@
                 html_content = html_content.replace(i, '<h2>fenge</h2>')
             # 提取瑞文系title
             title_ruixi = self.title_ruiwenxi(htm)
             # 通用标题处理
             title_html = self.title(title_ruixi)
             # 通用标题标签判断处理
             self.title_biaoqian_pd(title_html, fg_content, html_content, url)
-        except:
-            pass
+        except Exception as e:
+            print('内容处理报错为：', e)
 
     # 瑞文系数据库url遍历
     def ruiwen_xilie(self):
         # 去除已经爬取过的url
         zong_url = list(self.redis_sql.sdiff(self.url_ku, self.url_ku.replace('_url',
                 '_url_qita'), self.url_ku.replace('_url', '_yu_quchong'),self.url_ku.replace('_url', '_url_chucuo')))
         # 遍历差集url
         for url in zong_url:
+            zong_url.remove(url)
             # 判断是否为外站url
             if 'www.%s' % self.yu in url:
                 # 剔除指定栏目url
                 ti_url = 0
                 for ti in self.quchu_lujing_cis:
                     if ti in url:
                         ti_url = 1
@@ -668,34 +671,35 @@
         if sys.platform == 'win32':
             asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
         # 屏蔽警告
         warnings.simplefilter('ignore', DeprecationWarning)
         pool = redis.ConnectionPool(host=self.ip_all, port=self.redis_port, password=self.redis_password, db=self.redis_db,
                                     decode_responses=True)
         self.redis_sql = redis.Redis(connection_pool=pool)
+        self.mongodb_ip = str(self.redis_sql.get('mongodb_ip'))
         self.mongodb_port = int(self.redis_sql.get('mongodb_port'))
         self.mongodb_password = str(self.redis_sql.get('mongodb_password'))
         self.daili_no = str(self.redis_sql.get('daili_no'))
         self.daili_name = str(self.redis_sql.get('daili_name'))
         self.daili_password = str(self.redis_sql.get('daili_password'))
         self.dali_host = str(self.redis_sql.get('dali_host'))
         self.daili_port = int(self.redis_sql.get('daili_port'))
         self.emall_fsz = str(self.redis_sql.get('emall_fsz'))
         self.emall_name = str(self.redis_sql.get('emall_name'))
         self.emall_password = str(self.redis_sql.get('emall_password'))
         self.emall_sjr = str(self.redis_sql.get('emall_sjr'))
-        yuming_all = list(self.redis_sql.smembers('fanwen_yuming2'))[self.zhan_number].replace("'", "").replace('[',
+        yuming_all = sorted(list(self.redis_sql.smembers('fanwen_yuming2')))[self.zhan_number].replace("'", "").replace('[',
                                                   '').replace(']','').split(', ')
         self.yu = yuming_all[1]
         self.url_ku = yuming_all[0]
         # 判断是否开启代理
         if self.daili_no == '1':
             self.session = requests.session()
             self.session.keep_alive = False
-        self.mongo_db = pymongo.MongoClient(self.ip_all, self.mongodb_port, username='root', password=self.mongodb_password)
+        self.mongo_db = pymongo.MongoClient(self.mongodb_ip, self.mongodb_port, username='root', password=self.mongodb_password)
         for biao in ['quchu_title_ci', 'quchu_title_content_ci', 'quchu_lujing_ci', 'quchu_content_ci', 'tag_ciku']:
             # 去除标题内指定词
             if biao == 'quchu_title_ci':
                 self.quchu_title_cis = list(self.redis_sql.smembers(biao))
             # 去除标题含指定词的内容
             elif biao == 'quchu_title_content_ci':
                 self.quchu_title_content_cis = list(self.redis_sql.smembers(biao))
```

