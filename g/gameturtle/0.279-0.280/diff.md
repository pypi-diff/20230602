# Comparing `tmp/gameturtle-0.279.tar.gz` & `tmp/gameturtle-0.280.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gameturtle-0.279.tar", last modified: Wed Sep 29 09:22:52 2021, max compression
+gzip compressed data, was "gameturtle-0.280.tar", last modified: Fri Jun  2 08:37:18 2023, max compression
```

## Comparing `gameturtle-0.279.tar` & `gameturtle-0.280.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2021-09-29 09:22:52.859383 gameturtle-0.279/
--rw-rw-rw-   0        0        0     1572 2021-09-29 09:22:52.855383 gameturtle-0.279/PKG-INFO
--rw-rw-rw-   0        0        0     1001 2020-01-01 03:51:20.000000 gameturtle-0.279/README.md
-drwxrwxrwx   0        0        0        0 2021-09-29 09:22:52.830381 gameturtle-0.279/gameturtle/
--rw-rw-rw-   0        0        0    69957 2021-09-29 09:21:10.000000 gameturtle-0.279/gameturtle/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-29 09:22:52.853383 gameturtle-0.279/gameturtle.egg-info/
--rw-rw-rw-   0        0        0     1572 2021-09-29 09:22:52.000000 gameturtle-0.279/gameturtle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2021-09-29 09:22:52.000000 gameturtle-0.279/gameturtle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-29 09:22:52.000000 gameturtle-0.279/gameturtle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-09-29 09:22:46.000000 gameturtle-0.279/gameturtle.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2021-09-29 09:22:52.000000 gameturtle-0.279/gameturtle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-09-29 09:22:52.000000 gameturtle-0.279/gameturtle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-09-29 09:22:52.859383 gameturtle-0.279/setup.cfg
--rw-rw-rw-   0        0        0      746 2021-09-29 09:21:43.000000 gameturtle-0.279/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:37:18.392162 gameturtle-0.280/
+-rw-rw-rw-   0        0        0     1582 2023-06-02 08:37:18.390162 gameturtle-0.280/PKG-INFO
+-rw-rw-rw-   0        0        0     1001 2020-01-01 03:51:20.000000 gameturtle-0.280/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 08:37:18.321158 gameturtle-0.280/gameturtle/
+-rw-rw-rw-   0        0        0    70639 2023-06-01 03:58:52.000000 gameturtle-0.280/gameturtle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:37:18.352160 gameturtle-0.280/gameturtle.egg-info/
+-rw-rw-rw-   0        0        0     1582 2023-06-02 08:37:18.000000 gameturtle-0.280/gameturtle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-02 08:37:18.000000 gameturtle-0.280/gameturtle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 08:37:18.000000 gameturtle-0.280/gameturtle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 08:37:03.000000 gameturtle-0.280/gameturtle.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-06-02 08:37:18.000000 gameturtle-0.280/gameturtle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-02 08:37:18.000000 gameturtle-0.280/gameturtle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 08:37:18.394162 gameturtle-0.280/setup.cfg
+-rw-rw-rw-   0        0        0      756 2023-06-02 08:36:55.000000 gameturtle-0.280/setup.py
```

### Comparing `gameturtle-0.279/PKG-INFO` & `gameturtle-0.280/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameturtle
-Version: 0.279
+Version: 0.280
 Summary: Python gameturtle Module for make animations and games easily，by www.lixingqiu.com 
 Home-page: http://www.lixingqiu.com
 Author: lixingqiu
 Author-email: 406273900@qq.com
 License: MIT
 Description: ﻿# Python sprites module introduce
         
@@ -21,10 +21,10 @@
         5、Python experience courses and public welfare courses of training institutions.
         
          
         
         more example,please conatct lixingqiu, wechat:scratch8,website:<http://www.lixingqiu.com>
         
         sprites module Developer: Li Xingqiu，email:406273900@qq.com,Pingxiang, Jiangxi, China.
-Keywords: turtle game tkinter game pillow numpy pixel collide frame splitframe makegif splitgif
+Keywords: turtle game tkinter game pillow numpy pixel collide frame splitframe makegif makevideo splitgif
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gameturtle-0.279/README.md` & `gameturtle-0.280/README.md`

 * *Files identical despite different names*

### Comparing `gameturtle-0.279/gameturtle/__init__.py` & `gameturtle-0.280/gameturtle/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 ﻿"""
-   Sprite.py   
+   gameturtle.py   
    0.279版对0.273版进行了微调，主要是group和grab两个函数。
    增加了把RGB颜色三元组转换成以#开头的颜色转换函数，如(255,0,0)转换为#ff0000
    同时微调了pencolor命令。解决了不接收RGB三元组作为颜色报错问题。
    去掉了is_chinese函数，直接算字符的字节数，让single2multitext更加精准。
    新增了Key和Mouse类，进键盘和鼠标按键进行按键检测。
    增加了out_canvas的别名collide_edge
    新增make_rect，make_ellispe函数，用于生成矩形图和椭圆图，还有make_circle和make_square函数。
    新增replace_color替换颜色函数，角色的write命令，circle命令。
    新增pixelate像素化图形函数，mozaic马赛克图像处理函数。
    从tkinter.message模块导入了所有显示信息的命令对话框。
+   single2multitext函数把gb2312改成了utf-8
 """
 __author__ = '李兴球'
