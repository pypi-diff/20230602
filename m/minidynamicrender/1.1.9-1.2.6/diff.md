# Comparing `tmp/minidynamicrender-1.1.9.tar.gz` & `tmp/minidynamicrender-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidynamicrender-1.1.9.tar", max compression
+gzip compressed data, was "minidynamicrender-1.2.6.tar", max compression
```

## Comparing `minidynamicrender-1.1.9.tar` & `minidynamicrender-1.2.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    18431 2023-03-12 06:39:57.842329 minidynamicrender-1.1.9/LICENSE
--rw-r--r--   0        0        0     2340 2023-03-12 06:39:57.842329 minidynamicrender-1.1.9/README.md
--rw-r--r--   0        0        0     2121 2023-03-12 06:39:57.842329 minidynamicrender-1.1.9/minidynamicrender/Core.py
--rw-r--r--   0        0        0    36804 2023-03-12 06:39:57.842329 minidynamicrender-1.1.9/minidynamicrender/DynAdditional.py
--rw-r--r--   0        0        0     6577 2023-03-12 06:39:57.842329 minidynamicrender-1.1.9/minidynamicrender/DynConfig.py
--rw-r--r--   0        0        0     1782 2023-03-12 06:39:57.842329 minidynamicrender-1.1.9/minidynamicrender/DynForward.py
--rw-r--r--   0        0        0    12283 2023-03-12 06:39:57.842329 minidynamicrender-1.1.9/minidynamicrender/DynHeader.py
--rw-r--r--   0        0        0    55078 2023-03-12 06:39:57.842329 minidynamicrender-1.1.9/minidynamicrender/DynMajor.py
--rw-r--r--   0        0        0    14093 2023-03-12 06:39:57.842329 minidynamicrender-1.1.9/minidynamicrender/DynText.py
--rw-r--r--   0        0        0   332699 2023-03-12 06:41:10.414239 minidynamicrender-1.1.9/minidynamicrender/Static.zip
--rw-r--r--   0        0        0     2773 2023-03-12 06:39:57.878329 minidynamicrender-1.1.9/minidynamicrender/Tools.py
--rw-r--r--   0        0        0        0 2023-03-12 06:39:57.878329 minidynamicrender-1.1.9/minidynamicrender/__init__.py
--rw-r--r--   0        0        0      677 2023-03-12 06:46:33.265786 minidynamicrender-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     3253 1970-01-01 00:00:00.000000 minidynamicrender-1.1.9/setup.py
--rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 minidynamicrender-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0    18431 2023-03-12 06:39:57.842329 minidynamicrender-1.2.6/LICENSE
+-rw-r--r--   0        0        0     2340 2023-03-12 06:39:57.842329 minidynamicrender-1.2.6/README.md
+-rw-r--r--   0        0        0     2121 2023-03-12 06:39:57.842329 minidynamicrender-1.2.6/minidynamicrender/Core.py
+-rw-r--r--   0        0        0    36804 2023-03-12 06:39:57.842329 minidynamicrender-1.2.6/minidynamicrender/DynAdditional.py
+-rw-r--r--   0        0        0     6577 2023-03-12 06:39:57.842329 minidynamicrender-1.2.6/minidynamicrender/DynConfig.py
+-rw-r--r--   0        0        0     1782 2023-03-12 06:39:57.842329 minidynamicrender-1.2.6/minidynamicrender/DynForward.py
+-rw-r--r--   0        0        0    12283 2023-03-12 06:39:57.842329 minidynamicrender-1.2.6/minidynamicrender/DynHeader.py
+-rw-r--r--   0        0        0    55078 2023-03-12 06:39:57.842329 minidynamicrender-1.2.6/minidynamicrender/DynMajor.py
+-rw-r--r--   0        0        0    14120 2023-06-02 11:12:49.673332 minidynamicrender-1.2.6/minidynamicrender/DynText.py
+-rw-r--r--   0        0        0     2773 2023-03-12 06:39:57.878329 minidynamicrender-1.2.6/minidynamicrender/Tools.py
+-rw-r--r--   0        0        0        0 2023-03-12 06:39:57.878329 minidynamicrender-1.2.6/minidynamicrender/__init__.py
+-rw-r--r--   0        0        0      776 2023-06-02 11:12:56.517335 minidynamicrender-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 minidynamicrender-1.2.6/setup.py
+-rw-r--r--   0        0        0     3158 1970-01-01 00:00:00.000000 minidynamicrender-1.2.6/PKG-INFO
```

### Comparing `minidynamicrender-1.1.9/LICENSE` & `minidynamicrender-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `minidynamicrender-1.1.9/README.md` & `minidynamicrender-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `minidynamicrender-1.1.9/minidynamicrender/Core.py` & `minidynamicrender-1.2.6/minidynamicrender/Core.py`

 * *Files identical despite different names*

### Comparing `minidynamicrender-1.1.9/minidynamicrender/DynAdditional.py` & `minidynamicrender-1.2.6/minidynamicrender/DynAdditional.py`

 * *Files identical despite different names*

### Comparing `minidynamicrender-1.1.9/minidynamicrender/DynConfig.py` & `minidynamicrender-1.2.6/minidynamicrender/DynConfig.py`

 * *Files identical despite different names*

### Comparing `minidynamicrender-1.1.9/minidynamicrender/DynForward.py` & `minidynamicrender-1.2.6/minidynamicrender/DynForward.py`

 * *Files identical despite different names*

### Comparing `minidynamicrender-1.1.9/minidynamicrender/DynHeader.py` & `minidynamicrender-1.2.6/minidynamicrender/DynHeader.py`

 * *Files identical despite different names*

### Comparing `minidynamicrender-1.1.9/minidynamicrender/DynMajor.py` & `minidynamicrender-1.2.6/minidynamicrender/DynMajor.py`

 * *Files identical despite different names*

### Comparing `minidynamicrender-1.1.9/minidynamicrender/DynText.py` & `minidynamicrender-1.2.6/minidynamicrender/DynText.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
                 await self.draw_rich_text(i, rich_list)
 
         if self.offset != 45:
             self.pic_list.append(self.background)
 
     async def draw_pain_text(self, dyn_type: str, dyn_detail):
         dyn_detail = dyn_detail.translate(str.maketrans(
-            {'\r': '', chr(65039): '', chr(65038): '', chr(8205): ''}))
+            {'\r': '', chr(65039): '', chr(65038): '', chr(8205): '',chr(65279):'',chr(8203):""}))
         if dyn_type in {"RICH_TEXT_NODE_TYPE_AT", "RICH_TEXT_NODE_TYPE_TOPIC"}:
             for i in dyn_detail:
                 self.draw.text((self.offset, 0), i,
                                fill=self.dyn_color.dyn_blue, font=self.text_font)
                 self.offset += self.text_font.getlength(i)
                 if self.offset >= 1020:
                     self.pic_list.append(self.background)
