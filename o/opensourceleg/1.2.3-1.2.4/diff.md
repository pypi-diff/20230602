# Comparing `tmp/opensourceleg-1.2.3.tar.gz` & `tmp/opensourceleg-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-1.2.3.tar", max compression
+gzip compressed data, was "opensourceleg-1.2.4.tar", max compression
```

## Comparing `opensourceleg-1.2.3.tar` & `opensourceleg-1.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.3/LICENSE
--rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.3/README.md
--rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.3/opensourceleg/__init__.py
--rw-r--r--   0        0        0    21701 2023-06-02 15:30:09.743386 opensourceleg-1.2.3/opensourceleg/actuators.py
--rw-r--r--   0        0        0     2277 2023-06-01 22:39:19.258650 opensourceleg-1.2.3/opensourceleg/constants.py
--rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.2.3/opensourceleg/control.py
--rw-r--r--   0        0        0     4299 2023-06-02 06:57:31.927981 opensourceleg-1.2.3/opensourceleg/demo.py
--rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.3/opensourceleg/example.py
--rw-r--r--   0        0        0    10632 2023-06-01 21:48:32.759868 opensourceleg-1.2.3/opensourceleg/joints.py
--rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.3/opensourceleg/knee_encoder_map.npy
--rw-r--r--   0        0        0     8520 2023-06-01 22:39:19.421227 opensourceleg-1.2.3/opensourceleg/loadcell.py
--rw-r--r--   0        0        0     3799 2023-06-02 05:24:50.983197 opensourceleg-1.2.3/opensourceleg/logger.py
--rw-r--r--   0        0        0    15185 2023-06-02 15:14:01.350639 opensourceleg-1.2.3/opensourceleg/osl.py
--rw-r--r--   0        0        0    10384 2023-06-02 06:57:32.045778 opensourceleg-1.2.3/opensourceleg/state_machine.py
--rw-r--r--   0        0        0     6333 2023-06-02 14:52:19.367780 opensourceleg-1.2.3/opensourceleg/thermal.py
--rw-r--r--   0        0        0    21057 2023-06-01 22:39:19.630121 opensourceleg-1.2.3/opensourceleg/tui.py
--rw-r--r--   0        0        0     3531 2023-06-02 15:11:21.047386 opensourceleg-1.2.3/opensourceleg/units.py
--rw-r--r--   0        0        0    11590 2023-06-02 04:54:05.760995 opensourceleg-1.2.3/opensourceleg/utilities.py
--rw-r--r--   0        0        0     3668 2023-06-02 15:30:30.733471 opensourceleg-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.4/LICENSE
+-rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.4/README.md
+-rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.4/opensourceleg/__init__.py
+-rw-r--r--   0        0        0    22445 2023-06-02 20:45:59.012884 opensourceleg-1.2.4/opensourceleg/actuators.py
+-rw-r--r--   0        0        0     2283 2023-06-02 18:09:03.466245 opensourceleg-1.2.4/opensourceleg/constants.py
+-rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.2.4/opensourceleg/control.py
+-rw-r--r--   0        0        0     4259 2023-06-02 20:50:04.529275 opensourceleg-1.2.4/opensourceleg/demo.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.4/opensourceleg/example.py
+-rw-r--r--   0        0        0    11210 2023-06-02 20:45:59.013945 opensourceleg-1.2.4/opensourceleg/joints.py
+-rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.4/opensourceleg/knee_encoder_map.npy
+-rw-r--r--   0        0        0     8515 2023-06-02 20:45:59.014215 opensourceleg-1.2.4/opensourceleg/loadcell.py
+-rw-r--r--   0        0        0     3799 2023-06-02 05:24:50.983197 opensourceleg-1.2.4/opensourceleg/logger.py
+-rw-r--r--   0        0        0    15026 2023-06-02 20:53:49.594477 opensourceleg-1.2.4/opensourceleg/osl.py
+-rw-r--r--   0        0        0    10776 2023-06-02 20:50:04.631436 opensourceleg-1.2.4/opensourceleg/state_machine.py
+-rw-r--r--   0        0        0     6361 2023-06-02 18:52:35.890633 opensourceleg-1.2.4/opensourceleg/thermal.py
+-rw-r--r--   0        0        0    21057 2023-06-01 22:39:19.630121 opensourceleg-1.2.4/opensourceleg/tui.py
+-rw-r--r--   0        0        0     4331 2023-06-02 18:32:11.184018 opensourceleg-1.2.4/opensourceleg/units.py
+-rw-r--r--   0        0        0    11590 2023-06-02 04:54:05.760995 opensourceleg-1.2.4/opensourceleg/utilities.py
+-rw-r--r--   0        0        0     3668 2023-06-02 20:56:08.479891 opensourceleg-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.4/PKG-INFO
```

### Comparing `opensourceleg-1.2.3/LICENSE` & `opensourceleg-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.3/README.md` & `opensourceleg-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.3/opensourceleg/actuators.py` & `opensourceleg-1.2.4/opensourceleg/actuators.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     def _entry(self) -> None:
         self._device._log.debug(msg=f"[Actpack] Entering Voltage mode.")
 
     def _exit(self) -> None:
         self._device._log.debug(msg=f"[Actpack] Exiting Voltage mode.")
         self._set_voltage(voltage=0)
-        time.sleep(secs=0.1)
+        time.sleep(0.1)
 
     def _set_voltage(self, voltage: int) -> None:
         self._device.send_motor_command(
             ctrl_mode=self.mode,
             value=voltage,
         )
 
@@ -139,15 +139,15 @@
             self._set_gains()
 
         self._set_current(current=0)
 
     def _exit(self) -> None:
         self._device._log.debug(msg=f"[Actpack] Exiting Current mode.")
         self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
