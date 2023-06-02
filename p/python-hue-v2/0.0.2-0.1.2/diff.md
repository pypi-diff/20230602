# Comparing `tmp/python_hue_v2-0.0.2.tar.gz` & `tmp/python_hue_v2-0.1.2.tar.gz`

## Comparing `python_hue_v2-0.0.2.tar` & `python_hue_v2-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/.idea/hue-v2.iml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/src/python_hue_v2/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/src/python_hue_v2/__init__.py
--rw-r--r--   0        0        0     4864 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/src/python_hue_v2/bridge.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/src/python_hue_v2/hue.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/src/python_hue_v2/light.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/src/python_hue_v2/mdns.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/src/python_hue_v2/scene.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/tests/test_connection.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/tests/test_object_convert.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/LICENSE
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/README.md
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 python_hue_v2-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/.idea/hue-v2.iml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/src/python_hue_v2/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/src/python_hue_v2/__init__.py
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/src/python_hue_v2/bridge.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/src/python_hue_v2/grouped_light.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/src/python_hue_v2/hue.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/src/python_hue_v2/light.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/src/python_hue_v2/mdns.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/src/python_hue_v2/scene.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/tests/test_connection.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/tests/test_object_convert.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/README.md
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 python_hue_v2-0.1.2/PKG-INFO
```

### Comparing `python_hue_v2-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `python_hue_v2-0.1.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `python_hue_v2-0.0.2/src/python_hue_v2/bridge.py` & `python_hue_v2-0.1.2/src/python_hue_v2/bridge.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 from typing import List, Union
 
 
 class Bridge:
     def __init__(self, ip_address: str, hue_application_key: str):
         self.ip_address = ip_address
         self.hue_application_key = hue_application_key
-        self.hue_application_key_str = 'hue-application-key'
+        self.hue_application_key_name = 'hue-application-key'
         # url
         self.base_url = f'https://{self.ip_address}/clip/v2/resource'
 
         self._light_category = 'light'
         self._scene_category = 'scene'
         self._room_category = 'room'
         self._zone_category = 'zone'
         self._bridge_home_category = 'bridge_home'
         self._grouped_light_category = 'grouped_light'
         self._device_category = 'device'
         self._bridge_category = 'bridge'
-
-        self.device_list: list = []
         # requests.Request.
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
     @staticmethod
     def _get_response_error(r_json: dict):
         return r_json['errors']
 
@@ -39,64 +37,64 @@
         if res['errors']:
             raise ConnectionError(res['errors'])
         else:
             return res['data']
 
     def _get_by_id(self, category: str, item_id: str) -> dict:
         url = f'{self.base_url}/{category}/{item_id}'
-        res = requests.get(url, headers={self.hue_application_key_str: self.hue_application_key}, verify=False).json()
+        res = requests.get(url, headers={self.hue_application_key_name: self.hue_application_key}, verify=False).json()
         return self._convert_to_data(res)[0]
 
     def _get(self, category: str) -> List[dict]:
         url = f'{self.base_url}/{category}'
-        res = requests.get(url, headers={self.hue_application_key_str: self.hue_application_key}, verify=False).json()
+        res = requests.get(url, headers={self.hue_application_key_name: self.hue_application_key}, verify=False).json()
         return self._convert_to_data(res)
 
     def _put_by_id(self, category: str, item_id: str, properties: dict) -> dict:
         url = f'{self.base_url}/{category}/{item_id}'
         res = requests.put(url, data=json.dumps(properties),
-                           headers={self.hue_application_key_str: self.hue_application_key},
+                           headers={self.hue_application_key_name: self.hue_application_key},
                            verify=False).json()
         return self._convert_to_data(res)[0]
 
     def _post(self, category: str, properties: dict) -> list:
         url = f'{self.base_url}/{category}'
         res = requests.post(url, data=json.dumps(properties),
-                            headers={self.hue_application_key_str: self.hue_application_key},
+                            headers={self.hue_application_key_name: self.hue_application_key},
                             verify=False).json()
         return self._convert_to_data(res)
 
     def _delete_by_id(self, category: str, item_id: str) -> list:
         url = f'{self.base_url}/{category}/{item_id}'
