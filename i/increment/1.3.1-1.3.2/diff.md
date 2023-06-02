# Comparing `tmp/increment-1.3.1.tar.gz` & `tmp/increment-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "increment-1.3.1.tar", last modified: Mon May  1 02:01:16 2023, max compression
+gzip compressed data, was "increment-1.3.2.tar", last modified: Fri Jun  2 15:20:44 2023, max compression
```

## Comparing `increment-1.3.1.tar` & `increment-1.3.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 increment-1.3.1/LICENSE
--rw-r--r--   0        0        0     1699 2023-04-30 13:10:09.947977 increment-1.3.1/README.md
--rw-r--r--   0        0        0       29 2023-04-10 04:01:47.110396 increment-1.3.1/increment.py
--rw-r--r--   0        0        0      606 2023-04-30 19:29:45.948669 increment-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 increment-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 increment-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1825 2023-06-02 06:50:15.097906 increment-1.3.2/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 04:01:47.110396 increment-1.3.2/increment.py
+-rw-r--r--   0        0        0      608 2023-06-02 15:19:03.939502 increment-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 increment-1.3.2/PKG-INFO
```

### Comparing `increment-1.3.1/LICENSE` & `increment-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `increment-1.3.1/README.md` & `increment-1.3.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,71 +6,71 @@
 
 ```
 pip install increment
 ```
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
+[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQR-max.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
 
 开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
 
 # 教程
 
-导入：
+##### 导入
 
 ```python
 from increment import incrementer
 ```
 
-创建生成器：
+##### 创建生成器
 
 ```python
 inc = incrementer()
 ```
 
-使用创建生成器时的时间：
+##### 使用创建生成器时的时间
 
 ```python
 inc.pk1()
-# >>> 'lg85x42f_gsdo_258_0_1'
+# >>> 'lg85x42f_gsdo_258_1'
 
 inc.pk1()
-# >>> 'lg85x42f_gsdo_258_0_2'
+# >>> 'lg85x42f_gsdo_258_2'
 
 # 'lg85x42f'是创建生成器时的时间
 ```
 
-使用当前时间：
+##### 使用当前时间
 
 ```python
 inc.pk2()
-# >>> 'lg8657cj_gsdo_258_0_3'
+# >>> 'lg8657cj_gsdo_258_3'
 
 # 'lg8657cj'是当前时间
 ```
 
-只返回自增主键：
+##### 只返回自增主键
 
 ```python
 inc.pk3()
-# >>> '0_4'
+# >>> '4'
 
 inc.pk3()
-# >>> '0_5'
+# >>> '5'
 ```
 
 # 支持作者1元
 
 increment 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-200x200.jpg)
```

### Comparing `increment-1.3.1/pyproject.toml` & `increment-1.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "increment"
-version = "1.3.1"
+version = "1.3.2"
 description = "分布式主键生成器，支持多机器|多进程|多线程并发生成"
-dependencies = ["lccpy >=1.3"]
+dependencies = ["lccpy >=1.4.6"]
 keywords = ["increment"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `increment-1.3.1/PKG-INFO` & `increment-1.3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 Metadata-Version: 2.1
 Name: increment
-Version: 1.3.1
+Version: 1.3.2
 Summary: 分布式主键生成器，支持多机器|多进程|多线程并发生成
 Keywords: increment
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.3
+Requires-Dist: lccpy >=1.4.6
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/increment#readme
 
 # 项目描述
 
 分布式主键生成器，支持多机器|多进程|多线程并发生成。
 
 # 安装
 
 ```
 pip install increment
 ```
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
+[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQR-max.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
 
 开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)
 
 # 教程
 
-导入：
+##### 导入
 
 ```python
 from increment import incrementer
 ```
 
-创建生成器：
+##### 创建生成器
 
 ```python
 inc = incrementer()
 ```
 
-使用创建生成器时的时间：
+##### 使用创建生成器时的时间
 
 ```python
 inc.pk1()
-# >>> 'lg85x42f_gsdo_258_0_1'
+# >>> 'lg85x42f_gsdo_258_1'
 
 inc.pk1()
-# >>> 'lg85x42f_gsdo_258_0_2'
+# >>> 'lg85x42f_gsdo_258_2'
 
 # 'lg85x42f'是创建生成器时的时间
 ```
 
-使用当前时间：
+##### 使用当前时间
 
 ```python
 inc.pk2()
-# >>> 'lg8657cj_gsdo_258_0_3'
+# >>> 'lg8657cj_gsdo_258_3'
 
 # 'lg8657cj'是当前时间
 ```
 
-只返回自增主键：
+##### 只返回自增主键
 
 ```python
 inc.pk3()
-# >>> '0_4'
+# >>> '4'
 
 inc.pk3()
-# >>> '0_5'
+# >>> '5'
 ```
 
 # 支持作者1元
 
 increment 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR_1rmb_200_200.jpg)
+![donationQR.jpg](https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-200x200.jpg)
```