-        time.sleep(secs=1 / self._device.frequency)
+        time.sleep(1 / self._device.frequency)
 
     def _set_gains(
         self,
         kp: int = DEFAULT_CURRENT_GAINS.kp,
         ki: int = DEFAULT_CURRENT_GAINS.ki,
         ff: int = DEFAULT_CURRENT_GAINS.ff,
     ) -> None:
@@ -155,15 +155,15 @@
         assert 0 <= kp <= 80, "kp must be between 0 and 80"
         assert 0 <= ki <= 800, "ki must be between 0 and 800"
         assert 0 <= ff <= 128, "ff must be between 0 and 128"
 
         self._device.set_gains(kp=kp, ki=ki, kd=0, k=0, b=0, ff=ff)
         self._has_gains = True
 
-        time.sleep(secs=0.1)
+        time.sleep(0.1)
 
     def _set_current(self, current: int) -> None:
         """Sets the Q-axis current of the motor
 
         Args:
             current (int): _description_
         """
@@ -193,15 +193,15 @@
                 / Constants.RAD_PER_COUNT
             )
         )
 
     def _exit(self) -> None:
         self._device._log.debug(msg=f"[Actpack] Exiting Position mode.")
         self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
-        time.sleep(secs=0.1)
+        time.sleep(0.1)
 
     def _set_gains(
         self,
         kp: int = DEFAULT_POSITION_GAINS.kp,
         ki: int = DEFAULT_POSITION_GAINS.ki,
         kd: int = DEFAULT_POSITION_GAINS.kd,
     ) -> None:
@@ -209,15 +209,15 @@
         assert 0 <= kp <= 1000, "kp must be between 0 and 1000"
         assert 0 <= ki <= 1000, "ki must be between 0 and 1000"
         assert 0 <= kd <= 1000, "kd must be between 0 and 1000"
 
         self._device.set_gains(kp=kp, ki=ki, kd=kd, k=0, b=0, ff=0)
         self._has_gains = True
 
-        time.sleep(secs=1 / self._device.frequency)
+        time.sleep(1 / self._device.frequency)
 
     def _set_motor_position(self, counts: int) -> None:
         """Sets the motor position
 
         Args:
             counts (int): position in counts
         """
@@ -246,15 +246,15 @@
                 / Constants.RAD_PER_COUNT
             )
         )
 
     def _exit(self) -> None:
         self._device._log.debug(msg=f"[Actpack] Exiting Impedance mode.")
         self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
-        time.sleep(secs=1 / self._device.frequency)
+        time.sleep(1 / self._device.frequency)
 
     def _set_motor_position(self, counts: int) -> None:
         """Sets the motor position
 
         Args:
             counts (int): position in counts
         """
@@ -279,15 +279,15 @@
         assert 0 <= B, "B must be greater than 0"
 
         self._device.set_gains(
             kp=int(kp), ki=int(ki), kd=int(0), k=int(K), b=int(B), ff=int(ff)
         )
         self._has_gains = True
 