-        res = requests.delete(url, headers={self.hue_application_key_str: self.hue_application_key},
+        res = requests.delete(url, headers={self.hue_application_key_name: self.hue_application_key},
                               verify=False).json()
         return self._convert_to_data(res)
 
     def get_light(self, light_id: str) -> dict:
         return self._get_by_id(self._light_category, light_id)
 
     def get_lights(self) -> List[dict]:
         """
         Get all lights info in bridge
         :return:
         """
         return self._get(self._light_category)
 
-    def set_light(self, light_id_v2, light_property, key_value: dict):
-        data = {light_property: key_value}
+    def set_light(self, light_id_v2, light_property_name, property_value: dict):
+        data = {light_property_name: property_value}
         return self._put_by_id(self._light_category, light_id_v2, data)
 
     def get_scenes(self) -> List[dict]:
         return self._get(self._scene_category)
 
     def get_scene(self, scene_id) -> dict:
         return self._get_by_id(self._scene_category, scene_id)
 
-    def set_scene(self, scene_id, scene_property: str, data: Union[list, dict]):
-        return self._put_by_id(self._scene_category, scene_id, {scene_property: data})
+    def set_scene(self, scene_id, scene_property: str, property_value: Union[list, dict]):
+        return self._put_by_id(self._scene_category, scene_id, {scene_property: property_value})
 
     def create_scene(self, properties: dict) -> list:
         return self._post(self._scene_category, properties)
 
     def delete_scene(self, scene_id: str) -> list:
         return self._delete_by_id(self._scene_category, scene_id)
 
@@ -108,23 +106,39 @@
 
     def get_zones(self) -> List[dict]:
         return self._get(self._zone_category)
 
     def get_zone(self, zone_id: str) -> dict:
         return self._get_by_id(self._zone_category, zone_id)
 
+    def get_bridge_homes(self) -> List[dict]:
+        return self._get(self._bridge_category)
+
+    def get_bridge_home(self, bridge_home_id: str) -> dict:
+        return self._get_by_id(self._bridge_category, bridge_home_id)
+
+    def get_grouped_lights(self) -> List[dict]:
+        return self._get(self._grouped_light_category)
+
+    def get_grouped_light(self, grouped_light_id: str) -> dict:
+        return self._get_by_id(self._grouped_light_category, grouped_light_id)
+
+    def set_grouped_light_service(self, grouped_light_id: str, property_name: str, property_value: dict) -> dict:
+        return self._put_by_id(self._grouped_light_category, grouped_light_id,
+                               properties={property_name: property_value})
+
     def get_devices(self):
         return self._get(self._device_category)
 
     def get_device(self, device_id: str):
         return self._get_by_id(self._device_category, device_id)
 
     def get_bridge(self):
         return self._get(self._bridge_category)
 
-    def get_bridge_by_id(self, id_) -> dict:
+    def get_bridge_by_id(self, id_: str) -> dict:
         """
         Get bridge info by its id
         :param id_: https://developers.meethue.com/develop/hue-api-v2/api-reference/#resource_bridge__id__get
         :return: BridgeGet Info
         """
         return self._get_by_id(self._bridge_category, id_)
```

### Comparing `python_hue_v2-0.0.2/src/python_hue_v2/hue.py` & `python_hue_v2-0.1.2/src/python_hue_v2/hue.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import time
+
 from python_hue_v2.bridge import Bridge
 from python_hue_v2.light import Light
 from python_hue_v2.scene import Scene
+from python_hue_v2.grouped_light import GroupedLight
 from typing import List
 
 
 class Hue:
     def __init__(self, ip_address: str, hue_application_key: str):
         self.bridge = Bridge('ecb5fa8549cd.local', '7K-IbBzEV3wZoXkTlSh6HyLTALLFsYrxCjIcW1o9')
 
@@ -12,13 +15,24 @@
     def lights(self) -> List[Light]:
         return [Light(self.bridge, light_data['id']) for light_data in self.bridge.get_lights()]
 
     @property
     def scenes(self) -> List[Scene]:
         return [Scene(self.bridge, scene_data['id']) for scene_data in self.bridge.get_scenes()]
 
+    @property
+    def grouped_lights(self) -> List[GroupedLight]:
+        return [GroupedLight(self.bridge, grouped_light_data['id']) for grouped_light_data in
+                self.bridge.get_grouped_lights()]
+
 
 if __name__ == '__main__':
     hue = Hue('ecb5fa8549cd.local', '7K-IbBzEV3wZoXkTlSh6HyLTALLFsYrxCjIcW1o9')
-    # hue.get_device()
+    scenes = hue.scenes
+    for scene in scenes:
+        print(scene.data_dict)
+    scenes[2].recall(action='static')
     print()
-    hue.lights[0].on = False
+    time.sleep(1)
+    grouped_lights = hue.grouped_lights
+    grouped_lights[0].on = False
+    # hue.lights[0].on = False
```

### Comparing `python_hue_v2-0.0.2/src/python_hue_v2/light.py` & `python_hue_v2-0.1.2/src/python_hue_v2/light.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 from .bridge import Bridge
 
 
 class Light:
     def __init__(self, bridge: Bridge, light_id_v2: str):
         self.bridge = bridge
         self.light_id: str = light_id_v2
-        self._on: bool
 
     def _get(self) -> dict:
         return self.bridge.get_light(self.light_id)
 
-    def _set(self, light_property: str, key_value: dict) -> List[dict]:
-        return self.bridge.set_light(self.light_id, light_property, key_value)
+    def _set(self, light_property_name: str, property_value: dict) -> List[dict]:
+        return self.bridge.set_light(self.light_id, light_property_name, property_value)
 
     @property
-    def data(self) -> dict:
+    def data_dict(self) -> dict:
         return self._get()
 
     @property
-    def on(self):
+    def on(self) -> bool:
         data = self._get()
         return data['on']['on']
 
     @on.setter
     def on(self, value: bool):
         self._set('on', {'on': value})
```

### Comparing `python_hue_v2-0.0.2/src/python_hue_v2/mdns.py` & `python_hue_v2-0.1.2/src/python_hue_v2/mdns.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-0.0.2/src/python_hue_v2/scene.py` & `python_hue_v2-0.1.2/src/python_hue_v2/scene.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from typing import List, Union, Literal
 from .bridge import Bridge
 
 
 class SceneGet:
     """
     SceneGet Wrapper in https://developers.meethue.com/develop/hue-api-v2/api-reference/#resource_scene_get
     """
@@ -54,38 +54,46 @@
     def __init__(self, bridge: Bridge, scene_id_v2: str):
         self.bridge = bridge
         self.scene_id: str = scene_id_v2
 
     def _get(self) -> dict:
         return self.bridge.get_scene(self.scene_id)
 
-    def _set(self, scene_property: str, data: Union[list, dict]) -> List[dict]:
-        return self.bridge.set_scene(self.scene_id, scene_property, data)
+    def _set(self, scene_property_name: str, property_value: Union[list, dict]) -> List[dict]:
+        return self.bridge.set_scene(self.scene_id, scene_property_name, property_value)
 
     @property
     def data(self) -> SceneGet:
         return SceneGet(self._get())
-    
+
+    @property
+    def data_dict(self) -> dict:
+        """
+        Get raw properties by get
+        :return: One SceneGet data in properties. Because 1 id get 1 item. https://developers.meethue.com/develop/hue-api-v2/api-reference/#resource_scene__id__get
+        """
+        return self._get()
+
+    def recall(self, action: Literal['active', 'dynamic_palette', 'static']):
+        # {'status': 'active'} is failed
+        self._set('recall', {'action': action})
+
     @property
     def id(self) -> str:
         return self.scene_id
 
     @property
     def actions(self) -> list:
         return self._get()['actions']
 
     @actions.setter
     def actions(self, action_items: List[dict]):
         self._set('actions', action_items)
 
     @property
-    def recall(self) -> dict:
-        return self._get()['recall']
-
-    @property
     def meta_data(self) -> dict:
         return self._get()['metadata']
 
     @property
     def group(self) -> dict:
         return self._get()['group']
```

### Comparing `python_hue_v2-0.0.2/tests/test_connection.py` & `python_hue_v2-0.1.2/tests/test_connection.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,7 +30,20 @@
     assert type(hue.lights[0].color_xy) is dict
     assert type(hue.lights[0].color_xy['x']) is float
     assert type(hue.lights[0].color_xy['y']) is float
 
 
 def test_scenes():
     assert hue.scenes[0].type == 'scene'
+
+
+def test_grouped_light_type():
+    assert hue.grouped_lights[0].type == 'grouped_light'
+
+
+def test_grouped_light_brightness():
+    assert type(hue.grouped_lights[0].brightness) == float
+    hue.grouped_lights[0].on = True
+    hue.grouped_lights[0].brightness = 70.0
+    # Rounding error
+    assert hue.grouped_lights[0].brightness - 70.0 < 1
+    hue.grouped_lights[0].on = False
```

### Comparing `python_hue_v2-0.0.2/.gitignore` & `python_hue_v2-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `python_hue_v2-0.0.2/LICENSE` & `python_hue_v2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_hue_v2-0.0.2/pyproject.toml` & `python_hue_v2-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_hue_v2-0.0.2/PKG-INFO` & `python_hue_v2-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hue-v2
-Version: 0.0.2
+Version: 0.1.2
 Summary: A python library to control the Philips Hue lighting system.
 Project-URL: Documentation, https://github.com/FengChendian/python-hue-v2#readme
 Project-URL: Issues, https://github.com/FengChendian/python-hue-v2/issues
 Project-URL: Source, https://github.com/FengChendian/python-hue-v2
 Author-email: Yichen Zhao <njuzhaoyichen@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -24,16 +24,14 @@
 
 Python library to control the Philips Hue lighting system for Hue-V2 API.
 
 ## Features
 
 - Design for Hue API 2.0
 
-## Usage
-
 ## High Level Control
 
 ### Simple Example
 
 ```python
 import time
 from python_hue_v2 import Hue, BridgeFinder
@@ -48,8 +46,56 @@
 
 lights = hue.lights
 
 for light in lights:
     print(light.on)
     light.on = True
     light.brightness = 80.0
-```
+```
+### Scenes
+You can get scenes from hue bridge.
+```python
+from python_hue_v2 import Hue
+
+hue = Hue('bridge-ip', 'app-key')
+
+scenes = hue.scenes
+for scene in scenes:
+    print(scene.id)
+    print(scene.data_dict)
+```
+Recall scene using `active`, `dynamic_palette`, `static`.
+```python
+scene = scenes[0]
+scene.recall(action='active')
+```
+
+### Grouped Light
+Get Lights from hue.
+```python
+from python_hue_v2 import Hue
+
+hue = Hue('bridge-ip', 'app-key')
+grouped_lights = hue.grouped_lights
+
+for group in grouped_lights:
+    print(group.type)
+```
+
+## Low Level Control
+Also, you can use basic function in bridge class.
+```python
+import time
+from python_hue_v2 import Hue
+
+# or hue = Hue('ip address','app-key')
+hue = Hue('host_name', 'hue app key')  # create Hue instance
+bridge = hue.bridge
+
+bridge.get_lights()
+bridge.set_light('id', light_property_name='on', property_value={'on': True})
+
+bridge.get_zones()
+```
+## TODO
+
+- Zones, Rooms Control Class
```