```

### Comparing `minidynamicrender-1.1.9/minidynamicrender/Tools.py` & `minidynamicrender-1.2.6/minidynamicrender/Tools.py`

 * *Files identical despite different names*

### Comparing `minidynamicrender-1.1.9/pyproject.toml` & `minidynamicrender-1.2.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 [tool.poetry]
 name = "minidynamicrender"
-version = "1.1.9"
+version = "1.2.6"
 description = "A package that transform bilibili's dynamic data to image"
 authors = ["DMC <lzxder@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 loguru = "^0.6.0"
 pillow = "^9.4.0"
 qrcode = "^7.3.1"
-httpx = "^0.23.2"
+httpx = "^0.24.0"
 numpy = "^1.24.1"
-dynamicadaptor = "0.3.7"
+dynamicadaptor = "^0.4.3"
 emoji = "^2.2.0"
 fonttools = "^4.38.0"
 
 
 [[tool.poetry.source]]
 name = "url"
-url = "https://mirrors.bfsu.edu.cn/pypi/web/simple/"
+url = "https://pypi.org/simple"
 default = true
 secondary = false
 
+
+[[tool.poetry.source]]
+name = "qh"
+url = "https://pypi.tuna.tsinghua.edu.cn/simple"
+default = false
+secondary = true
+
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.1"
 bilirpc = "^0.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `minidynamicrender-1.1.9/setup.py` & `minidynamicrender-1.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 packages = \
 ['minidynamicrender']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['dynamicadaptor==0.3.7',
+['dynamicadaptor>=0.4.3,<0.5.0',
  'emoji>=2.2.0,<3.0.0',
  'fonttools>=4.38.0,<5.0.0',
- 'httpx>=0.23.2,<0.24.0',
+ 'httpx>=0.24.0,<0.25.0',
  'loguru>=0.6.0,<0.7.0',
  'numpy>=1.24.1,<2.0.0',
  'pillow>=9.4.0,<10.0.0',
  'qrcode>=7.3.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'minidynamicrender',
-    'version': '1.1.9',
+    'version': '1.2.6',
     'description': "A package that transform bilibili's dynamic data to image",
     'long_description': '# DynamicRender\n\n用于将B站的动态渲染为图片（需要配合适配器将动态转化为特定格式）\n\n## 使用\n\n### 安装\n\n```bash\npip install dynamicrender\n```\n\n### 1. 格式化动态\n\n```python\n\n# 如果数据是grpc返回的数据\nfrom google.protobuf.json_format import MessageToDict\nfrom dynamicadaptor.DynamicConversion import formate_message\nfrom bilirpc.api import get_dy_detail\nimport asyncio\nfrom dynamicrender.Core import DyRender \n\nasync def sample1():\n    dynamic_grpc = await get_dy_detail("746530608345251842")\n    dynamic: dict = MessageToDict(dynamic_grpc[0])\n    dynamic_formate = formate_message("grpc", dynamic)\n    render = DyRender()\n    # DyRender 实例化时可以传两个参数\n    #1. data_path: {str} 为静态文件所在的位置，当data_path内不存在Static目录，则会自动解压自带的Static到data_path内\n    # 2.font_path: {str/dic}当font_path为str类型的时候必须为字体的路径，路径不存在的话会使用默认的字体\n    # 不建议使用传dict的方法修改字体\n    # 当font_path为dict的时候必须为如以下所示的dict:\n    """\n    {\n     text: str\n     extra_text: str\n     emoji: str\n    }\n    三个都必须是字体的路径，text为文本主体的字体路径，extra_text为备选字体的路径，emoji为emoji字体的路径，\n    \n    注意！！！\n    \n    每款emoji字体的字体大小都有固定值，如果修改了emoji字体必须同时修改emoji字体的字体大小\n    \n    """\n    result = await render.dyn_render(dynamic_formate)\n    result.show()\n    \nasyncio.run(sample1())\n\n\n\n# 如果是web返回的数据\n\nimport asyncio\nimport httpx\nfrom dynamicrender.Core import DyRender\nfrom dynamicadaptor.DynamicConversion import formate_message \n\nasync def sample2():\n    url = "https://api.bilibili.com/x/polymer/web-dynamic/v1/detail?timezone_offset=-480&id=746530608345251842"\n    headers = {\n        "Referer": "https://t.bilibili.com/746530608345251842"\n    }\n    result = httpx.get(url, headers=headers).json()\n    dynamic_formate = formate_message("web", result["data"]["item"])\n    render = DyRender()\n    result = await render.dyn_render(dynamic_formate)\n    result.show()\n\n\n# asyncio.run(sample2())\n\n```\n\n### 示例\n\n![示例图片](https://i0.hdslb.com/bfs/new_dyn/7fcb290284e46c75f432ee069349a49a37815472.png)',
     'author': 'DMC',
     'author_email': 'lzxder@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `minidynamicrender-1.1.9/PKG-INFO` & `minidynamicrender-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: minidynamicrender
-Version: 1.1.9
+Version: 1.2.6
 Summary: A package that transform bilibili's dynamic data to image
 Author: DMC
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dynamicadaptor (==0.3.7)
+Requires-Dist: dynamicadaptor (>=0.4.3,<0.5.0)
 Requires-Dist: emoji (>=2.2.0,<3.0.0)
 Requires-Dist: fonttools (>=4.38.0,<5.0.0)
-Requires-Dist: httpx (>=0.23.2,<0.24.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: qrcode (>=7.3.1,<8.0.0)
 Description-Content-Type: text/markdown
 
 # DynamicRender
```