-        time.sleep(secs=1 / self._device.frequency)
+        time.sleep(1 / self._device.frequency)
 
 
 class DephyActpack(Device):
     """Class for the Dephy Actpack
 
     Args:
         Device (_type_): _description_
@@ -332,16 +332,21 @@
         self._log: Logger = logger
         self._state = None
         self._units: UnitsDefinition = units if units else DEFAULT_UNITS
 
         self._motor_zero_position = 0.0
         self._joint_zero_position = 0.0
 
-        self._thermal_model: ThermalModel = ThermalModel(temp_limit_windings=80, soft_border_C_windings=10, temp_limit_case=70, soft_border_C_case=10)
-        
+        self._thermal_model: ThermalModel = ThermalModel(
+            temp_limit_windings=80,
+            soft_border_C_windings=10,
+            temp_limit_case=70,
+            soft_border_C_case=10,
+        )
+
         self._modes: dict[str, ActpackMode] = {
             "voltage": VoltageMode(device=self),
             "position": PositionMode(device=self),
             "current": CurrentMode(device=self),
             "impedance": ImpedanceMode(device=self),
         }
 
@@ -357,30 +362,34 @@
         except OSError as e:
             print("\n")
             self._log.error(
                 msg=f"Need admin previleges to open the port '{self.port}'. \n\nPlease run the script with 'sudo' command or add the user to the dialout group.\n"
             )
             os._exit(status=1)
 
-        time.sleep(secs=0.1)
+        time.sleep(0.1)
         self._data = self.read()
         self._mode.enter()
 
     def stop(self) -> None:
         self.set_mode(mode="voltage")
         self.set_voltage(value=0)
 
-        time.sleep(secs=0.1)
+        time.sleep(0.1)
         self.close()
 
     def update(self) -> None:
         if self.is_streaming:
             self._data = self.read()
-            self._thermal_model.T_c = self.temperature
-            self._thermal_model.update(dt=(1/self._frequency), motor_current=self.motor_current)
+            self._thermal_model.T_c = self._units.convert_to_default_units(
+                value=self.case_temperature, attribute="temperature"
+            )
+            self._thermal_model.update(
+                dt=(1 / self._frequency), motor_current=self.motor_current
+            )
         else:
             self._log.warning(
                 msg=f"[Actpack] Please open() the device before streaming data."
             )
 
     def set_mode(self, mode: str) -> None:
         if mode in self._modes:
@@ -550,119 +559,132 @@
         return self._motor_zero_position
 
     @property
     def joint_zero_position(self) -> float:
         return self._joint_zero_position
 
     @property
-    def battery_voltage(self):
+    def battery_voltage(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
                 value=self._data.batt_volt,
                 attribute="voltage",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def batter_current(self):
+    def batter_current(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
                 value=self._data.batt_curr,
                 attribute="current",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def motor_voltage(self):
+    def motor_voltage(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
                 value=self._data.mot_volt,
                 attribute="voltage",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def motor_current(self):
+    def motor_current(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
                 value=self._data.mot_cur,
                 attribute="current",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def motor_torque(self):
+    def motor_torque(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
                 value=self._data.mot_cur * Constants.NM_PER_MILLIAMP,
                 attribute="torque",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def motor_position(self):
+    def motor_position(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
                 value=int(self._data.mot_ang) * Constants.RAD_PER_COUNT,
                 attribute="position",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def motor_velocity(self):
+    def motor_velocity(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
                 value=int(self._data.mot_vel) * Constants.RAD_PER_COUNT,
                 attribute="velocity",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def motor_acceleration(self):
+    def motor_acceleration(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
                 value=self._data.mot_acc,
                 attribute="acceleration",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def joint_position(self):
+    def joint_position(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
                 value=self._data.ank_ang * Constants.RAD_PER_COUNT,
                 attribute="position",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def joint_velocity(self):
+    def joint_velocity(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
                 value=self._data.ank_vel * Constants.RAD_PER_COUNT,
                 attribute="velocity",
             )
         else:
-            return 0
+            return 0.0
+
+    @property
+    def case_temperature(self) -> float:
+        if self._data is not None:
+            return self._units.convert_from_default_units(
+                value=self._data.temperature,
+                attribute="temperature",
+            )
+        else:
+            return 0.0
 
     @property
-    def temperature(self):
+    def winding_temperature(self) -> float:
         if self._data is not None:
-            return self._data.temperature
+            return self._units.convert_from_default_units(
+                value=self._thermal_model.T_w,
+                attribute="temperature",
+            )
         else:
-            return 0
+            return 0.0
 
     @property
     def genvars(self):
         if self._data is not None:
             return np.array(
                 object=[
                     self._data.genvar_0,
@@ -673,65 +695,65 @@
                     self._data.genvar_5,
                 ]
             )
         else:
             return np.zeros(shape=6)
 
     @property
-    def acc_x(self):
+    def accelx(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.acc_x * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                value=self._data.accelx * Constants.M_PER_SEC_SQUARED_ACCLSB,
                 attribute="gravity",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def acc_y(self):
+    def accely(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.acc_y * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                value=self._data.accely * Constants.M_PER_SEC_SQUARED_ACCLSB,
                 attribute="gravity",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def acc_z(self):
+    def accelz(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.acc_z * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                value=self._data.accelz * Constants.M_PER_SEC_SQUARED_ACCLSB,
                 attribute="gravity",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def gyro_x(self):
+    def gyrox(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.gyro_x * Constants.RAD_PER_SEC_GYROLSB,
+                value=self._data.gyrox * Constants.RAD_PER_SEC_GYROLSB,
                 attribute="velocity",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def gyro_y(self):
+    def gyroy(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.gyro_y * Constants.RAD_PER_SEC_GYROLSB,
+                value=self._data.gyroy * Constants.RAD_PER_SEC_GYROLSB,
                 attribute="velocity",
             )
         else:
-            return 0
+            return 0.0
 
     @property
-    def gyro_z(self):
+    def gyroz(self) -> float:
         if self._data is not None:
             return self._units.convert_from_default_units(
-                value=self._data.gyro_z * Constants.RAD_PER_SEC_GYROLSB,
+                value=self._data.gyroz * Constants.RAD_PER_SEC_GYROLSB,
                 attribute="velocity",
             )
         else:
-            return 0
+            return 0.0
```

### Comparing `opensourceleg-1.2.3/opensourceleg/constants.py` & `opensourceleg-1.2.4/opensourceleg/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     IMPEDANCE_A = 0.00028444
     IMPEDANCE_C = 0.0007812
 
     NM_PER_RAD_TO_K: float = RAD_PER_COUNT / IMPEDANCE_C * 1e3 / NM_PER_AMP
     NM_S_PER_RAD_TO_B: float = RAD_PER_DEG / IMPEDANCE_A * 1e3 / NM_PER_AMP
 
-    MAX_CURRENT: float = 22000
+    MAX_CASE_TEMPERATURE: float = 80
 
     LOADCELL_MATRIX = np.array(
         [
             (-38.72600, -1817.74700, 9.84900, 43.37400, -44.54000, 1824.67000),
             (-8.61600, 1041.14900, 18.86100, -2098.82200, 31.79400, 1058.6230),
             (
                 -1047.16800,
```

### Comparing `opensourceleg-1.2.3/opensourceleg/control.py` & `opensourceleg-1.2.4/opensourceleg/control.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.3/opensourceleg/demo.py` & `opensourceleg-1.2.4/opensourceleg/demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def estance_to_lstance(osl: OpenSourceLeg) -> bool:
     """
     Transition from early stance to late stance when the loadcell
     reads a force greater than a threshold.
     """
-    assert osl.loadcell is not None
-    if osl.loadcell.fz < -0.0167 * BODY_WEIGHT:
+    assert osl is not None
+    if osl.loadcell.fz < -1.25:  # type: ignore
         return True
     else:
         return False
 
 
 def lstance_to_eswing(osl: OpenSourceLeg) -> bool:
     """
     Transition from late stance to early swing when the loadcell
     reads a force less than a threshold.
     """
     assert osl.loadcell is not None
-    if osl.loadcell.fz > -0.00267 * BODY_WEIGHT:
+    if osl.loadcell.fz > 0.0:
         return True
     else:
         return False
 
 
 def eswing_to_lswing(osl: OpenSourceLeg) -> bool:
     """
@@ -79,27 +79,27 @@
         dephy_mode=False,
     )
 
     osl.add_state_machine()
 
     early_stance = State(name="e_stance")
     early_stance.set_knee_impedance_paramters(theta=5, k=130, b=450)