-__date__ = '2021/9/29'
+__date__ = '2023/06/01'
 __blog__ = 'www.lixingqiu.com'
-__version__ = 0.279
+__version__ = 0.280
 
 import os
 import time
 import math
 import numpy as np
 from random import randint
 from tkinter import Tk,Canvas
 from tkinter.messagebox import *
+from moviepy.editor import ImageSequenceClip
 from PIL import Image,ImageTk,ImageGrab,ImageOps,ImageDraw,ImageColor,ImageFont,ImageSequence
 
 
 def replace_color(im,source,dest):
     """颜色替换函数，把source颜色换成dest颜色
        im：pillow图形对象,
        soucrce: 将要换的颜色值，如[255,0,0,255]为红色
@@ -118,15 +120,15 @@
     txtbiao = []
     start = 0
     index = 0
     # w是一个计数器，记录当前行字母数(一个汉字算两个字母)是否超出length
     w = 0                                               
     current_line_length = 0
     while index < len(line):       
-        w = w + len(bytes(line[index],'gb2312'))             # 根据字节长度决定位数    
+        w = w + len(bytes(line[index],'utf-8'))             # 根据字节长度决定位数3个字节一个汉字,所以写length90的话一行显示30汉字 
         current_line_length += 1
         if w>= length or line[index]=='\n':
             if line[index]=='\n':  current_line_length -= 1      # 不加入换行符
             txtbiao.append(line[start:start+current_line_length]) # current_line_length是动态的。
             start += current_line_length
             if line[index]=='\n':start+= 1
             w = 0
@@ -232,15 +234,25 @@
        images = [ images + os.sep + str(i) + ext for i in range(0,amounts)]
        frames = [Image.open(frame) for frame in images]
 
    pic = frames[0]
    if filename==None:filename=str(time.time()) + ".gif"
    pic.save(filename, save_all=True,append_images=frames[1:],
             optimize=True,quality=quality,duration=duration,loop=loop)
-   
+
+def makevideo(images,filename=None,fps=30, durations=None, with_mask=True, ismask=False, load_images=False):
+    """images:是一个列表,列表中是pillow图形对象,或者是一个文件夹路径名"""
+    if isinstance(images,list):
+        images = [np.array(im) for im in images]
+    clip = ImageSequenceClip(images, fps=fps,durations=durations,with_mask=with_mask,ismask=ismask,load_images=load_images)
+    if filename:
+        clip.write_videofile(filename, fps=fps)
+    else:
+        return clip
+    
 def txt2images(string,width=480,height=360,background=None,margin=68,fontsize=18,
                fontfile="simkai.ttf",fgcolor=(150,200,200,255),bgcolor=(0,0,0,0),compress=False):
     
     """文本转逐帧图像,string:字符串，width:宽度，height:高度,background:背景图或颜色,
        margin:边距，fontsize:字体大小，fgcolor:字的颜色，bgcolor:背景色
 
     """
```

### Comparing `gameturtle-0.279/gameturtle.egg-info/PKG-INFO` & `gameturtle-0.280/gameturtle.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameturtle
-Version: 0.279
+Version: 0.280
 Summary: Python gameturtle Module for make animations and games easily，by www.lixingqiu.com 
 Home-page: http://www.lixingqiu.com
 Author: lixingqiu
 Author-email: 406273900@qq.com
 License: MIT
 Description: ﻿# Python sprites module introduce
         
@@ -21,10 +21,10 @@
         5、Python experience courses and public welfare courses of training institutions.
         
          
         
         more example,please conatct lixingqiu, wechat:scratch8,website:<http://www.lixingqiu.com>
         
         sprites module Developer: Li Xingqiu，email:406273900@qq.com,Pingxiang, Jiangxi, China.
-Keywords: turtle game tkinter game pillow numpy pixel collide frame splitframe makegif splitgif
+Keywords: turtle game tkinter game pillow numpy pixel collide frame splitframe makegif makevideo splitgif
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gameturtle-0.279/setup.py` & `gameturtle-0.280/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 with open("README.md", encoding='utf-8') as fh:
     long_d = fh.read()
 
 
 setup(name='gameturtle',
       long_description_content_type="text/markdown",
-      version = '0.279',
+      version = '0.280',
       description = 'Python gameturtle Module for make animations and games easily，by www.lixingqiu.com ',
       long_description = long_d,      
-      keywords = 'turtle game tkinter game pillow numpy pixel collide frame splitframe makegif splitgif',
+      keywords = 'turtle game tkinter game pillow numpy pixel collide frame splitframe makegif makevideo splitgif',
       url = 'http://www.lixingqiu.com',
       author ='lixingqiu',
       author_email = '406273900@qq.com',
       license = 'MIT',
       packages = ['gameturtle'],
       zip_safe = False,
       install_requires = [ 'pillow>=2.7.0','numpy']
```

