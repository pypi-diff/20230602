# Comparing `tmp/discordlevelingcard-0.5.6.tar.gz` & `tmp/discordlevelingcard-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordlevelingcard-0.5.6.tar", max compression
+gzip compressed data, was "discordlevelingcard-0.6.0.tar", max compression
```

## Comparing `discordlevelingcard-0.5.6.tar` & `discordlevelingcard-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      129 2023-05-29 17:20:09.194905 discordlevelingcard-0.5.6/DiscordLevelingCard/__init__.py
--rw-r--r--   0        0        0      842 2023-04-25 08:29:49.129344 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/curveborder.png
--rw-r--r--   0        0        0     2596 2023-04-25 08:29:49.129826 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/curvedoverlay.png
--rw-r--r--   0        0        0    60288 2023-04-25 08:29:49.131350 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/levelfont.otf
--rw-r--r--   0        0        0     9742 2023-04-25 08:29:49.132354 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/mask_circle.jpg
--rw-r--r--   0        0        0     3024 2023-05-30 11:34:28.727698 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/mask_hexagon.png
--rw-r--r--   0        0        0     4775 2023-05-29 17:05:04.175407 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/overlay1.png
--rw-r--r--   0        0        0     2590 2023-04-25 08:29:49.133788 discordlevelingcard-0.5.6/DiscordLevelingCard/card_settings.py
--rw-r--r--   0        0        0    12505 2023-05-29 17:39:37.772268 discordlevelingcard-0.5.6/DiscordLevelingCard/discord_card.py
--rw-r--r--   0        0        0      531 2023-04-25 08:29:49.134664 discordlevelingcard-0.5.6/DiscordLevelingCard/error.py
--rw-r--r--   0        0        0    13919 2023-05-30 18:51:58.560733 discordlevelingcard-0.5.6/DiscordLevelingCard/sandbox.py
--rw-r--r--   0        0        0    10446 2023-05-30 17:34:42.418755 discordlevelingcard-0.5.6/DiscordLevelingCard/tester.py
--rw-r--r--   0        0        0     1083 2023-04-25 08:29:49.135173 discordlevelingcard-0.5.6/LICENSE
--rw-r--r--   0        0        0      929 2023-05-30 18:28:32.085735 discordlevelingcard-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     8785 2023-05-30 18:57:13.411441 discordlevelingcard-0.5.6/README.md
--rw-r--r--   0        0        0     9587 2023-05-30 19:01:35.151432 discordlevelingcard-0.5.6/setup.py
--rw-r--r--   0        0        0     9383 2023-05-30 19:01:35.151432 discordlevelingcard-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      129 2023-05-29 17:20:09.194905 discordlevelingcard-0.6.0/DiscordLevelingCard/__init__.py
+-rw-r--r--   0        0        0      842 2023-04-25 08:29:49.129344 discordlevelingcard-0.6.0/DiscordLevelingCard/assets/curveborder.png
+-rw-r--r--   0        0        0     2596 2023-04-25 08:29:49.129826 discordlevelingcard-0.6.0/DiscordLevelingCard/assets/curvedoverlay.png
+-rw-r--r--   0        0        0    60288 2023-04-25 08:29:49.131350 discordlevelingcard-0.6.0/DiscordLevelingCard/assets/levelfont.otf
+-rw-r--r--   0        0        0     9742 2023-04-25 08:29:49.132354 discordlevelingcard-0.6.0/DiscordLevelingCard/assets/mask_circle.jpg
+-rw-r--r--   0        0        0     3024 2023-05-30 11:34:28.727698 discordlevelingcard-0.6.0/DiscordLevelingCard/assets/mask_hexagon.png
+-rw-r--r--   0        0        0     4775 2023-05-29 17:05:04.175407 discordlevelingcard-0.6.0/DiscordLevelingCard/assets/overlay1.png
+-rw-r--r--   0        0        0     2590 2023-04-25 08:29:49.133788 discordlevelingcard-0.6.0/DiscordLevelingCard/card_settings.py
+-rw-r--r--   0        0        0    12505 2023-05-29 17:39:37.772268 discordlevelingcard-0.6.0/DiscordLevelingCard/discord_card.py
+-rw-r--r--   0        0        0      531 2023-04-25 08:29:49.134664 discordlevelingcard-0.6.0/DiscordLevelingCard/error.py
+-rw-r--r--   0        0        0    16406 2023-06-02 16:19:14.934334 discordlevelingcard-0.6.0/DiscordLevelingCard/sandbox.py
+-rw-r--r--   0        0        0    12197 2023-06-02 16:30:02.167203 discordlevelingcard-0.6.0/DiscordLevelingCard/tester.py
+-rw-r--r--   0        0        0     1083 2023-04-25 08:29:49.135173 discordlevelingcard-0.6.0/LICENSE
+-rw-r--r--   0        0        0      929 2023-06-02 16:30:10.278178 discordlevelingcard-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    11340 2023-06-02 16:19:16.408370 discordlevelingcard-0.6.0/README.md
+-rw-r--r--   0        0        0    12143 2023-06-02 16:33:14.157535 discordlevelingcard-0.6.0/setup.py
+-rw-r--r--   0        0        0    11871 2023-06-02 16:33:14.158036 discordlevelingcard-0.6.0/PKG-INFO
```

### Comparing `discordlevelingcard-0.5.6/DiscordLevelingCard/assets/curveborder.png` & `discordlevelingcard-0.6.0/DiscordLevelingCard/assets/curveborder.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.6/DiscordLevelingCard/assets/curvedoverlay.png` & `discordlevelingcard-0.6.0/DiscordLevelingCard/assets/curvedoverlay.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.6/DiscordLevelingCard/assets/levelfont.otf` & `discordlevelingcard-0.6.0/DiscordLevelingCard/assets/levelfont.otf`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.6/DiscordLevelingCard/assets/mask_circle.jpg` & `discordlevelingcard-0.6.0/DiscordLevelingCard/assets/mask_circle.jpg`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.6/DiscordLevelingCard/assets/mask_hexagon.png` & `discordlevelingcard-0.6.0/DiscordLevelingCard/assets/mask_hexagon.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.6/DiscordLevelingCard/assets/overlay1.png` & `discordlevelingcard-0.6.0/DiscordLevelingCard/assets/overlay1.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.6/DiscordLevelingCard/card_settings.py` & `discordlevelingcard-0.6.0/DiscordLevelingCard/card_settings.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.6/DiscordLevelingCard/discord_card.py` & `discordlevelingcard-0.6.0/DiscordLevelingCard/discord_card.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.6/DiscordLevelingCard/error.py` & `discordlevelingcard-0.6.0/DiscordLevelingCard/error.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.6/DiscordLevelingCard/sandbox.py` & `discordlevelingcard-0.6.0/DiscordLevelingCard/sandbox.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from io import BytesIO
-from typing import Optional, Union
+from typing import Optional, Union, List
 
 from aiohttp import ClientSession
 from PIL import Image, ImageDraw, ImageFont, ImageColor
 from .error import InvalidImageUrl
 from pathlib import Path
 from .card_settings import Settings
 