-    early_stance.is_knee_active = True
+    early_stance.make_knee_active()
 
     late_stance = State(name="l_stance")
     late_stance.set_knee_impedance_paramters(theta=5, k=175, b=200)
-    late_stance.is_knee_active = True
+    late_stance.make_knee_active()
 
     early_swing = State(name="e_swing")
     early_swing.set_knee_impedance_paramters(theta=62, k=40, b=40)
-    early_swing.is_knee_active = True
+    early_swing.make_knee_active()
 
     late_swing = State(name="l_swing")
     late_swing.set_knee_impedance_paramters(theta=30, k=100, b=200)
-    late_swing.is_knee_active = True
+    late_swing.make_knee_active()
 
     foot_flat = Event(name="foot_flat")
     heel_off = Event(name="heel_off")
     toe_off = Event(name="toe_off")
     pre_heel_strike = Event(name="pre_heel_strike")
     heel_strike = Event(name="heel_strike")
     misc = Event(name="misc")
```

### Comparing `opensourceleg-1.2.3/opensourceleg/joints.py` & `opensourceleg-1.2.4/opensourceleg/joints.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         self._motor_current_sp = 0.0
         self._motor_position_sp = 0.0
 
         self._stiffness_sp: int = 200
         self._damping_sp: int = 400
         self._equilibrium_position_sp = 0.0
 
+        self._max_temperature: float = Constants.MAX_CASE_TEMPERATURE
+
         self._control_mode_sp: str = "voltage"
 
         if "knee" in name.lower() or "ankle" in name.lower():
             self._name: str = name
         else:
             self._log.warning(msg=f"Invalid joint name: {name}")
             return
@@ -80,20 +82,20 @@
 
         self.set_mode(mode="voltage")
         self.set_voltage(value=-1 * homing_voltage)  # mV, negative for counterclockwise
 
         _motor_encoder_array = []
         _joint_encoder_array = []
 
-        time.sleep(secs=0.1)
+        time.sleep(0.1)
 
         try:
             while is_homing:
                 self.update()
-                time.sleep(secs=1 / homing_frequency)
+                time.sleep(1 / homing_frequency)
 
                 _motor_encoder_array.append(self.motor_position)
                 _joint_encoder_array.append(self.joint_position)
 
                 if (
                     abs(self.output_velocity) <= VELOCITY_THRESHOLD
                     or abs(self.motor_current) >= CURRENT_THRESHOLD
@@ -105,15 +107,15 @@
             self.set_voltage(value=0)
             self._log.warning(msg="Homing interrupted.")
             return
 
         _motor_zero_pos = self.motor_position
         _joint_zero_pos = self.joint_position
 
-        time.sleep(secs=0.1)
+        time.sleep(0.1)
 
         if np.std(_motor_encoder_array) < 1e-6:
             self._log.warning(
                 msg=f"[{self._name}] Motor encoder not working. Please check the wiring."
             )
             return
 
@@ -162,19 +164,19 @@
             self._log.warning(
                 msg=f"[{self._name}] Please home the joint before making the encoder map."
             )
             return
 
         self.set_mode(mode="current")
         self.set_current_gains()
-        time.sleep(secs=0.1)
+        time.sleep(0.1)
         self.set_current_gains()
 
         self.set_output_torque(torque=0.0)
-        time.sleep(secs=0.1)
+        time.sleep(0.1)
         self.set_output_torque(torque=0.0)
 
         _joint_position_array = []
         _output_position_array = []
 
         self._log.info(
             msg=f"[{self._name}] Please manually move the joint numerous times \
@@ -186,15 +188,15 @@
 
         try:
             while time.time() - _start_time < 10:
                 self.update()
                 _joint_position_array.append(self.joint_position)
                 _output_position_array.append(self.output_position)
 
-                time.sleep(secs=1 / self.frequency)
+                time.sleep(1 / self.frequency)
 
         except KeyboardInterrupt:
             self._log.warning(msg="Encoder map interrupted.")
             return
 
         self._log.info(msg=f"[{self._name}] You may now stop moving the joint.")
 
@@ -204,14 +206,25 @@
         _coeffs = _beta[0]
 
         self._encoder_map = np.polynomial.polynomial.Polynomial(coef=_coeffs)
 
         np.save(file=f"./{self._name}_encoder_map.npy", arr=_coeffs)
         self._log.info(msg=f"[{self._name}] Encoder map saved.")
 
+    def set_max_temperature(self, temperature: float) -> None:
+        """
+        Set the maximum temperature of the motor.
+
+        Args:
+            temperature (float): temperature in degrees Celsius
+        """
+        self._max_temperature = self._units.convert_to_default_units(
+            value=temperature, attribute="temperature"
+        )
+
     def set_output_torque(self, torque: float) -> None:
         """
         Set the output torque of the joint.
         This is the torque that is applied to the joint, not the motor.
 
         Args:
             torque (float): torque in user-defined units
@@ -300,14 +313,20 @@
         return self._name
 
     @property
     def gear_ratio(self) -> float:
         return self._gear_ratio
 
     @property
+    def max_temperature(self) -> float:
+        return self._units.convert_from_default_units(
+            value=self._max_temperature, attribute="temperature"
+        )
+
+    @property
     def is_homed(self) -> bool:
         return self._is_homed
 
     @property
     def encoder_map(self):
         return self._encoder_map
```

### Comparing `opensourceleg-1.2.3/opensourceleg/loadcell.py` & `opensourceleg-1.2.4/opensourceleg/loadcell.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     MEM_R_CH6_H = 18
     MEM_R_CH6_L = 19
 
     def __init__(self, bus, I2C_addr=0x66) -> None:
         """Create a strainamp object, to talk over I2C"""
         # self._I2CMan = I2CManager(bus)
         self._SMBus = SMBus(bus=bus)
-        time.sleep(secs=1)
+        time.sleep(1)
         self.bus = bus
         self.addr = I2C_addr
         self.genvars = np.zeros((3, 6))
         self.indx = 0
         self.is_streaming = True
         self.data = []
         self.failed_reads = 0
```

### Comparing `opensourceleg-1.2.3/opensourceleg/logger.py` & `opensourceleg-1.2.4/opensourceleg/logger.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.3/opensourceleg/osl.py` & `opensourceleg-1.2.4/opensourceleg/osl.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,39 +33,35 @@
         if OpenSourceLeg._instance is None:
             OpenSourceLeg()
         return OpenSourceLeg._instance
 
     def __init__(
         self,
         frequency: int = 200,
-        current_limit: float = Constants.MAX_CURRENT,
         file_name: str = "./osl.log",
     ) -> None:
         """
         Initialize the OSL class.
 
         Parameters
         ----------
         frequency : int, optional
             The frequency of the control loop, by default 200
-        current_limit : float, optional
-            The current limit of the motor in mA, by default 8000
         file_name : str, optional
             The name of the log file, by default "./osl.log"
         """
 
         self._frequency: int = frequency
 
         self._has_knee: bool = False
         self._has_ankle: bool = False
         self._has_loadcell: bool = False
         self._has_tui: bool = False
         self._has_sm: bool = False
 
-        self._current_limit: float = current_limit
         self._set_state_machine_parameters: bool = False
 
         self._knee: Joint = None  # type: ignore
         self._ankle: Joint = None  # type: ignore
         self._loadcell: Loadcell = None  # type: ignore
 
         self.log = Logger(
@@ -261,24 +257,28 @@
 
     def update(
         self,
     ) -> None:
         if self.has_knee:
             self._knee.update()
 
-            if self.knee.motor_current > self.current_limit:  # type: ignore
-                self.log.warn(msg="[KNEE] Current limit reached. Stopping motor.")
+            if self.knee.case_temperature > self.knee.max_temperature:  # type: ignore
+                self.log.warn(
+                    msg="[KNEE] Thermal limit {self.knee.max_temperature} reached. Stopping motor."
+                )
                 self.__exit__(type=None, value=None, tb=None)
                 exit()
 
         if self.has_ankle:
             self._ankle.update()
 
-            if self.ankle.motor_current > self.current_limit:  # type: ignore
-                self.log.warn("[ANKLE] Current limit () reached. Stopping motor.")
+            if self.ankle.case_temperature > self.ankle.max_temperature:  # type: ignore
+                self.log.warn(
+                    msg="[ANKLE] Thermal limit {self.ankle.max_temperature} reached. Stopping motor."
+                )
                 self.__exit__(type=None, value=None, tb=None)
                 exit()
 
         if self.has_loadcell:
             self._loadcell.update()
 
         if self.has_state_machine:
@@ -317,15 +317,15 @@
         set_state_machine_parameters : bool, optional
             Whether to set the joint impedance gains and equilibrium angles to the current state's values, by default False
         """
 
         self._set_state_machine_parameters = set_state_machine_parameters
         self.update()
 
-        time.sleep(secs=0.1)
+        time.sleep(0.1)
 
         if not self.has_tui:
             self.update()
 
         else:
             self.tui.add_update_callback(callback=self.update)  # type: ignore
             self.tui.run()  # type: ignore
@@ -424,21 +424,21 @@
     def reset(self) -> None:
         self.log.debug(msg="[OSL] Resetting OSL.")
 
         if self.has_knee:
             self.knee.set_mode(mode="voltage")  # type: ignore
             self.knee.set_voltage(value=0, force=True)  # type: ignore
 
-            time.sleep(secs=0.1)
+            time.sleep(0.1)
 
         if self.has_ankle:
             self.ankle.set_mode(mode="voltage")  # type: ignore
             self.ankle.set_voltage(value=0, force=True)  # type: ignore
 
-            time.sleep(secs=0.1)
+            time.sleep(0.1)
 
     @property
     def knee(self):
         if self.has_knee:
             return self._knee
         else:
             self.log.warning(msg="[OSL] Knee is not connected.")
@@ -454,18 +454,14 @@
     def loadcell(self):
         if self.has_loadcell:
             return self._loadcell
         else:
             self.log.warning(msg="[OSL] Loadcell is not connected.")
 
     @property
-    def current_limit(self) -> float:
-        return self._current_limit
-
-    @property
     def units(self) -> UnitsDefinition:
         return self._units
 
     @property
     def has_knee(self) -> bool:
         return self._has_knee
```

### Comparing `opensourceleg-1.2.3/opensourceleg/state_machine.py` & `opensourceleg-1.2.4/opensourceleg/state_machine.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,55 +2,61 @@
 # A simple and scalable Finite State Machine module
 
 from typing import Any, Callable, List, Optional
 
 from dataclasses import dataclass, field
 
 
-@dataclass
-class StateMachineData:
-    """
-    A class to represent the data of the state machine.
-    """
-
-    is_knee_active: bool = False
-    knee_stiffness: float = 0.0
-    knee_damping: float = 0.0
-    knee_theta: float = 0.0
-
-    is_ankle_active: bool = False
-    ankle_stiffness: float = 0.0
-    ankle_damping: float = 0.0
-    ankle_theta: float = 0.0
-
-    custom_data: dict[str, Any] = field(default_factory=dict)
-
-
 class State:
     """
     A class to represent a state in a finite state machine.
+
+    Args:
+        name (str): Name of the state
+        is_knee_active (bool): Whether the knee is active
+        knee_stiffness (float): Knee stiffness
+        knee_damping (float): Knee damping
+        knee_equilibrium_angle (float): Knee equilibrium angle
+        is_ankle_active (bool): Whether the ankle is active
+        ankle_stiffness (float): Ankle stiffness
+        ankle_damping (float): Ankle damping
+        ankle_equilibrium_angle (float): Ankle equilibrium angle
+
+    Note:
+        The knee and ankle impedance parameters are only used if the
+        corresponding joint is active. You can also set custom data
+        using the `set_custom_data` method.
     """
 
     def __init__(
-        self, name: str = "state", data: StateMachineData = StateMachineData()
+        self,
+        name: str = "state",
+        is_knee_active: bool = False,
+        knee_stiffness: float = 0.0,
+        knee_damping: float = 0.0,
+        knee_equilibrium_angle: float = 0.0,
+        is_ankle_active: bool = False,
+        ankle_stiffness: float = 0.0,
+        ankle_damping: float = 0.0,
+        ankle_equilibrium_angle: float = 0.0,
     ) -> None:
-        """
-        Parameters
-        ----------
-        name : str
-            The name of the state.
-        theta : float, optional
-            The theta parameter of the impedance model, by default 0.0
-        k : float, optional
-            The stiffness of the joint in PID units, by default 0.0
-        b : float, optional
-            The damping of the joint in PID units, by default 0.0
-        """
+
         self._name: str = name
-        self._data: StateMachineData = data
+
+        self._is_knee_active: bool = is_knee_active
+        self._knee_stiffness: float = knee_stiffness
+        self._knee_damping: float = knee_damping
+        self._knee_theta: float = knee_equilibrium_angle
+
+        self._is_ankle_active: bool = is_ankle_active
+        self._ankle_stiffness: float = ankle_stiffness
+        self._ankle_damping: float = ankle_damping
+        self._ankle_theta: float = ankle_equilibrium_angle
+
+        self._custom_data: dict[str, Any] = field(default_factory=dict)
 
         # Callbacks
         self._entry_callbacks: list[Callable[[Any], None]] = []
         self._exit_callbacks: list[Callable[[Any], None]] = []
 
     def __eq__(self, __o) -> bool:
         if __o.name == self._name:
@@ -61,28 +67,28 @@
     def __ne__(self, __o) -> bool:
         return not self.__eq__(__o)
 
     def __call__(self, data: Any) -> Any:
         pass
 
     def set_knee_impedance_paramters(self, theta, k, b) -> None:
-        self._data.knee_theta = theta
-        self._data.knee_stiffness = k
-        self._data.knee_damping = b
+        self._knee_theta = theta
+        self._knee_stiffness = k
+        self._knee_damping = b
 
     def set_ankle_impedance_paramters(self, theta, k, b) -> None:
-        self._data.ankle_theta = theta
-        self._data.ankle_stiffness = k
-        self._data.ankle_damping = b
+        self._ankle_theta = theta
+        self._ankle_stiffness = k
+        self._ankle_damping = b
 
     def set_custom_data(self, key: str, value: Any) -> None:
-        self._data.custom_data[key] = value
+        self._custom_data[key] = value
 
     def get_custom_data(self, key: str) -> Any:
-        return self._data.custom_data[key]
+        return self._custom_data[key]
 
     def on_entry(self, callback: Callable[[Any], None]) -> None:
         self._entry_callbacks.append(callback)
 
     def on_exit(self, callback: Callable[[Any], None]) -> None:
         self._exit_callbacks.append(callback)
 
@@ -90,57 +96,55 @@
         for c in self._entry_callbacks:
             c(data)
 
     def stop(self, data: Any) -> None:
         for c in self._exit_callbacks:
             c(data)
 
+    def make_knee_active(self):
+        self._is_knee_active = True
+
+    def make_ankle_active(self):
+        self._is_ankle_active = True
+
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def knee_stiffness(self) -> float:
-        return self._data.knee_stiffness
+        return self._knee_stiffness
 
     @property
     def knee_damping(self) -> float:
-        return self._data.knee_damping
+        return self._knee_damping
 
     @property
     def knee_theta(self) -> float:
-        return self._data.knee_theta
+        return self._knee_theta
 
     @property
     def ankle_stiffness(self) -> float:
-        return self._data.ankle_stiffness
+        return self._ankle_stiffness
 
     @property
     def ankle_damping(self) -> float:
-        return self._data.ankle_damping
+        return self._ankle_damping
 
     @property
     def ankle_theta(self) -> float:
-        return self._data.ankle_theta
+        return self._ankle_theta
 
     @property
     def is_knee_active(self) -> bool:
-        return self._data.is_knee_active
-
-    @is_knee_active.setter
-    def is_knee_active(self, value: bool) -> None:
-        self._data.is_knee_active = value
+        return self._is_knee_active
 
     @property
     def is_ankle_active(self) -> bool:
-        return self._data.is_ankle_active
-
-    @is_ankle_active.setter
-    def is_ankle_active(self, value: bool) -> None:
-        self._data.is_ankle_active = value
+        return self._is_ankle_active
 
 
 class Idle(State):
     def __init__(self) -> None:
         self._name = "idle"
         super().__init__(name=self._name)
 
@@ -256,15 +260,15 @@
         self._current_state: Optional[State] = None
         self._exit_callback: Optional[Callable[[Idle, Any], None]] = None
         self._exit_state = Idle()
         self.add_state(state=self._exit_state)
         self._initial_state = self._exit_state
 
         self._exited = True
-        self._osl: Any = None  # type: ignore
+        self._osl: Any = osl  # type: ignore
 
     def add_state(self, state: State, initial_state: bool = False) -> None:
         """
         Add a state to the state machine.
 
         Parameters
         ----------
```

### Comparing `opensourceleg-1.2.3/opensourceleg/thermal.py` & `opensourceleg-1.2.4/opensourceleg/thermal.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,94 +3,97 @@
 # Authors: Jianping Lin and Gray C. Thomas
 
 import numpy as np
 
 
 class ThermalModel:
     """
-    Thermal model of a motor developed by Jianping Lin and Gray C. Thomas 
+    Thermal model of a motor developed by Jianping Lin and Gray C. Thomas
     @U-M Locomotion Lab, directed by Dr. Robert Gregg
 
-    The model is based on the following assumptions:
-    1. The motor is a lumped system with two thermal nodes: the winding and the case.
-    2. The winding and the case are assumed to be in thermal equilibrium with the ambient.
-    3. The winding and the case are assumed to be in thermal equilibrium with each other.
-
-    The model is based on the following equations:
-    1. C_w * dT_w/dt = (I^2)R + (T_c-T_w)/R_WC
-    2. C_c * dT_c/dt = (T_w-T_c)/R_WC + (T_w-T_a)/R_CA
+    Assumptions:
+        1: The motor is a lumped system with two thermal nodes: the winding and the case.
+        2: The winding and the case are assumed to be in thermal equilibrium with the ambient.
+        3: The winding and the case are assumed to be in thermal equilibrium with each other.
+
+    Equations:
+        1: C_w * dT_w/dt = (I^2)R + (T_c-T_w)/R_WC
+        2: C_c * dT_c/dt = (T_w-T_c)/R_WC + (T_w-T_a)/R_CA
 
     where:
-    C_w: Thermal capacitance of the winding
-    C_c: Thermal capacitance of the case
-    R_WC: Thermal resistance between the winding and the case
-    R_CA: Thermal resistance between the case and the ambient
-    T_w: Temperature of the winding
-    T_c: Temperature of the case
-    T_a: Temperature of the ambient
-    I: Current
-    R: Resistance
-
-    The model is implemented in the following way:
-    1. The model is updated at every time step with the current and the ambient temperature.
-    2. The model can be used to predict the temperature of the winding and the case at any time step.
-    3. The model can also be used to scale the torque based on the temperature of the winding and the case.
+        C_w: Thermal capacitance of the winding
+        C_c: Thermal capacitance of the case
+        R_WC: Thermal resistance between the winding and the case
+        R_CA: Thermal resistance between the case and the ambient
+        T_w: Temperature of the winding
+        T_c: Temperature of the case
+        T_a: Temperature of the ambient
+        I: Current
+        R: Resistance
+
+    Implementation:
+        1: The model is updated at every time step with the current and the ambient temperature.
+        2: The model can be used to predict the temperature of the winding and the case at any time step.
+        3: The model can also be used to scale the torque based on the temperature of the winding and the case.
 
     Args:
-        ambient (int, optional): Ambient temperature in Celsius. Defaults to 21.
-        params (dict, optional): Dictionary of parameters. Defaults to dict().
-        temp_limit_windings (int, optional): Maximum temperature of the windings in Celsius. Defaults to 115.
-        soft_border_C_windings (int, optional): Soft border of the windings in Celsius. Defaults to 15.
-        temp_limit_case (int, optional): Maximum temperature of the case in Celsius. Defaults to 80.
-        soft_border_C_case (int, optional): Soft border of the case in Celsius. Defaults to 5.
+        ambient (float): Ambient temperature in Celsius. Defaults to 21.
+        params (dict): Dictionary of parameters. Defaults to dict().
+        temp_limit_windings (float): Maximum temperature of the windings in Celsius. Defaults to 115.
+        soft_border_C_windings (float): Soft border of the windings in Celsius. Defaults to 15.
+        temp_limit_case (float): Maximum temperature of the case in Celsius. Defaults to 80.
+        soft_border_C_case (float): Soft border of the case in Celsius. Defaults to 5.
 
 
     """
+
     def __init__(
         self,
-        ambient=21,
-        params=dict(),
-        temp_limit_windings=115,
-        soft_border_C_windings=15,
-        temp_limit_case=80,
-        soft_border_C_case=5,
+        ambient: float = 21,
+        params: dict = dict(),
+        temp_limit_windings: float = 115,
+        soft_border_C_windings: float = 15,
+        temp_limit_case: float = 80,
+        soft_border_C_case: float = 5,
     ) -> None:
 
         # The following parameters result from Jack Schuchmann's test with no fans
         self.C_w: float = 0.20 * 81.46202695970649
         self.R_WC = 1.0702867186480716
         self.C_c = 512.249065845453
         self.R_CA = 1.9406620046327363
         self.α: float = 0.393 * 1 / 100  # Pure copper. Taken from thermalmodel3.py
         self.R_T_0 = 65  # temp at which resistance was measured
         self.R_ϕ_0 = 0.376  # emirical, from the computed resistance (q-axis voltage/ q-axis current). Ohms
 
         self.__dict__.update(params)
-        self.T_w: int = ambient
-        self.T_c: int = ambient
-        self.T_a: int = ambient
-        self.soft_max_temp_windings: int = temp_limit_windings - soft_border_C_windings
-        self.abs_max_temp_windings: int = temp_limit_windings
-        self.soft_border_windings: int = soft_border_C_windings
-
-        self.soft_max_temp_case: int = temp_limit_case - soft_border_C_case
-        self.abs_max_temp_case: int = temp_limit_case
-        self.soft_border_case: int = soft_border_C_case
+        self.T_w: float = ambient
+        self.T_c: float = ambient
+        self.T_a: float = ambient
+        self.soft_max_temp_windings: float = (
+            temp_limit_windings - soft_border_C_windings
+        )
+        self.abs_max_temp_windings: float = temp_limit_windings
+        self.soft_border_windings: float = soft_border_C_windings
+
+        self.soft_max_temp_case: float = temp_limit_case - soft_border_C_case
+        self.abs_max_temp_case: float = temp_limit_case
+        self.soft_border_case: float = soft_border_C_case
 
-    def update(self, dt, motor_current: float = 0) -> None:
+    def update(self, dt: float = 1 / 200, motor_current: float = 0) -> None:
         """
         Updates the temperature of the winding and the case based on the current and the ambient temperature.
 
         Args:
-            dt (float): Time step in seconds.
-            motor_current (float, optional): Current in mA. Defaults to 0.
+            dt (float): Time step in seconds. Defaults to 1/200.
+            motor_current (float): Current in mA. Defaults to 0.
 
         Dynamics:
-            self.C_w * d self.T_w /dt = (I^2)R + (self.T_c-self.T_w)/self.R_WC
-            self.C_c * d self.T_c /dt = (self.T_w-self.T_c)/self.R_WC + (self.T_w-self.T_a)/self.R_CA
+            1: self.C_w * d self.T_w /dt = (I^2)R + (self.T_c-self.T_w)/self.R_WC
+            2: self.C_c * d self.T_c /dt = (self.T_w-self.T_c)/self.R_WC + (self.T_w-self.T_a)/self.R_CA
         """
 
         I_q_des: float = motor_current * 1e-3
 
         I2R = (
             I_q_des**2 * self.R_ϕ_0 * (1 + self.α * (self.T_w - self.R_T_0))
         )  # accounts for resistance change due to temp.
@@ -104,23 +107,23 @@
 
     def update_and_get_scale(self, dt, motor_current: float = 0, FOS=3.0):
         """
         Updates the temperature of the winding and the case based on the current and the ambient temperature and returns the scale factor for the torque.
 
         Args:
             dt (float): Time step in seconds.
-            motor_current (float, optional): Current in mA. Defaults to 0.
-            FOS (float, optional): Factor of safety. Defaults to 3.0.
+            motor_current (float): Current in mA. Defaults to 0.
+            FOS (float): Factor of safety. Defaults to 3.0.
 
         Returns:
             float: Scale factor for the torque.
 
         Dynamics:
-            self.C_w * d self.T_w /dt = (I^2)R + (self.T_c-self.T_w)/self.R_WC
-            self.C_c * d self.T_c /dt = (self.T_w-self.T_c)/self.R_WC + (self.T_w-self.T_a)/self.R_CA
+            1: self.C_w * d self.T_w /dt = (I^2)R + (self.T_c-self.T_w)/self.R_WC
+            2: self.C_c * d self.T_c /dt = (self.T_w-self.T_c)/self.R_WC + (self.T_w-self.T_a)/self.R_CA
         """
 
         I_q_des: float = motor_current * 1e-3
 
         I2R_des = (
             FOS * I_q_des**2 * self.R_ϕ_0 * (1 + self.α * (self.T_w - self.R_T_0))
         )  # accounts for resistance change due to temp.
```

### Comparing `opensourceleg-1.2.3/opensourceleg/tui.py` & `opensourceleg-1.2.4/opensourceleg/tui.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.3/opensourceleg/units.py` & `opensourceleg-1.2.4/opensourceleg/units.py`

 * *Files 14% similar despite different names*

```diff
@@ -65,14 +65,25 @@
         "mV": 1,
         "V": 1000,
     },
     "gravity": {
         "m/s^2": 1.0,
         "g": 9.80665,
     },
+    "temperature": {
+        "C": 1.0,
+        "F": 0.55556,
+        "K": 1.0,
+    },
+}
+
+TEMPERATURE_CONVERSIONS = {
+    "C": 0,
+    "F": 32,
+    "K": 273.15,
 }
 
 
 class UnitsDefinition(dict):
     """
     UnitsDefinition class is a dictionary with set and get methods that checks if the keys are valid
 
@@ -103,28 +114,39 @@
         Args:
             value (float): Value to be converted
             attribute (str): Attribute to be converted
 
         Returns:
             float: Converted value in the default unit
         """
-        return value * ALL_UNITS[attribute][self[attribute]]
+        val: float = value * ALL_UNITS[attribute][self[attribute]]
+
+        if attribute == "temperature":
+            val = (value - TEMPERATURE_CONVERSIONS[self[attribute]]) * ALL_UNITS[attribute][self[attribute]]  # type: ignore
+
+        return val
 
     def convert_from_default_units(self, value: float, attribute: str) -> float:
         """
         convert a value from the default unit to another unit
 
         Args:
             value (float): Value to be converted
             attribute (str): Attribute to be converted
 
         Returns:
             float: Converted value in the default unit
         """
-        return value / ALL_UNITS[attribute][self[attribute]]
+
+        val: float = value / ALL_UNITS[attribute][self[attribute]]
+
+        if attribute == "temperature":
+            val = val + TEMPERATURE_CONVERSIONS[self[attribute]]  # type: ignore
+
+        return val
 
 
 DEFAULT_UNITS = UnitsDefinition(
     {
         "force": "N",
         "torque": "N-m",
         "stiffness": "N/rad",
@@ -134,9 +156,17 @@
         "mass": "kg",
         "velocity": "rad/s",
         "acceleration": "rad/s^2",
         "time": "s",
         "current": "mA",
         "voltage": "mV",
         "gravity": "m/s^2",
+        "temperature": "C",
     }
 )
+
+if __name__ == "__main__":
+    units: UnitsDefinition = DEFAULT_UNITS
+    units["temperature"] = "F"  # type: ignore
+
+    print(units.convert_to_default_units(value=80, attribute="temperature"))
+    print(units.convert_from_default_units(value=0, attribute="temperature"))
```

### Comparing `opensourceleg-1.2.3/opensourceleg/utilities.py` & `opensourceleg-1.2.4/opensourceleg/utilities.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.3/pyproject.toml` & `opensourceleg-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "1.2.3"
+version = "1.2.4"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
```

### Comparing `opensourceleg-1.2.3/PKG-INFO` & `opensourceleg-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 1.2.3
+Version: 1.2.4
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
 Home-page: https://github.com/neurobionics/opensourceleg
 License: GNU GPL v3.0
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