@@ -47,14 +47,16 @@
     - `max_exp`
     - `rank`
 
     Methods
     -------
     - `custom_card1`
         Creates a rank card with the first design
+    -  `custom_canvas`
+        A blank canvas to make whatever you want!
 
     Raises
     ------
     - `InvalidImageType`
         If the image type is not supported
     - `InvalidImageUrl`
         If the image url is invalid
@@ -208,23 +210,25 @@
             self.background = self.background.resize((int(self.background.size[0]*(resize/100)), int(self.background.size[1]*(resize/100))))
         
         self.background.save(image, 'PNG')
         image.seek(0)
         return image
 
 
-    async def custom_card3(
+    async def custom_canvas(
             self,
-            resize:int = 100,
 
-            senstivity:int = 200,
-            card_colour: str = "black",
+            has_background: bool = True,
+            background_colour: str = "black",
+
+            canvas_size: tuple = (1000, 333),
+
+            resize:int = 100,
 
-            border_width: int = 25,
-            border_height: int = 25,
+            overlay: Union[None, List] = [[(1000-50, 333-50),(25, 25), "black", 200]],
             
             avatar_frame: str = "curvedborder",
             avatar_size: int = 260,
             avatar_position: tuple = (53, 36),
             
             text_font: str = "levelfont.otf",
 
@@ -232,39 +236,48 @@
             username_font_size: int = 50,
 
             level_position: tuple = (500,40),
             level_font_size: int = 50,
 
             exp_position: tuple = (775,130),
             exp_font_size: int = 50,
+            bar_exp: Union[None, int] = None,
+
+            exp_bar_width: int = 619,
+            exp_bar_height: int = 50,
+            exp_bar_background_colour: Union[str, tuple] = "white",
+            exp_bar_position:tuple = (330, 235),
+            exp_bar_curve: int = 30,
+            extra_text: Union[List, None] = None
+
+
         )-> Union[None, bytes]:
         """
         Sandbox for third type of card which returns "BytesIO"
 
         Parameters
         ----------
+        has_background: :class:`bool`
+            Whether to use a background image or not. Default is True
+        
+        background_colour: :class:`str`
+            The colour of the background, only used if has_background is set to False. Default is black.
+        
+        canvas_size: :class:`tuple`
+            The size of the canvas. Default is (1000, 333)
+        
         resize: :class:`int`
             The percentage to resize the image to. Default is 100
-        
-        senstivity: :class:`int`
-            Change the transparency of the black box over the background image.
-                Default is 200.range - [0,255] 
+                    
+        overlay: :class:`list`
+            A list of overlays to be placed on the background. Default is [[(1000-50, 333-50),(25, 25), "black", 200]].
 
-        border_width: :class:`int`
-            width of the border. default is 25
-
-        border_height: :class:`int`
-            height of the border. default is 25
-            
         avatar_frame: :class:`str`
             `circle` `square` `curvedborder` `hexagon` or path to a self created mask.
         
-        card_colour: :class:`str`
-            colour of the translucent overlay. Default is black.
-
         text_font: :class:`str`
             Default is `levelfont.otf` or path to a custom otf or ttf file type font.
 
         avatar_size: :class:`int`
             size of the avatar. Default is 260.
 
         avatar_position: :class:`tuple`
@@ -283,47 +296,81 @@
             font size of the level. Default is 50.
 
         exp_position: :class:`tuple`
             pixel position of the exp to be placed at. Default is (775,130)
         
         exp_font_size: :class:`int`
             font size of the exp. Default is 50.
+
+        exp_bar_width: :class:`int`
+            width of the exp bar. Default is 619.
+        
+        exp_bar_height: :class:`int`
+            height of the exp bar. Default is 50.
+        
+        exp_bar_background_colour: :class:`str`
+            colour of the exp bar. Default is white.
+        
+        exp_bar_position: :class:`tuple`
+            pixel position of the exp bar to be placed at. Default is (330, 235)
         
+        exp_bar_curve: :class:`int`
+            curve of the exp bar. Default is 30.
+
+        extra_text: :class:`list`
+            list of tuples containing text and position of the text to be placed on the card. Default is None. eg ["string", (x-position, y-position), font-size, "colour"]
+
+        exp_bar: :class:`int`
+            The calculated exp of the user. Default is None.
+        
+
         Attributes
         ----------
+        - `has_background`
+        - `background_colour`
+        - `canvas_size`
         - `resize`
-        - `senstivity`
-        - `border_width`
-        - `border_height`
+        - `overlay`
         - `avatar_frame`
-        - `card_colour`
         - `text_font`
         - `avatar_size`
         - `avatar_position`
         - `username_position`
         - `username_font_size`
         - `level_position`
         - `level_font_size`
         - `exp_position`
         - `exp_font_size`
+        - `exp_bar_width`
+        - `exp_bar_height`
+        - `exp_bar_background_colour`
+        - `exp_bar_position`
+        - `exp_bar_curve`
+        - `extra_text`
+        - `exp_bar`
         
         """
         path = str(Path(__file__).parent)
 
         if isinstance(self.avatar, str):
             if self.avatar.startswith("http"):
                 self.avatar = await Sandbox._image(self.avatar)
         elif isinstance(self.avatar, Image.Image):
             pass
         else:
             raise TypeError(f"avatar must be a url, not {type(self.avatar)}") 
 
-        background = self.background.resize((1000, 333))
-        cut = Image.new("RGBA", (1000-(border_width*2), 333-(border_height*2)) , ImageColor.getcolor(card_colour, "RGB")+(senstivity,))
-        background.paste(cut, (border_width, border_height) ,cut)
+        if has_background:
+            background = self.background.resize(canvas_size)
+        else:
+            background = Image.new("RGBA", canvas_size, ImageColor.getcolor(background_colour, "RGB"))
+        if overlay is not None:
+            for x in overlay:
+                cut = Image.new("RGBA", x[0] , ImageColor.getcolor(x[2], "RGB")+(x[3],))
+                background.paste(cut, x[1] ,cut)
 
         avatar = self.avatar.resize((avatar_size, avatar_size))
 
         if avatar_frame == "square":
             mask = Image.new("RGBA", (avatar_size, avatar_size), "white")
         elif avatar_frame == "circle":
             mask = Image.open(path + "/assets/mask_circle.jpg").resize((avatar_size, avatar_size))
@@ -356,28 +403,38 @@
         if self.rank is not None:
             combined = "LEVEL: " + self._convert_number(self.level) + "       " + "RANK: " + str(self.rank)
         else:
             combined = "LEVEL: " + self._convert_number(self.level)
         draw.text(level_position, combined,font=ImageFont.truetype(fontname,level_font_size), fill=self.text_color,stroke_width=1,stroke_fill=(0, 0, 0))
         draw.text(username_position, self.username,font=ImageFont.truetype(fontname,username_font_size), fill=self.text_color,stroke_width=1,stroke_fill=(0, 0, 0))
 
+        if extra_text is not None and type(extra_text) == list:
+            for x in extra_text:
+                draw.text(x[1], x[0],font=ImageFont.truetype(fontname,x[2]), fill=(ImageColor.getcolor(x[3], "RGBA") if type(x[3]) != tuple else extra_text),stroke_width=1,stroke_fill=(0, 0, 0))
+
         exp = f"{self._convert_number(self.current_exp)}/{self._convert_number(self.max_exp)}"
         draw.text(exp_position, exp,font=ImageFont.truetype(fontname,exp_font_size), fill=self.text_color,stroke_width=1,stroke_fill=(0, 0, 0))
 
-        bar_exp = (self.current_exp/self.max_exp)*619
+        if bar_exp == None:
+            bar_exp = (self.current_exp/self.max_exp)*exp_bar_width
+            exp_bar_curve_custom = exp_bar_curve
+        else:
+            bar_exp = bar_exp*exp_bar_width
+
         if bar_exp <= 50:
-            bar_exp = 50  
+            bar_exp = 50
+            exp_bar_curve_custom = exp_bar_curve//2
 
-        im = Image.new("RGBA", (620, 51))
+        im = Image.new("RGBA", (exp_bar_width+1, exp_bar_height+1))
         draw = ImageDraw.Draw(im, "RGBA")
-        draw.rounded_rectangle((0, 0, 619, 50), 30, fill=(255,255,255,225))
+        draw.rounded_rectangle((0, 0, exp_bar_width, exp_bar_height), exp_bar_curve, fill=(exp_bar_background_colour if type(exp_bar_background_colour) == tuple else ImageColor.getcolor(exp_bar_background_colour, "RGBA")))
         if self.current_exp != 0:
-            draw.rounded_rectangle((0, 0, bar_exp, 50), 30, fill=self.bar_color)
-        
-        background.paste(im, (330, 235), im.convert("RGBA"))
+            draw.rounded_rectangle((0, 0, bar_exp, exp_bar_height), exp_bar_curve_custom, fill=self.bar_color)
+
+        background.paste(im, exp_bar_position, im.convert("RGBA"))
 
         image = BytesIO()
         if resize != 100:
             background = background.resize((int(background.size[0]*(resize/100)), int(background.size[1]*(resize/100))))
         background.save(image, 'PNG')
         image.seek(0)
         return image
```

### Comparing `discordlevelingcard-0.5.6/DiscordLevelingCard/tester.py` & `discordlevelingcard-0.6.0/DiscordLevelingCard/tester.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-from io import BytesIO
-from typing import Optional, Union
+from typing import Optional, Union, List
 
-from aiohttp import ClientSession
-from PIL import Image, ImageDraw, ImageFont
-from .error import InvalidImageUrl
-from pathlib import Path
+from PIL import Image
 from .card_settings import Settings
 from . import RankCard, Sandbox
 
 
 class Tester:
     """class to test Sandbox and RankCard locally
 
@@ -225,63 +221,72 @@
             rank=self.rank,
             cacheing=self.cacheing
         )
         card = await card.custom_card1(resize=resize,card_colour=card_colour)
         Image.open(card).save(f"{self.path}.png", "PNG")
         return
     
-    async def test_sandbox_card3(
+    async def test_sandbox_custom_canvas(
             self,
-            resize:int = 100,
 
-            senstivity:int = 200,
-            card_colour: str = "black",
+            has_background: bool = True,
+            background_colour: str = "black",
+
+            canvas_size: tuple = (1000, 333),
 
-            border_width: int = 25,
-            border_height: int = 25,
+            resize:int = 100,
+
+            overlay: Union[None, List] = [[(1000-50, 333-50),(25, 25), "black", 200]],
             
             avatar_frame: str = "curvedborder",
             avatar_size: int = 260,
             avatar_position: tuple = (53, 36),
             
             text_font: str = "levelfont.otf",
 
             username_position: tuple = (330,130),
             username_font_size: int = 50,
 
             level_position: tuple = (500,40),
             level_font_size: int = 50,
 
             exp_position: tuple = (775,130),
-            exp_font_size: int = 50
+            exp_font_size: int = 50,
+            bar_exp: Union[None, int] = None,
+
+            exp_bar_width: int = 619,
+            exp_bar_height: int = 50,
+            exp_bar_background_colour: Union[str, tuple] = "white",
+            exp_bar_position:tuple = (330, 235),
+            exp_bar_curve: int = 30,
+            extra_text: Union[List, None] = None
 
         )->None:
         """test card3 of Sandbox with this method
 
         Parameters
         ----------
+        has_background: :class:`bool`
+            Whether to use a background image or not. Default is True
+        
+        background_colour: :class:`str`
+            The colour of the background, only used if has_background is set to False. Default is black.
+        
+        canvas_size: :class:`tuple`
+            The size of the canvas. Default is (1000, 333)
+        
         resize: :class:`int`
             The percentage to resize the image to. Default is 100
-        
-        senstivity: :class:`int`
-            Change the transparency of the black box over the background image.
-                Default is 200.range - [0,255] 
-
-        border_width: :class:`int`
-            width of the border. default is 25
-
-        border_height: :class:`int`
-            height of the border. default is 25
+                    
+        overlay: :class:`list`
+            A list of overlays to be placed on the background. Default is [[(1000-50, 333-50),(25, 25), "black", 200]].
 
         avatar_frame: :class:`str`
             `circle` `square` `curvedborder` `hexagon` or path to a self created mask.
         
-        card_colour: :class:`str`
-            colour of the translucent overlay. Default is black.
-
         text_font: :class:`str`
             Default is `levelfont.otf` or path to a custom otf or ttf file type font.
 
         avatar_size: :class:`int`
             size of the avatar. Default is 260.
 
         avatar_position: :class:`tuple`
@@ -300,32 +305,61 @@
             font size of the level. Default is 50.
 
         exp_position: :class:`tuple`
             pixel position of the exp to be placed at. Default is (775,130)
         
         exp_font_size: :class:`int`
             font size of the exp. Default is 50.
+
+        exp_bar_width: :class:`int`
+            width of the exp bar. Default is 619.
+        
+        exp_bar_height: :class:`int`
+            height of the exp bar. Default is 50.
+        
+        exp_bar_background_colour: :class:`str`
+            colour of the exp bar. Default is white.
+        
+        exp_bar_position: :class:`tuple`
+            pixel position of the exp bar to be placed at. Default is (330, 235)
         
+        exp_bar_curve: :class:`int`
+            curve of the exp bar. Default is 30.
+
+        extra_text: :class:`list`
+            list of tuples containing text and position of the text to be placed on the card. Default is None. eg ["string", (x-position, y-position), font-size, "colour"]
+
+        exp_bar: :class:`int`
+            The calculated exp of the user. Default is None.
+        
+
         Attributes
         ----------
+        - `has_background`
+        - `background_colour`
+        - `canvas_size`
         - `resize`
-        - `senstivity`
-        - `border_width`
-        - `border_height`
+        - `overlay`
         - `avatar_frame`
-        - `card_colour`
         - `text_font`
         - `avatar_size`
         - `avatar_position`
         - `username_position`
         - `username_font_size`
         - `level_position`
         - `level_font_size`
         - `exp_position`
         - `exp_font_size`
+        - `exp_bar_width`
+        - `exp_bar_height`
+        - `exp_bar_background_colour`
+        - `exp_bar_position`
+        - `exp_bar_curve`
+        - `extra_text`
+        - `exp_bar`
         
         Returns
         -------
         returns nothing but saves a file in the current directory with the given name
         """
 
         card = Sandbox(
@@ -334,26 +368,34 @@
             level=self.level,
             username=self.username,
             current_exp=self.current_exp,
             max_exp=self.max_exp,
             rank=self.rank,
             cacheing=self.cacheing
         )
-        card = await card.custom_card3(
+        card = await card.custom_canvas(
+            has_background=has_background,
+            background_colour=background_colour,
+            canvas_size=canvas_size,
             resize=resize,
-            card_colour=card_colour,
-            senstivity=senstivity,
-            border_width=border_width,
-            border_height=border_height,
+            overlay=overlay,
             avatar_frame=avatar_frame,
             avatar_size=avatar_size,
             avatar_position=avatar_position,
             text_font=text_font,
             username_position=username_position,
             username_font_size=username_font_size,
             level_position=level_position,
             level_font_size=level_font_size,
             exp_position=exp_position,
-            exp_font_size=exp_font_size        
+            exp_font_size=exp_font_size,
+            exp_bar_width=exp_bar_width,
+            exp_bar_height=exp_bar_height,
+            exp_bar_background_colour=exp_bar_background_colour,
+            exp_bar_position=exp_bar_position,
+            exp_bar_curve=exp_bar_curve,
+            extra_text=extra_text,
+            exp_bar=bar_exp
+            
         )
         Image.open(card).save(f"{self.path}.png", "PNG")
         return
```

### Comparing `discordlevelingcard-0.5.6/LICENSE` & `discordlevelingcard-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.6/pyproject.toml` & `discordlevelingcard-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discordlevelingcard"
-version = "0.5.6"
+version = "0.6.0"
 readme = "README.md"
 description = "A library with leveling cards for your discord bot."
 repository = "https://github.com/krishsharma0413/DiscordLevelingCard"
 authors = ["Reset <krishsharma0413@gmail.com>"]
 license = "MIT"
 keywords = [
     "discord", "leveling", "card",
```

### Comparing `discordlevelingcard-0.5.6/setup.py` & `discordlevelingcard-0.6.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*'], 'DiscordLevelingCard': ['assets/*']}
 
 install_requires = \
 ['Pillow>=9.2.0,<10.0.0', 'aiohttp>=3.8.1,<4.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'discordlevelingcard',
-    'version': '0.5.6',
+    'version': '0.6.0',
     'description': 'A library with leveling cards for your discord bot.',
-    'long_description': '# DiscordLevelingCard\nA library with Rank cards for your discord bot.\n\n<h3 style="color:yellow;"> now create your own custom rank cards!</h3>\n\n<br>\n\n[![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)\n\n# card preview\n\n`card1`\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n\n`card2`\n![card2](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n\n`card3` *same as card2 but with background*\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n# installation\n\n`for pypi version`\n```sh\npip install discordlevelingcard\n```\n\n`for github developement version`\n```sh\npip install git+https://github.com/krishsharma0413/DiscordLevelingCard\n```\n\n# How To Use\n\nIf you don\'t provide `path` then the method will return `bytes` which can directly be used in discord.py/disnake/pycord/nextcord \'s `File class`.\n\n\n<br>\n\n\n# Example\n\n`since no path was provided, it returns bytes which can directly be used in discord.py and its fork\'s File class.`\n\n```py\nfrom disnake.ext import commands\nfrom DiscordLevelingCard import RankCard, Settings\nimport disnake\n\nclient = commands.Bot()\n# define background, bar_color, text_color at one place\ncard_settings = Settings(\n    background="url or path to background image",\n    text_color="white",\n    bar_color="#000000"\n)\n\n@client.slash_command(name="rank")\nasync def user_rank_card(ctx, user:disnake.Member):\n    await ctx.response.defer()\n    a = RankCard(\n        settings=card_settings,\n        avatar=user.display_avatar.url,\n        level=1,\n        current_exp=1,\n        max_exp=1,\n        username="cool username"\n    )\n    image = await a.card1()\n    await ctx.edit_original_message(file=disnake.File(image, filename="rank.png")) # providing filename is very important\n\n```\n\n<br>\n\n## Documentation\n\n\n<details>\n\n<summary> <span style="color:yellow">RankCard</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n## methods\n\n- `card1`\n- `card2`\n- `card3`\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">Sandbox</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    cacheing:bool = True,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n- `cacheing` - if set to `True` then it will cache the image and will not regenerate it again. (default is `True`)\n  \n\n## methods\n- `custom_card1`\n  \n</details>\n\n\n\n\n<details>\n\n<summary> <span style="color:yellow">Settings</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nSettings(\n    background: Union[PathLike, BufferedIOBase, str],\n    bar_color: Optional[str] = \'white\',\n    text_color: Optional[str] = \'white\',\n    background_color: Optional[str]= "#36393f"\n\n)\n```\n\n- `background` - background image url or file-object in `rb` mode.\n  - `4:1` aspect ratio recommended.\n\n- `bar_color` - color of the bar [example: "white" or "#000000"]\n\n- `text_color` - color of the text [example: "white" or "#000000"]\n\n- `background_color` - color of the background [example: "white" or "#000000"]\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card1</span> method</summary>\n\n\n```py\nRankCard.card1(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card2</span> method</summary>\n\n\n```py\nRankCard.card2(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card3</span> method</summary>\n\n\n```py\nRankCard.card3(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">custom_card1</span> method</summary>\n\n\n```py\nSandbox.custom_card1(card_colour:str = "black", resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n- `card_colour` : color of the card. (default is black)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n## examples\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/blue_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/white_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/black_card1.png)\n\n<br>\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">custom_card3</span> method</summary>\n\n\n```py\nSandbox.custom_card3(\n    resize:int = 100,\n\n    senstivity:int = 200,\n    card_colour: str = "black",\n\n    border_width: int = 25,\n    border_height: int = 25,\n    \n    avatar_frame: str = "curvedborder",\n    avatar_size: int = 260,\n    avatar_position: tuple = (53, 36),\n    \n    text_font: str = "levelfont.otf",\n\n    username_position: tuple = (330,130),\n    username_font_size: int = 50,\n\n    level_position: tuple = (500,40),\n    level_font_size: int = 50,\n\n    exp_position: tuple = (775,130),\n    exp_font_size: int = 50,\n\n)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n- `senstivity` : senstivity of the avatar frame. (default is 200)\n- `card_colour` : color of the card. (default is black)\n- `border_width` : width of the border. (default is 25)\n- `border_height` : height of the border. (default is 25)\n- `avatar_frame` : avatar frame. (default is "curvedborder")\n- `avatar_size` : size of the avatar. (default is 260)\n- `avatar_position` : position of the avatar. (default is (53, 36))\n- `text_font` : font of the text. (default is "levelfont.otf")\n- `username_position` : position of the username. (default is (330,130))\n- `username_font_size` : font size of the username. (default is 50)\n- `level_position` : position of the level. (default is (500,40))\n- `level_font_size` : font size of the level. (default is 50)\n- `exp_position` : position of the exp. (default is (775,130))\n- `exp_font_size` : font size of the exp. (default is 50)\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n## examples\n\n![custom_card3](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20example-1.png)\n\n![custom_card3](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20unholy%20example-2.png)\n\n<br>\n\n</details>\n\n\n<br><br>\n\nif you want to see changelog then click [here](https://github.com/krishsharma0413/DiscordLevelingCard/blob/main/CHANGELOG.md)\n\n<br><br>\nplease star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D\n',
+    'long_description': '# DiscordLevelingCard\nA library with Rank cards for your discord bot.\n\n<h3 style="color:yellow;"> now create your own custom rank cards!</h3>\n\n<br>\n\n[![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)\n\n# card preview\n\n`card1`\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n\n`card2`\n![card2](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n\n`card3` *same as card2 but with background*\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n# installation\n\n`for pypi version`\n```sh\npip install discordlevelingcard\n```\n\n`for github developement version`\n```sh\npip install git+https://github.com/krishsharma0413/DiscordLevelingCard\n```\n\n# How To Use\n\nIf you don\'t provide `path` then the method will return `bytes` which can directly be used in discord.py/disnake/pycord/nextcord \'s `File class`.\n\n\n<br>\n\n\n# Example\n\n`since no path was provided, it returns bytes which can directly be used in discord.py and its fork\'s File class.`\n\n```py\nfrom disnake.ext import commands\nfrom DiscordLevelingCard import RankCard, Settings\nimport disnake\n\nclient = commands.Bot()\n# define background, bar_color, text_color at one place\ncard_settings = Settings(\n    background="url or path to background image",\n    text_color="white",\n    bar_color="#000000"\n)\n\n@client.slash_command(name="rank")\nasync def user_rank_card(ctx, user:disnake.Member):\n    await ctx.response.defer()\n    a = RankCard(\n        settings=card_settings,\n        avatar=user.display_avatar.url,\n        level=1,\n        current_exp=1,\n        max_exp=1,\n        username="cool username"\n    )\n    image = await a.card1()\n    await ctx.edit_original_message(file=disnake.File(image, filename="rank.png")) # providing filename is very important\n\n```\n\n<br>\n\n## Documentation\n\n\n<details>\n\n<summary> <span style="color:yellow">RankCard</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n## methods\n\n- `card1`\n- `card2`\n- `card3`\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">Sandbox</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    cacheing:bool = True,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n- `cacheing` - if set to `True` then it will cache the image and will not regenerate it again. (default is `True`)\n  \n\n## methods\n- `custom_card1`\n  \n</details>\n\n\n\n\n<details>\n\n<summary> <span style="color:yellow">Settings</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nSettings(\n    background: Union[PathLike, BufferedIOBase, str],\n    bar_color: Optional[str] = \'white\',\n    text_color: Optional[str] = \'white\',\n    background_color: Optional[str]= "#36393f"\n\n)\n```\n\n- `background` - background image url or file-object in `rb` mode.\n  - `4:1` aspect ratio recommended.\n\n- `bar_color` - color of the bar [example: "white" or "#000000"]\n\n- `text_color` - color of the text [example: "white" or "#000000"]\n\n- `background_color` - color of the background [example: "white" or "#000000"]\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card1</span> method</summary>\n\n\n```py\nRankCard.card1(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card2</span> method</summary>\n\n\n```py\nRankCard.card2(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card3</span> method</summary>\n\n\n```py\nRankCard.card3(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">custom_card1</span> method</summary>\n\n\n```py\nSandbox.custom_card1(card_colour:str = "black", resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n- `card_colour` : color of the card. (default is black)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n## examples\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/blue_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/white_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/black_card1.png)\n\n<br>\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">custom_canvas</span> method</summary>\n\n\n```py\nSandbox.custom_canvas(\n    resize:int = 100,\n\n    senstivity:int = 200,\n    card_colour: str = "black",\n\n    border_width: int = 25,\n    border_height: int = 25,\n    \n    avatar_frame: str = "curvedborder",\n    avatar_size: int = 260,\n    avatar_position: tuple = (53, 36),\n    \n    text_font: str = "levelfont.otf",\n\n    username_position: tuple = (330,130),\n    username_font_size: int = 50,\n\n    level_position: tuple = (500,40),\n    level_font_size: int = 50,\n\n    exp_position: tuple = (775,130),\n    exp_font_size: int = 50,\n\n)\n```\n\n## attribute\n  - `has_background` : if set to `True` then it will add a background to the image. (default is `True`)\n  - `background_colour` : color of the background. (default is `black`)\n  - `canvas_size` : size of the canvas. (default is `(1000, 333)`)\n  - `resize` : resize the final image. (default is 100, treat it as a percentage.)\n  - `overlay` : A list of overlays to be placed on the background. (Default is `[[(1000-50, 333-50),(25, 25), "black", 200]]`.)\n  - `avatar_frame` : `circle` `square` `curvedborder` `hexagon` or path to a self created mask. (Default is `curvedborder`.)\n  - `text_font` : Default is `levelfont.otf` or path to a custom otf or ttf file type font.\n  - `avatar_size` : size of the avatar. (default is `260`)\n  - `avatar_position` : position of the avatar. (default is `(53, 36)`)\n  - `username_position` : position of the username. (default is `(330,130)`)\n  - `username_font_size` : font size of the username. (default is `50`)\n  - `level_position` : position of the level. (default is `(500,40)`)\n  - `level_font_size` : font size of the level. (default is `50`)\n  - `exp_position` : position of the exp. (default is `(775,130)`)\n  - `exp_font_size` : font size of the exp. (default is `50`)\n  - `exp_bar_width` : width of the exp bar. (default is `619`)\n  - `exp_bar_height` : height of the exp bar. (default is `50`)\n  - `exp_bar_background_colour` : color of the exp bar background. (default is `white`)\n  - `exp_bar_position` : position of the exp bar. (default is `(330, 235)`)\n  - `exp_bar_curve` : curve of the exp bar. (default is `30`)\n  - `extra_text` : A list of extra text to be placed on the image. (Default is `None`.)\n  - `exp_bar` : The calculated exp of the user. (Default is `None`.)\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n## examples\n\n![custom_canvas](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20example-1.png)\n\n![custom_canvas](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20unholy%20example-2.png)\n\n\nAn Example that i really loved was this one, here is the code for it as well. (you might have to tweak a lot to make it work for you though. )\n\n```py\nfrom DiscordLevelingCard import Sandbox, Settings\nimport asyncio\nfrom PIL import Image\n\nsetting = Settings(\n    background="./bg.jpg",\n    bar_color="green",\n    text_color="white")\n\nasync def main():\n    rank = Sandbox(\n        username="krishsharma0413",\n        level=1,\n        current_exp=10,\n        max_exp=400,\n        settings=setting,\n        avatar=Image.open("./avatarimg.png")\n    )\n    result = await rank.custom_canvas(\n        avatar_frame="square",\n        avatar_size=233,\n        avatar_position=(50, 50),\n        exp_bar_background_colour = "black",\n        exp_bar_height=50,\n        exp_bar_width=560,\n        exp_bar_curve=0,\n        exp_bar_position=(70, 400),\n        username_position=(320, 50),\n        level_position=(320, 225),\n        exp_position=(70, 330),\n        canvas_size=(700, 500),\n\n        overlay=[[(350, 233),(300, 50), "white", 100],\n                 [(600, 170),(50, 300), "white", 100]],\n\n        extra_text=[\n            ["bio-", (320, 110), 25, "white"],\n            ["this can very well be a bio", (320, 140), 25, "white"],\n            ["even mutiple lines!", (320, 170), 25, "white"],\n            ["if we remove bio- even more!", (320, 200), 25, "white"],\n            ]\n\n    )\n    \n    # you don\'t need this line if you are using this in discord.py\n    Image.open(result).save("result.png", "PNG")\n\n\nasyncio.run(main())\n```\n\nand this is how it looks :D\n\n![custom_canvas](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/extra%20canvas%20example.png)\n\n<br>\n\n</details>\n\n\n<br><br>\n\nif you want to see changelog then click [here](https://github.com/krishsharma0413/DiscordLevelingCard/blob/main/CHANGELOG.md)\n\n<br><br>\nplease star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D\n',
     'author': 'Reset',
     'author_email': 'krishsharma0413@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/krishsharma0413/DiscordLevelingCard',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `discordlevelingcard-0.5.6/PKG-INFO` & `discordlevelingcard-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordlevelingcard
-Version: 0.5.6
+Version: 0.6.0
 Summary: A library with leveling cards for your discord bot.
 Home-page: https://github.com/krishsharma0413/DiscordLevelingCard
 License: MIT
 Keywords: discord,leveling,card,image,discord.py,disnake,nextcord,rank,ranking,level,discord-bot,bot,discord-leveling,level-card,discord-leveling-card,discord-rank-card,sandbox,custom,custom-card
 Author: Reset
 Author-email: krishsharma0413@gmail.com
 Requires-Python: >=3.8,<4
@@ -321,19 +321,19 @@
 
 <br>
 
 </details>
 
 <details>
 
-<summary> <span style="color:yellow">custom_card3</span> method</summary>
+<summary> <span style="color:yellow">custom_canvas</span> method</summary>
 
 
 ```py
-Sandbox.custom_card3(
+Sandbox.custom_canvas(
     resize:int = 100,
 
     senstivity:int = 200,
     card_colour: str = "black",
 
     border_width: int = 25,
     border_height: int = 25,
@@ -353,39 +353,106 @@
     exp_position: tuple = (775,130),
     exp_font_size: int = 50,
 
 )
 ```
 
 ## attribute
-- `resize` : resize the final image. (default is 100, treat it as a percentage.)
-- `senstivity` : senstivity of the avatar frame. (default is 200)
-- `card_colour` : color of the card. (default is black)
-- `border_width` : width of the border. (default is 25)
-- `border_height` : height of the border. (default is 25)
-- `avatar_frame` : avatar frame. (default is "curvedborder")
-- `avatar_size` : size of the avatar. (default is 260)
-- `avatar_position` : position of the avatar. (default is (53, 36))
-- `text_font` : font of the text. (default is "levelfont.otf")
-- `username_position` : position of the username. (default is (330,130))
-- `username_font_size` : font size of the username. (default is 50)
-- `level_position` : position of the level. (default is (500,40))
-- `level_font_size` : font size of the level. (default is 50)
-- `exp_position` : position of the exp. (default is (775,130))
-- `exp_font_size` : font size of the exp. (default is 50)
+  - `has_background` : if set to `True` then it will add a background to the image. (default is `True`)
+  - `background_colour` : color of the background. (default is `black`)
+  - `canvas_size` : size of the canvas. (default is `(1000, 333)`)
+  - `resize` : resize the final image. (default is 100, treat it as a percentage.)
+  - `overlay` : A list of overlays to be placed on the background. (Default is `[[(1000-50, 333-50),(25, 25), "black", 200]]`.)
+  - `avatar_frame` : `circle` `square` `curvedborder` `hexagon` or path to a self created mask. (Default is `curvedborder`.)
+  - `text_font` : Default is `levelfont.otf` or path to a custom otf or ttf file type font.
+  - `avatar_size` : size of the avatar. (default is `260`)
+  - `avatar_position` : position of the avatar. (default is `(53, 36)`)
+  - `username_position` : position of the username. (default is `(330,130)`)
+  - `username_font_size` : font size of the username. (default is `50`)
+  - `level_position` : position of the level. (default is `(500,40)`)
+  - `level_font_size` : font size of the level. (default is `50`)
+  - `exp_position` : position of the exp. (default is `(775,130)`)
+  - `exp_font_size` : font size of the exp. (default is `50`)
+  - `exp_bar_width` : width of the exp bar. (default is `619`)
+  - `exp_bar_height` : height of the exp bar. (default is `50`)
+  - `exp_bar_background_colour` : color of the exp bar background. (default is `white`)
+  - `exp_bar_position` : position of the exp bar. (default is `(330, 235)`)
+  - `exp_bar_curve` : curve of the exp bar. (default is `30`)
+  - `extra_text` : A list of extra text to be placed on the image. (Default is `None`.)
+  - `exp_bar` : The calculated exp of the user. (Default is `None`.)
+
 
 ## returns 
 - `bytes` which can directly be used within `discord.File` class.
 
 
 ## examples
 
-![custom_card3](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20example-1.png)
+![custom_canvas](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20example-1.png)
+
+![custom_canvas](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20unholy%20example-2.png)
+
+
+An Example that i really loved was this one, here is the code for it as well. (you might have to tweak a lot to make it work for you though. )
+
+```py
+from DiscordLevelingCard import Sandbox, Settings
+import asyncio
+from PIL import Image
+
+setting = Settings(
+    background="./bg.jpg",
+    bar_color="green",
+    text_color="white")
+
+async def main():
+    rank = Sandbox(
+        username="krishsharma0413",
+        level=1,
+        current_exp=10,
+        max_exp=400,
+        settings=setting,
+        avatar=Image.open("./avatarimg.png")
+    )
+    result = await rank.custom_canvas(
+        avatar_frame="square",
+        avatar_size=233,
+        avatar_position=(50, 50),
+        exp_bar_background_colour = "black",
+        exp_bar_height=50,
+        exp_bar_width=560,
+        exp_bar_curve=0,
+        exp_bar_position=(70, 400),
+        username_position=(320, 50),
+        level_position=(320, 225),
+        exp_position=(70, 330),
+        canvas_size=(700, 500),
+
+        overlay=[[(350, 233),(300, 50), "white", 100],
+                 [(600, 170),(50, 300), "white", 100]],
+
+        extra_text=[
+            ["bio-", (320, 110), 25, "white"],
+            ["this can very well be a bio", (320, 140), 25, "white"],
+            ["even mutiple lines!", (320, 170), 25, "white"],
+            ["if we remove bio- even more!", (320, 200), 25, "white"],
+            ]
+
+    )
+    
+    # you don't need this line if you are using this in discord.py
+    Image.open(result).save("result.png", "PNG")
+
+
+asyncio.run(main())
+```
+
+and this is how it looks :D
 
-![custom_card3](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20unholy%20example-2.png)
+![custom_canvas](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/extra%20canvas%20example.png)
 
 <br>
 
 </details>
 
 
 <br><br>
```

