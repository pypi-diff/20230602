# Comparing `tmp/opensourceleg-1.2.2.tar.gz` & `tmp/opensourceleg-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-1.2.2.tar", max compression
+gzip compressed data, was "opensourceleg-1.2.3.tar", max compression
```

## Comparing `opensourceleg-1.2.2.tar` & `opensourceleg-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.2/LICENSE
--rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.2/README.md
--rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.2/opensourceleg/__init__.py
--rw-r--r--   0        0        0    19717 2023-05-18 00:45:47.154614 opensourceleg-1.2.2/opensourceleg/actuators.py
--rw-r--r--   0        0        0     1554 2023-05-11 18:11:48.610119 opensourceleg-1.2.2/opensourceleg/constants.py
--rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.2.2/opensourceleg/control.py
--rw-r--r--   0        0        0     3373 2023-05-18 00:36:35.044683 opensourceleg-1.2.2/opensourceleg/demo.py
--rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.2/opensourceleg/example.py
--rw-r--r--   0        0        0    10266 2023-05-18 00:38:28.486647 opensourceleg-1.2.2/opensourceleg/joints.py
--rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.2/opensourceleg/knee_encoder_map.npy
--rw-r--r--   0        0        0     8975 2023-05-18 00:38:28.488117 opensourceleg-1.2.2/opensourceleg/loadcell.py
--rw-r--r--   0        0        0     3713 2023-05-11 18:11:48.609099 opensourceleg-1.2.2/opensourceleg/logger.py
--rw-r--r--   0        0        0    14001 2023-05-18 00:45:20.037491 opensourceleg-1.2.2/opensourceleg/osl.py
--rw-r--r--   0        0        0     8305 2023-05-17 22:14:38.697899 opensourceleg-1.2.2/opensourceleg/state_machine.py
--rw-r--r--   0        0        0     3470 2023-05-11 18:11:49.648892 opensourceleg-1.2.2/opensourceleg/thermal.py
--rw-r--r--   0        0        0    21102 2023-05-18 00:38:00.668950 opensourceleg-1.2.2/opensourceleg/tui.py
--rw-r--r--   0        0        0     3529 2023-05-11 18:11:47.533081 opensourceleg-1.2.2/opensourceleg/units.py
--rw-r--r--   0        0        0    11526 2023-05-18 00:45:43.527511 opensourceleg-1.2.2/opensourceleg/utilities.py
--rw-r--r--   0        0        0     3668 2023-05-18 00:46:44.835096 opensourceleg-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 opensourceleg-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.3/README.md
+-rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.3/opensourceleg/__init__.py
+-rw-r--r--   0        0        0    21701 2023-06-02 15:30:09.743386 opensourceleg-1.2.3/opensourceleg/actuators.py
+-rw-r--r--   0        0        0     2277 2023-06-01 22:39:19.258650 opensourceleg-1.2.3/opensourceleg/constants.py
+-rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.2.3/opensourceleg/control.py
+-rw-r--r--   0        0        0     4299 2023-06-02 06:57:31.927981 opensourceleg-1.2.3/opensourceleg/demo.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.3/opensourceleg/example.py
+-rw-r--r--   0        0        0    10632 2023-06-01 21:48:32.759868 opensourceleg-1.2.3/opensourceleg/joints.py
+-rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.3/opensourceleg/knee_encoder_map.npy
+-rw-r--r--   0        0        0     8520 2023-06-01 22:39:19.421227 opensourceleg-1.2.3/opensourceleg/loadcell.py
+-rw-r--r--   0        0        0     3799 2023-06-02 05:24:50.983197 opensourceleg-1.2.3/opensourceleg/logger.py
+-rw-r--r--   0        0        0    15185 2023-06-02 15:14:01.350639 opensourceleg-1.2.3/opensourceleg/osl.py
+-rw-r--r--   0        0        0    10384 2023-06-02 06:57:32.045778 opensourceleg-1.2.3/opensourceleg/state_machine.py
+-rw-r--r--   0        0        0     6333 2023-06-02 14:52:19.367780 opensourceleg-1.2.3/opensourceleg/thermal.py
+-rw-r--r--   0        0        0    21057 2023-06-01 22:39:19.630121 opensourceleg-1.2.3/opensourceleg/tui.py
+-rw-r--r--   0        0        0     3531 2023-06-02 15:11:21.047386 opensourceleg-1.2.3/opensourceleg/units.py
+-rw-r--r--   0        0        0    11590 2023-06-02 04:54:05.760995 opensourceleg-1.2.3/opensourceleg/utilities.py
+-rw-r--r--   0        0        0     3668 2023-06-02 15:30:30.733471 opensourceleg-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.3/PKG-INFO
```

### Comparing `opensourceleg-1.2.2/LICENSE` & `opensourceleg-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.2/README.md` & `opensourceleg-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.2/opensourceleg/actuators.py` & `opensourceleg-1.2.3/opensourceleg/actuators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,251 +1,293 @@
+from typing import Any, Callable
+
 import os
 import time
+from ctypes import c_int
 from dataclasses import dataclass
 
 import flexsea.fx_enums as fxe
 import numpy as np
 from flexsea.device import Device
 
 from opensourceleg.constants import Constants
 from opensourceleg.control import (
     DEFAULT_CURRENT_GAINS,
     DEFAULT_IMPEDANCE_GAINS,
     DEFAULT_POSITION_GAINS,
 )
 from opensourceleg.logger import Logger
+from opensourceleg.thermal import ThermalModel
 from opensourceleg.units import DEFAULT_UNITS, UnitsDefinition
 
 
 @dataclass
 class ControlModes:
-    voltage = fxe.FX_VOLTAGE
-    current = fxe.FX_CURRENT
-    position = fxe.FX_POSITION
-    impedance = fxe.FX_IMPEDANCE
+    """
+    Control modes for the Dephy Actpack
+    """
+
+    voltage: c_int = fxe.FX_VOLTAGE
+    current: c_int = fxe.FX_CURRENT
+    position: c_int = fxe.FX_POSITION
+    impedance: c_int = fxe.FX_IMPEDANCE
 
 
 CONTROL_MODE = ControlModes()
 
 
 class ActpackMode:
-    def __init__(self, control_mode, device: "DephyActpack"):
-        self._control_mode = control_mode
-        self._device = device
-        self._entry_callback: callable = lambda: None
-        self._exit_callback: callable = lambda: None
+    """
+    Base class for Actpack modes
+
+    Args:
+        control_mode (c_int): Control mode
+        device (DephyActpack): Dephy Actpack
+    """
+
+    def __init__(self, control_mode: c_int, device: "DephyActpack") -> None:
+
+        self._control_mode: c_int = control_mode
+        self._device: DephyActpack = device
+        self._entry_callback: Callable[[], None] = lambda: None
+        self._exit_callback: Callable[[], None] = lambda: None
 
         self._has_gains = False
 
     def __eq__(self, __o: object) -> bool:
         if isinstance(__o, ActpackMode):
             return self._control_mode == __o._control_mode
         return False
 
     def __str__(self) -> str:
-        return str(self._control_mode)
+        return str(object=self._control_mode)
 
     @property
-    def mode(self):
+    def mode(self) -> c_int:
+        """
+        Control mode
+
+        Returns:
+            c_int: Control mode
+        """
         return self._control_mode
 
     @property
     def has_gains(self) -> bool:
+        """
+        Whether the mode has gains
+
+        Returns:
+            bool: True if the mode has gains, False otherwise
+        """
         return self._has_gains
 
-    def enter(self):
+    def enter(self) -> None:
+        """
+        Calls the entry callback
+        """
         self._entry_callback()
 
-    def exit(self):
+    def exit(self) -> None:
+        """
+        Calls the exit callback
+        """
         self._exit_callback()
 
-    def transition(self, to_state: "ActpackMode"):
+    def transition(self, to_state: "ActpackMode") -> None:
+        """
+        Transition to another mode. Calls the exit callback of the current mode
+        and the entry callback of the new mode.
+
+        Args:
+            to_state (ActpackMode): Mode to transition to
+        """
         self.exit()
         to_state.enter()
 
 
 class VoltageMode(ActpackMode):
-    def __init__(self, device: "DephyActpack"):
-        super().__init__(CONTROL_MODE.voltage, device)
+    def __init__(self, device: "DephyActpack") -> None:
+        super().__init__(control_mode=CONTROL_MODE.voltage, device=device)
         self._entry_callback = self._entry
         self._exit_callback = self._exit
 
-    def _entry(self):
-        self._device._log.debug(f"[Actpack] Entering Voltage mode.")
+    def _entry(self) -> None:
+        self._device._log.debug(msg=f"[Actpack] Entering Voltage mode.")
 
-    def _exit(self):
-        self._device._log.debug(f"[Actpack] Exiting Voltage mode.")
-        self._set_voltage(0)
-        time.sleep(0.1)
+    def _exit(self) -> None:
+        self._device._log.debug(msg=f"[Actpack] Exiting Voltage mode.")
+        self._set_voltage(voltage=0)
+        time.sleep(secs=0.1)
 
-    def _set_voltage(self, voltage: int):
+    def _set_voltage(self, voltage: int) -> None:
         self._device.send_motor_command(
-            self.mode,
-            voltage,
+            ctrl_mode=self.mode,
+            value=voltage,
         )
 
 
 class CurrentMode(ActpackMode):
-    def __init__(self, device: "DephyActpack"):
-        super().__init__(CONTROL_MODE.current, device)
+    def __init__(self, device: "DephyActpack") -> None:
+        super().__init__(control_mode=CONTROL_MODE.current, device=device)
         self._entry_callback = self._entry
         self._exit_callback = self._exit
 
-    def _entry(self):
-        self._device._log.debug(f"[Actpack] Entering Current mode.")
+    def _entry(self) -> None:
+        self._device._log.debug(msg=f"[Actpack] Entering Current mode.")
 
         if not self.has_gains:
             self._set_gains()
 
-        self._set_current(0)
+        self._set_current(current=0)
 
-    def _exit(self):
-        self._device._log.debug(f"[Actpack] Exiting Current mode.")
-        self._device.send_motor_command(CONTROL_MODE.voltage, 0)
-        time.sleep(1 / self._device.frequency)
+    def _exit(self) -> None:
+        self._device._log.debug(msg=f"[Actpack] Exiting Current mode.")
+        self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
+        time.sleep(secs=1 / self._device.frequency)
 
     def _set_gains(
         self,
         kp: int = DEFAULT_CURRENT_GAINS.kp,
         ki: int = DEFAULT_CURRENT_GAINS.ki,
         ff: int = DEFAULT_CURRENT_GAINS.ff,
-    ):
+    ) -> None:
 
         assert 0 <= kp <= 80, "kp must be between 0 and 80"
         assert 0 <= ki <= 800, "ki must be between 0 and 800"
         assert 0 <= ff <= 128, "ff must be between 0 and 128"
 
         self._device.set_gains(kp=kp, ki=ki, kd=0, k=0, b=0, ff=ff)
         self._has_gains = True
 
-        time.sleep(0.1)
+        time.sleep(secs=0.1)
 
-    def _set_current(self, current: int):
+    def _set_current(self, current: int) -> None:
         """Sets the Q-axis current of the motor
 
         Args:
             current (int): _description_
         """
         self._device.send_motor_command(
-            self.mode,
-            current,
+            ctrl_mode=self.mode,
+            value=current,
         )
 
 
 class PositionMode(ActpackMode):
-    def __init__(self, device: "DephyActpack"):
-        super().__init__(CONTROL_MODE.position, device)
+    def __init__(self, device: "DephyActpack") -> None:
+        super().__init__(control_mode=CONTROL_MODE.position, device=device)
         self._entry_callback = self._entry
         self._exit_callback = self._exit
 
-    def _entry(self):
-        self._device._log.debug(f"[Actpack] Entering Position mode.")
+    def _entry(self) -> None:
+        self._device._log.debug(msg=f"[Actpack] Entering Position mode.")
 
         if not self.has_gains:
             self._set_gains()
 
         self._set_motor_position(
-            int(
+            counts=int(
                 self._device._units.convert_to_default_units(
-                    self._device.motor_position, "position"
+                    value=self._device.motor_position, attribute="position"
                 )
                 / Constants.RAD_PER_COUNT
             )
         )
 
-    def _exit(self):
-        self._device._log.debug(f"[Actpack] Exiting Position mode.")
-        self._device.send_motor_command(CONTROL_MODE.voltage, 0)
-        time.sleep(0.1)
+    def _exit(self) -> None:
+        self._device._log.debug(msg=f"[Actpack] Exiting Position mode.")
+        self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
+        time.sleep(secs=0.1)
 
     def _set_gains(
         self,
         kp: int = DEFAULT_POSITION_GAINS.kp,
         ki: int = DEFAULT_POSITION_GAINS.ki,
         kd: int = DEFAULT_POSITION_GAINS.kd,
-    ):
+    ) -> None:
 
         assert 0 <= kp <= 1000, "kp must be between 0 and 1000"
         assert 0 <= ki <= 1000, "ki must be between 0 and 1000"
         assert 0 <= kd <= 1000, "kd must be between 0 and 1000"
 
         self._device.set_gains(kp=kp, ki=ki, kd=kd, k=0, b=0, ff=0)
         self._has_gains = True
 
-        time.sleep(1 / self._device.frequency)
+        time.sleep(secs=1 / self._device.frequency)
 
-    def _set_motor_position(self, counts: int):
+    def _set_motor_position(self, counts: int) -> None:
         """Sets the motor position
 
         Args:
             counts (int): position in counts
         """
         self._device.send_motor_command(
-            self.mode,
-            counts,
+            ctrl_mode=self.mode,
+            value=counts,
         )
 
 
 class ImpedanceMode(ActpackMode):
-    def __init__(self, device: "DephyActpack"):
-        super().__init__(CONTROL_MODE.impedance, device)
+    def __init__(self, device: "DephyActpack") -> None:
+        super().__init__(control_mode=CONTROL_MODE.impedance, device=device)
         self._entry_callback = self._entry
         self._exit_callback = self._exit
 
-    def _entry(self):
-        self._device._log.debug(f"[Actpack] Entering Impedance mode.")
+    def _entry(self) -> None:
+        self._device._log.debug(msg=f"[Actpack] Entering Impedance mode.")
         if not self.has_gains:
             self._set_gains()
 
         self._set_motor_position(
-            int(
+            counts=int(
                 self._device._units.convert_to_default_units(
-                    self._device.motor_position, "position"
+                    value=self._device.motor_position, attribute="position"
                 )
                 / Constants.RAD_PER_COUNT
             )
         )
 
-    def _exit(self):
-        self._device._log.debug(f"[Actpack] Exiting Impedance mode.")
-        self._device.send_motor_command(CONTROL_MODE.voltage, 0)
-        time.sleep(1 / self._device.frequency)
+    def _exit(self) -> None:
+        self._device._log.debug(msg=f"[Actpack] Exiting Impedance mode.")
+        self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
+        time.sleep(secs=1 / self._device.frequency)
 
-    def _set_motor_position(self, counts: int):
+    def _set_motor_position(self, counts: int) -> None:
         """Sets the motor position
 
         Args:
             counts (int): position in counts
         """
         self._device.send_motor_command(
-            self.mode,
-            counts,
+            ctrl_mode=self.mode,
+            value=counts,
         )
 
     def _set_gains(
         self,
         kp: int = DEFAULT_IMPEDANCE_GAINS.kp,
         ki: int = DEFAULT_IMPEDANCE_GAINS.ki,
         K: int = DEFAULT_IMPEDANCE_GAINS.K,
         B: int = DEFAULT_IMPEDANCE_GAINS.B,
         ff: int = DEFAULT_IMPEDANCE_GAINS.ff,
-    ):
+    ) -> None:
 
         assert 0 <= kp <= 80, "kp must be between 0 and 80"
         assert 0 <= ki <= 800, "ki must be between 0 and 800"
         assert 0 <= ff <= 128, "ff must be between 0 and 128"
         assert 0 <= K, "K must be greater than 0"
         assert 0 <= B, "B must be greater than 0"
 
         self._device.set_gains(
             kp=int(kp), ki=int(ki), kd=int(0), k=int(K), b=int(B), ff=int(ff)
         )
         self._has_gains = True
 
-        time.sleep(1 / self._device.frequency)
+        time.sleep(secs=1 / self._device.frequency)
 
 
 class DephyActpack(Device):
     """Class for the Dephy Actpack
 
     Args:
         Device (_type_): _description_
@@ -260,15 +302,15 @@
     """
 
     def __init__(
         self,
         port: str = "/dev/ttyACM0",
         baud_rate: int = 230400,
         frequency: int = 500,
-        logger: Logger = None,
+        logger: Logger = Logger(),
         units: UnitsDefinition = DEFAULT_UNITS,
         debug_level: int = 0,
         dephy_log: bool = False,
     ) -> None:
         """
         Initializes the Actpack class
 
@@ -277,420 +319,419 @@
             baud_rate (int): _description_. Defaults to 230400.
             frequency (int): _description_. Defaults to 500.
             logger (Logger): _description_
             units (UnitsDefinition): _description_
             debug_level (int): _description_. Defaults to 0.
             dephy_log (bool): _description_. Defaults to False.
         """
-        super().__init__(port, baud_rate)
-        self._debug_level = debug_level
-        self._dephy_log = dephy_log
-        self._frequency = frequency
-        self._data: dict = None
-        self._log = logger
+        super().__init__(port=port, baud_rate=baud_rate)
+        self._debug_level: int = debug_level
+        self._dephy_log: bool = dephy_log
+        self._frequency: int = frequency
+        self._data: Any = None
+
+        self._log: Logger = logger
         self._state = None
-        self._units = units if units else DEFAULT_UNITS
+        self._units: UnitsDefinition = units if units else DEFAULT_UNITS
 
         self._motor_zero_position = 0.0
         self._joint_zero_position = 0.0
 
+        self._thermal_model: ThermalModel = ThermalModel(temp_limit_windings=80, soft_border_C_windings=10, temp_limit_case=70, soft_border_C_case=10)
+        
         self._modes: dict[str, ActpackMode] = {
-            "voltage": VoltageMode(self),
-            "position": PositionMode(self),
-            "current": CurrentMode(self),
-            "impedance": ImpedanceMode(self),
+            "voltage": VoltageMode(device=self),
+            "position": PositionMode(device=self),
+            "current": CurrentMode(device=self),
+            "impedance": ImpedanceMode(device=self),
         }
 
         self._mode: ActpackMode = self._modes["voltage"]
 
-    def start(self):
+    def start(self) -> None:
         try:
-            self.open(self._frequency, self._debug_level, log_enabled=self._dephy_log)
+            self.open(
+                freq=self._frequency,
+                log_level=self._debug_level,
+                log_enabled=self._dephy_log,
+            )
         except OSError as e:
             print("\n")
             self._log.error(
-                f"Need admin previleges to open the port '{self.port}'. \n\nPlease run the script with 'sudo' command or add the user to the dialout group.\n"
+                msg=f"Need admin previleges to open the port '{self.port}'. \n\nPlease run the script with 'sudo' command or add the user to the dialout group.\n"
             )
-            os._exit(1)
+            os._exit(status=1)
 
-        time.sleep(0.1)
+        time.sleep(secs=0.1)
         self._data = self.read()
         self._mode.enter()
 
-    def stop(self):
-        self.set_mode("voltage")
-        self.set_voltage(0, force=True)
+    def stop(self) -> None:
+        self.set_mode(mode="voltage")
+        self.set_voltage(value=0)
 
-        time.sleep(0.1)
+        time.sleep(secs=0.1)
         self.close()
 
-    def update(self):
+    def update(self) -> None:
         if self.is_streaming:
             self._data = self.read()
+            self._thermal_model.T_c = self.temperature
+            self._thermal_model.update(dt=(1/self._frequency), motor_current=self.motor_current)
         else:
             self._log.warning(
-                f"[Actpack] Please open() the device before streaming data."
+                msg=f"[Actpack] Please open() the device before streaming data."
             )
 
-    def set_mode(self, mode: str):
+    def set_mode(self, mode: str) -> None:
         if mode in self._modes:
-            self._mode.transition(self._modes[mode])
+            self._mode.transition(to_state=self._modes[mode])
             self._mode = self._modes[mode]
 
         else:
-            self._log.warning(f"Mode {mode} not found")
+            self._log.warning(msg=f"Mode {mode} not found")
             return
 
-    def set_motor_zero_position(self, position: float):
-        self._motor_zero_position = position
+    def set_motor_zero_position(self, position: float) -> None:
+        self._motor_zero_position: float = position
 
-    def set_joint_zero_position(self, position: float):
-        self._joint_zero_position = position
+    def set_joint_zero_position(self, position: float) -> None:
+        self._joint_zero_position: float = position
 
     def set_position_gains(
         self,
         kp: int = DEFAULT_POSITION_GAINS.kp,
         ki: int = DEFAULT_POSITION_GAINS.ki,
         kd: int = DEFAULT_POSITION_GAINS.kd,
-        force: bool = True,
-    ):
+    ) -> None:
 
         """
         Sets the position gains
 
         Args:
             kp (int): The proportional gain
             ki (int): The integral gain
             kd (int): The derivative gain
-            force (bool): Force the mode transition. Defaults to False.
         """
         if self._mode != self._modes["position"]:
-            self._log.warning(f"Cannot set position gains in mode {self._mode}")
+            self._log.warning(msg=f"Cannot set position gains in mode {self._mode}")
             return
 
-        self._mode._set_gains(kp=kp, ki=ki, kd=kd)
+        self._mode.set_gains(kp=kp, ki=ki, kd=kd)  # type: ignore
 
     def set_current_gains(
         self,
         kp: int = DEFAULT_CURRENT_GAINS.kp,
         ki: int = DEFAULT_CURRENT_GAINS.ki,
         ff: int = DEFAULT_CURRENT_GAINS.ff,
-        force: bool = True,
-    ):
+    ) -> None:
 
         """
         Sets the current gains
 
         Args:
             kp (int): The proportional gain
             ki (int): The integral gain
             ff (int): The feedforward gain
-            force (bool): Force the mode transition. Defaults to False.
         """
         if self._mode != self._modes["current"]:
             self._log.warning(f"Cannot set current gains in mode {self._mode}")
             return
 
-        self._mode._set_gains(kp=kp, ki=ki, ff=ff)
+        self._mode._set_gains(kp=kp, ki=ki, ff=ff)  # type: ignore
 
     def set_impedance_gains(
         self,
         kp: int = DEFAULT_IMPEDANCE_GAINS.kp,
         ki: int = DEFAULT_IMPEDANCE_GAINS.ki,
         K: int = DEFAULT_IMPEDANCE_GAINS.K,
         B: int = DEFAULT_IMPEDANCE_GAINS.B,
         ff: int = DEFAULT_IMPEDANCE_GAINS.ff,
-        force: bool = True,
-    ):
+    ) -> None:
         """
         Sets the impedance gains
 
         Args:
             kp (int): The proportional gain
             ki (int): The integral gain
             K (int): The spring constant
             B (int): The damping constant
             ff (int): The feedforward gain
-            force (bool): Force the mode transition. Defaults to False.
         """
         if self._mode != self._modes["impedance"]:
-            self._log.warning(f"Cannot set impedance gains in mode {self._mode}")
+            self._log.warning(msg=f"Cannot set impedance gains in mode {self._mode}")
             return
 
-        self._mode._set_gains(kp=kp, ki=ki, K=K, B=B, ff=ff)
+        self._mode._set_gains(kp=kp, ki=ki, K=K, B=B, ff=ff)  # type: ignore
 
-    def set_voltage(self, value: float, force: bool = False):
+    def set_voltage(self, value: float) -> None:
         """
         Sets the q axis voltage
 
         Args:
             value (float): The voltage to set
-            force (bool): Force the mode transition. Defaults to False.
         """
         if self._mode != self._modes["voltage"]:
-            self._log.warning(f"Cannot set voltage in mode {self._mode}")
+            self._log.warning(msg=f"Cannot set voltage in mode {self._mode}")
             return
 
-        self._mode._set_voltage(
-            int(self._units.convert_to_default_units(value, "voltage")),
+        self._mode._set_voltage(  # type: ignore
+            int(self._units.convert_to_default_units(value=value, attribute="voltage")),
         )
 
-    def set_current(self, value: float, force: bool = False):
+    def set_current(self, value: float) -> None:
         """
         Sets the q axis current
 
         Args:
             value (float): The current to set
-            force (bool): Force the mode transition. Defaults to False.
         """
         if self._mode != self._modes["current"]:
-            self._log.warning(f"Cannot set current in mode {self._mode}")
+            self._log.warning(msg=f"Cannot set current in mode {self._mode}")
             return
 
-        self._mode._set_current(
-            int(self._units.convert_to_default_units(value, "current")),
+        self._mode._set_current(  # type: ignore
+            int(self._units.convert_to_default_units(value=value, attribute="current")),
         )
 
-    def set_motor_torque(self, torque: float, force: bool = False):
+    def set_motor_torque(self, torque: float) -> None:
         """
         Sets the motor torque
 
         Args:
             torque (float): The torque to set
-            force (bool): Force the mode transition. Defaults to False.
         """
         if self._mode != self._modes["current"]:
-            self._log.warning(f"Cannot set motor_torque in mode {self._mode}")
+            self._log.warning(msg=f"Cannot set motor_torque in mode {self._mode}")
             return
 
-        self._mode._set_current(
+        self._mode._set_current(  # type: ignore
             int(
-                self._units.convert_to_default_units(torque, "torque")
+                self._units.convert_to_default_units(value=torque, attribute="torque")
                 / Constants.NM_PER_MILLIAMP
             ),
         )
 
-    def set_motor_position(self, position: float):
+    def set_motor_position(self, position: float) -> None:
         """
         Sets the motor position
 
         Args:
             position (float): The position to set
         """
         if self._mode not in [self._modes["position"], self._modes["impedance"]]:
-            self._log.warning(f"Cannot set motor position in mode {self._mode}")
+            self._log.warning(msg=f"Cannot set motor position in mode {self._mode}")
             return
 
-        self._mode._set_motor_position(
+        self._mode._set_motor_position(  # type: ignore
             int(
-                self._units.convert_to_default_units(position, "position")
+                self._units.convert_to_default_units(
+                    value=position, attribute="position"
+                )
                 / Constants.RAD_PER_COUNT
             ),
         )
 
     # Read only properties from the actpack
 
     @property
-    def units(self):
+    def units(self) -> UnitsDefinition:
         return self._units
 
     @property
-    def frequency(self):
+    def frequency(self) -> int:
         return self._frequency
 
     @property
-    def mode(self):
+    def mode(self) -> ActpackMode:
         return self._mode
 
     @property
-    def motor_zero_position(self):
+    def motor_zero_position(self) -> float:
         return self._motor_zero_position
 
     @property
-    def joint_zero_position(self):
+    def joint_zero_position(self) -> float:
         return self._joint_zero_position
 
     @property
     def battery_voltage(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.batt_volt,
-                "voltage",
+                value=self._data.batt_volt,
+                attribute="voltage",
             )
         else:
             return 0
 
     @property
     def batter_current(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.batt_curr,
-                "current",
+                value=self._data.batt_curr,
+                attribute="current",
             )
         else:
             return 0
 
     @property
     def motor_voltage(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.mot_volt,
-                "voltage",
+                value=self._data.mot_volt,
+                attribute="voltage",
             )
         else:
             return 0
 
     @property
     def motor_current(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.mot_cur,
-                "current",
+                value=self._data.mot_cur,
+                attribute="current",
             )
         else:
             return 0
 
     @property
     def motor_torque(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.mot_cur * Constants.NM_PER_MILLIAMP,
-                "torque",
+                value=self._data.mot_cur * Constants.NM_PER_MILLIAMP,
+                attribute="torque",
             )
         else:
             return 0
 
     @property
     def motor_position(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                int(self._data.mot_ang) * Constants.RAD_PER_COUNT,
-                "position",
+                value=int(self._data.mot_ang) * Constants.RAD_PER_COUNT,
+                attribute="position",
             )
         else:
             return 0
 
     @property
     def motor_velocity(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                int(self._data.mot_vel) * Constants.RAD_PER_COUNT,
-                "velocity",
+                value=int(self._data.mot_vel) * Constants.RAD_PER_COUNT,
+                attribute="velocity",
             )
         else:
             return 0
 
     @property
     def motor_acceleration(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.mot_acc,
-                "acceleration",
+                value=self._data.mot_acc,
+                attribute="acceleration",
             )
         else:
             return 0
 
     @property
-    def motor_torque(self):
+    def joint_position(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self.motor_current * Constants.NM_PER_AMP,
-                "torque",
+                value=self._data.ank_ang * Constants.RAD_PER_COUNT,
+                attribute="position",
             )
         else:
             return 0
 
     @property
-    def joint_position(self):
+    def joint_velocity(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.ank_ang * Constants.RAD_PER_COUNT,
-                "position",
+                value=self._data.ank_vel * Constants.RAD_PER_COUNT,
+                attribute="velocity",
             )
         else:
             return 0
 
     @property
-    def joint_velocity(self):
+    def temperature(self):
         if self._data is not None:
-            return self._units.convert_from_default_units(
-                self._data.ank_vel * Constants.RAD_PER_COUNT,
-                "velocity",
-            )
+            return self._data.temperature
         else:
             return 0
 
     @property
     def genvars(self):
         if self._data is not None:
             return np.array(
-                [
+                object=[
                     self._data.genvar_0,
                     self._data.genvar_1,
                     self._data.genvar_2,
                     self._data.genvar_3,
                     self._data.genvar_4,
                     self._data.genvar_5,
                 ]
             )
         else:
-            return np.zeros(6)
+            return np.zeros(shape=6)
 
     @property
     def acc_x(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.accelx * Constants.M_PER_SEC_SQUARED_ACCLSB,
-                "gravity",
+                value=self._data.acc_x * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                attribute="gravity",
             )
         else:
             return 0
 
     @property
     def acc_y(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.accely * Constants.M_PER_SEC_SQUARED_ACCLSB,
-                "gravity",
+                value=self._data.acc_y * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                attribute="gravity",
             )
         else:
             return 0
 
     @property
     def acc_z(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.accelz * Constants.M_PER_SEC_SQUARED_ACCLSB,
-                "gravity",
+                value=self._data.acc_z * Constants.M_PER_SEC_SQUARED_ACCLSB,
+                attribute="gravity",
             )
         else:
             return 0
 
     @property
     def gyro_x(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.gyrox * Constants.RAD_PER_SEC_GYROLSB,
-                "velocity",
+                value=self._data.gyro_x * Constants.RAD_PER_SEC_GYROLSB,
+                attribute="velocity",
             )
         else:
             return 0
 
     @property
     def gyro_y(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.gyroy * Constants.RAD_PER_SEC_GYROLSB,
-                "velocity",
+                value=self._data.gyro_y * Constants.RAD_PER_SEC_GYROLSB,
+                attribute="velocity",
             )
         else:
             return 0
 
     @property
     def gyro_z(self):
         if self._data is not None:
             return self._units.convert_from_default_units(
-                self._data.gyroz * Constants.RAD_PER_SEC_GYROLSB,
-                "velocity",
+                value=self._data.gyro_z * Constants.RAD_PER_SEC_GYROLSB,
+                attribute="velocity",
             )
         else:
             return 0
```

### Comparing `opensourceleg-1.2.2/opensourceleg/control.py` & `opensourceleg-1.2.3/opensourceleg/control.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.2/opensourceleg/demo.py` & `opensourceleg-1.2.3/opensourceleg/demo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,135 +1,152 @@
 from opensourceleg.osl import OpenSourceLeg
 from opensourceleg.state_machine import Event, State
 
 BODY_WEIGHT = 60.0  # kg
 
 
-def estance_to_lstance(osl: OpenSourceLeg):
+def estance_to_lstance(osl: OpenSourceLeg) -> bool:
     """
     Transition from early stance to late stance when the loadcell
     reads a force greater than a threshold.
     """
+    assert osl.loadcell is not None
     if osl.loadcell.fz < -0.0167 * BODY_WEIGHT:
         return True
     else:
         return False
 
 
-def lstance_to_eswing(osl: OpenSourceLeg):
+def lstance_to_eswing(osl: OpenSourceLeg) -> bool:
     """
     Transition from late stance to early swing when the loadcell
     reads a force less than a threshold.
     """
+    assert osl.loadcell is not None
     if osl.loadcell.fz > -0.00267 * BODY_WEIGHT:
         return True
     else:
         return False
 
 
-def eswing_to_lswing(osl: OpenSourceLeg):
+def eswing_to_lswing(osl: OpenSourceLeg) -> bool:
     """
     Transition from early swing to late swing when the knee angle
     is greater than a threshold and the knee velocity is less than
     a threshold.
     """
+    assert osl.knee is not None
     if osl.knee.output_position > 60 and osl.knee.output_velocity < 0.135:
         return True
     else:
         return False
 
 
-def eswing_to_estance(osl: OpenSourceLeg):
+def eswing_to_estance(osl: OpenSourceLeg) -> bool:
     """
     Transition from early swing to early stance when the loadcell
     reads a force greater than a threshold.
     """
+    assert osl.loadcell is not None
     if osl.loadcell.fz < -0.02 * BODY_WEIGHT:
         return True
     else:
-        False
+        return False
 
 
-def lswing_to_estance(osl: OpenSourceLeg):
+def lswing_to_estance(osl: OpenSourceLeg) -> bool:
     """
     Transition from late swing to early stance when the loadcell
     reads a force greater than a threshold or the knee angle is
     less than a threshold.
     """
+    assert osl.knee is not None and osl.loadcell is not None
     if osl.loadcell.fz < -0.02 * BODY_WEIGHT or osl.knee.output_position < 30:
         return True
     else:
         return False
 
 
 def main():
     osl = OpenSourceLeg(frequency=200)
-    osl.units["position"] = "deg"
+    osl.units["position"] = "deg"  # type: ignore
 
     osl.add_joint(
         name="knee",
         gear_ratio=41.4999,
     )
 
     osl.add_loadcell(
         dephy_mode=False,
     )
 
     osl.add_state_machine()
 
-    early_stance = State("e_stance", 5, 130, 450)
-    late_stance = State("l_stance", 5, 175, 200)
-    early_swing = State("e_swing", 62, 40, 40)
-    late_swing = State("l_swing", 30, 100, 200)
-
-    foot_flat = Event("foot_flat")
-    heel_off = Event("heel_off")
-    toe_off = Event("toe_off")
-    pre_heel_strike = Event("pre_heel_strike")
-    heel_strike = Event("heel_strike")
-    misc = Event("misc")
-
-    osl.state_machine.add_state(early_stance, initial_state=True)
-    osl.state_machine.add_state(late_stance)
-    osl.state_machine.add_state(early_swing)
-    osl.state_machine.add_state(late_swing)
-
-    osl.state_machine.add_event(foot_flat)
-    osl.state_machine.add_event(heel_off)
-    osl.state_machine.add_event(toe_off)
-    osl.state_machine.add_event(pre_heel_strike)
-    osl.state_machine.add_event(heel_strike)
-    osl.state_machine.add_event(misc)
+    early_stance = State(name="e_stance")
+    early_stance.set_knee_impedance_paramters(theta=5, k=130, b=450)
+    early_stance.is_knee_active = True
+
+    late_stance = State(name="l_stance")
+    late_stance.set_knee_impedance_paramters(theta=5, k=175, b=200)
+    late_stance.is_knee_active = True
+
+    early_swing = State(name="e_swing")
+    early_swing.set_knee_impedance_paramters(theta=62, k=40, b=40)
+    early_swing.is_knee_active = True
+
+    late_swing = State(name="l_swing")
+    late_swing.set_knee_impedance_paramters(theta=30, k=100, b=200)
+    late_swing.is_knee_active = True
+
+    foot_flat = Event(name="foot_flat")
+    heel_off = Event(name="heel_off")
+    toe_off = Event(name="toe_off")
+    pre_heel_strike = Event(name="pre_heel_strike")
+    heel_strike = Event(name="heel_strike")
+    misc = Event(name="misc")
+
+    assert osl.state_machine is not None
+    osl.state_machine.add_state(state=early_stance, initial_state=True)
+    osl.state_machine.add_state(state=late_stance)
+    osl.state_machine.add_state(state=early_swing)
+    osl.state_machine.add_state(state=late_swing)
+
+    osl.state_machine.add_event(event=foot_flat)
+    osl.state_machine.add_event(event=heel_off)
+    osl.state_machine.add_event(event=toe_off)
+    osl.state_machine.add_event(event=pre_heel_strike)
+    osl.state_machine.add_event(event=heel_strike)
+    osl.state_machine.add_event(event=misc)
 
     osl.state_machine.add_transition(
-        early_stance,
-        late_stance,
-        foot_flat,
-        estance_to_lstance,
+        source=early_stance,
+        destination=late_stance,
+        event=foot_flat,
+        callback=estance_to_lstance,
     )
 
     osl.state_machine.add_transition(
-        late_stance,
-        early_swing,
-        heel_off,
-        lstance_to_eswing,
+        source=late_stance,
+        destination=early_swing,
+        event=heel_off,
+        callback=lstance_to_eswing,
     )
 
     osl.state_machine.add_transition(
-        early_swing,
-        late_swing,
-        toe_off,
-        eswing_to_lswing,
+        source=early_swing,
+        destination=late_swing,
+        event=toe_off,
+        callback=eswing_to_lswing,
     )
 
     osl.state_machine.add_transition(
-        late_swing,
-        early_stance,
-        heel_strike,
-        lswing_to_estance,
+        source=late_swing,
+        destination=early_stance,
+        event=heel_strike,
+        callback=lswing_to_estance,
     )
 
     osl.add_tui()
 
     with osl:
         osl.run(set_state_machine_parameters=True)
```

### Comparing `opensourceleg-1.2.2/opensourceleg/joints.py` & `opensourceleg-1.2.3/opensourceleg/joints.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self,
         name: str = "knee",
         port: str = "/dev/ttyACM0",
         baud_rate: int = 230400,
         frequency: int = 500,
         gear_ratio: float = 1.0,
         has_loadcell: bool = False,
-        logger: Logger = None,
+        logger: Logger = Logger(),
         units: UnitsDefinition = DEFAULT_UNITS,
         debug_level: int = 0,
         dephy_log: bool = False,
     ) -> None:
 
         super().__init__(
             port=port,
@@ -50,103 +50,103 @@
         self._stiffness_sp: int = 200
         self._damping_sp: int = 400
         self._equilibrium_position_sp = 0.0
 
         self._control_mode_sp: str = "voltage"
 
         if "knee" in name.lower() or "ankle" in name.lower():
-            self._name = name
+            self._name: str = name
         else:
-            self._log.warning(f"Invalid joint name: {name}")
+            self._log.warning(msg=f"Invalid joint name: {name}")
             return
 
-        if os.path.isfile(f"./{self._name}_encoder_map.npy"):
-            coefficients = np.load(f"./{self._name}_encoder_map.npy")
-            self._encoder_map = np.polynomial.polynomial.Polynomial(coefficients)
+        if os.path.isfile(path=f"./{self._name}_encoder_map.npy"):
+            coefficients = np.load(file=f"./{self._name}_encoder_map.npy")
+            self._encoder_map = np.polynomial.polynomial.Polynomial(coef=coefficients)
         else:
             self._log.debug(
-                f"[{self._name}] No encoder map found. Please run the calibration routine."
+                msg=f"[{self._name}] No encoder map found. Please run the calibration routine."
             )
 
     def home(
         self,
         homing_voltage: int = 2000,
         homing_frequency: int = 100,
-    ):
+    ) -> None:
 
         is_homing = True
 
         CURRENT_THRESHOLD = 6000
         VELOCITY_THRESHOLD = 0.001
 
-        self.set_mode("voltage")
-        self.set_voltage(-1 * homing_voltage)  # mV, negative for counterclockwise
+        self.set_mode(mode="voltage")
+        self.set_voltage(value=-1 * homing_voltage)  # mV, negative for counterclockwise
 
         _motor_encoder_array = []
         _joint_encoder_array = []
 
-        time.sleep(0.1)
+        time.sleep(secs=0.1)
 
         try:
             while is_homing:
                 self.update()
-                time.sleep(1 / homing_frequency)
+                time.sleep(secs=1 / homing_frequency)
 
                 _motor_encoder_array.append(self.motor_position)
                 _joint_encoder_array.append(self.joint_position)
 
                 if (
                     abs(self.output_velocity) <= VELOCITY_THRESHOLD
                     or abs(self.motor_current) >= CURRENT_THRESHOLD
                 ):
-                    self.set_voltage(0)
+                    self.set_voltage(value=0)
                     is_homing = False
 
         except KeyboardInterrupt:
-            self.set_voltage(0)
-            self._log.warning("Homing interrupted.")
+            self.set_voltage(value=0)
+            self._log.warning(msg="Homing interrupted.")
             return
 
         _motor_zero_pos = self.motor_position
         _joint_zero_pos = self.joint_position
 
-        time.sleep(0.1)
+        time.sleep(secs=0.1)
 
         if np.std(_motor_encoder_array) < 1e-6:
             self._log.warning(
-                f"[{self._name}] Motor encoder not working. Please check the wiring."
+                msg=f"[{self._name}] Motor encoder not working. Please check the wiring."
             )
             return
 
         elif np.std(_joint_encoder_array) < 1e-6:
             self._log.warning(
-                f"[{self._name}] Joint encoder not working. Please check the wiring."
+                msg=f"[{self._name}] Joint encoder not working. Please check the wiring."
             )
             return
 
         if "ankle" in self._name.lower():
             self._zero_pos = np.deg2rad(30)
-            self.set_motor_zero_position(_motor_zero_pos)
-            self.set_joint_zero_position(_joint_zero_pos)
+            self.set_motor_zero_position(position=_motor_zero_pos)
+            self.set_joint_zero_position(position=_joint_zero_pos)
 
         else:
             self._zero_pos = 0.0
-            self.set_motor_zero_position(_motor_zero_pos)
-            self.set_joint_zero_position(_joint_zero_pos)
+            self.set_motor_zero_position(position=_motor_zero_pos)
+            self.set_joint_zero_position(position=_joint_zero_pos)
 
         self._is_homed = True
 
-        # if self.encoder_map is None:
-        #     if (
-        #         input(f"[{self._name}] Would you like to make an encoder map? (y/n): ")
-        #         == "y"
-        #     ):
-        #         self.make_encoder_map()
+        if self.encoder_map is None:
+            if (
+                input(f"[{self._name}] Would you like to make an encoder map? (y/n): ")
+                == "y"
+            ):
+                self.make_encoder_map()
 
-    def make_encoder_map(self):
+    def make_encoder_map(self) -> None:
         """
         This method makes a lookup table to calculate the position measured by the joint encoder.
         This is necessary because the magnetic output encoders are nonlinear.
         By making the map while the joint is unloaded, joint position calculated by motor position * gear ratio
         should be the same as the true joint position.
 
         Output from this function is a file containing a_i values parameterizing the map
@@ -156,90 +156,90 @@
         Author: Kevin Best, PhD
                 U-M Neurobionics Lab
                 Gitub: tkevinbest, https://github.com/tkevinbest
         """
 
         if not self.is_homed:
             self._log.warning(
-                f"[{self._name}] Please home the joint before making the encoder map."
+                msg=f"[{self._name}] Please home the joint before making the encoder map."
             )
             return
 
-        self.set_mode("current")
+        self.set_mode(mode="current")
         self.set_current_gains()
-        time.sleep(0.1)
+        time.sleep(secs=0.1)
         self.set_current_gains()
 
-        self.set_output_torque(0.0)
-        time.sleep(0.1)
-        self.set_output_torque(0.0)
+        self.set_output_torque(torque=0.0)
+        time.sleep(secs=0.1)
+        self.set_output_torque(torque=0.0)
 
         _joint_position_array = []
         _output_position_array = []
 
         self._log.info(
-            f"[{self._name}] Please manually move the joint numerous times \
+            msg=f"[{self._name}] Please manually move the joint numerous times \
                 through its full range of motion for 10 seconds.\
                    \n Press any key to continue."
         )
 
-        _start_time = time.time()
+        _start_time: float = time.time()
 
         try:
             while time.time() - _start_time < 10:
                 self.update()
                 _joint_position_array.append(self.joint_position)
                 _output_position_array.append(self.output_position)
 
-                time.sleep(1 / self.frequency)
+                time.sleep(secs=1 / self.frequency)
 
         except KeyboardInterrupt:
-            self._log.warning("Encoder map interrupted.")
+            self._log.warning(msg="Encoder map interrupted.")
             return
 
-        self._log.info(f"[{self._name}] You may now stop moving the joint.")
+        self._log.info(msg=f"[{self._name}] You may now stop moving the joint.")
 
         _power = np.arange(4.0)
         _a_mat = np.array(_joint_position_array).reshape(-1, 1) ** _power
         _beta = np.linalg.lstsq(_a_mat, _output_position_array, rcond=None)[0]
         _coeffs = _beta[0]
 
-        self._encoder_map = np.polynomial.polynomial.Polynomial(_coeffs)
+        self._encoder_map = np.polynomial.polynomial.Polynomial(coef=_coeffs)
 
-        np.save(f"./{self._name}_encoder_map.npy", _coeffs)
-        self._log.info(f"[{self._name}] Encoder map saved.")
+        np.save(file=f"./{self._name}_encoder_map.npy", arr=_coeffs)
+        self._log.info(msg=f"[{self._name}] Encoder map saved.")
 
-    def set_output_torque(self, torque: float):
+    def set_output_torque(self, torque: float) -> None:
         """
         Set the output torque of the joint.
         This is the torque that is applied to the joint, not the motor.
 
         Args:
             torque (float): torque in user-defined units
         """
-        self.set_motor_torque(torque / self.gear_ratio)
+        self.set_motor_torque(torque=torque / self.gear_ratio)
 
-    def set_output_position(self, position: float):
+    def set_output_position(self, position: float) -> None:
         """
         Set the output position of the joint.
         This is the desired position of the joint, not the motor.
 
         Args:
             position (float): position in user-defined units
         """
-        self.set_motor_position(position * self.gear_ratio)
+        self.set_motor_position(position=position * self.gear_ratio)
 
     def set_motor_impedance(
         self,
         kp: int = 40,
         ki: int = 400,
         K: float = 0.08922,
         B: float = 0.0038070,
         ff: int = 128,
-    ):
+    ) -> None:
         """
         Set the impedance gains of the motor in real units: Nm/rad and Nm/rad/s.
 
         Args:
             kp (int): Proportional gain. Defaults to 40.
             ki (int): Integral gain. Defaults to 400.
             K (float): Spring constant. Defaults to 0.08922 Nm/rad.
@@ -257,15 +257,15 @@
     def set_joint_impedance(
         self,
         kp: int = 40,
         ki: int = 400,
         K: float = 0.08922,
         B: float = 0.0038070,
         ff: int = 128,
-    ):
+    ) -> None:
         """
         Set the impedance gains of the joint in real units: Nm/rad and Nm/rad/s.
 
         Conversion:
             K_motor = K_joint / (gear_ratio ** 2)
             B_motor = B_joint / (gear_ratio ** 2)
 
@@ -280,73 +280,73 @@
             kp=kp,
             ki=ki,
             K=K / (self.gear_ratio**2),
             B=B / (self.gear_ratio**2),
             ff=ff,
         )
 
-    def update_set_points(self):
-        self.set_mode(self.control_mode_sp)
+    def update_set_points(self) -> None:
+        self.set_mode(mode=self.control_mode_sp)
 
     @property
     def zero_position(self):
         return self._zero_pos
 
     @zero_position.setter
     def zero_position(self, value):
         self._zero_pos = value
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self._name
 
     @property
-    def gear_ratio(self):
+    def gear_ratio(self) -> float:
         return self._gear_ratio
 
     @property
-    def is_homed(self):
+    def is_homed(self) -> bool:
         return self._is_homed
 
     @property
     def encoder_map(self):
         return self._encoder_map
 
     @property
-    def output_position(self):
+    def output_position(self) -> float:
         return self.motor_position / self.gear_ratio
 
     @property
-    def output_velocity(self):
+    def output_velocity(self) -> float:
         return self.motor_velocity / self.gear_ratio
 
     @property
-    def joint_torque(self):
+    def joint_torque(self) -> float:
         return self.motor_torque * self.gear_ratio
 
     @property
-    def motor_current_sp(self):
+    def motor_current_sp(self) -> float:
         return self._motor_current_sp
 
     @property
-    def motor_voltage_sp(self):
+    def motor_voltage_sp(self) -> float:
         return self._motor_voltage_sp
 
     @property
-    def motor_position_sp(self):
+    def motor_position_sp(self) -> float:
         return self._motor_position_sp
 
     @property
-    def stiffness_sp(self):
+    def stiffness_sp(self) -> int:
         return self._stiffness_sp
 
     @property
-    def damping_sp(self):
+    def damping_sp(self) -> int:
         return self._damping_sp
 
     @property
-    def equilibirum_position_sp(self):
+    def equilibirum_position_sp(self) -> float:
         return self._equilibrium_position_sp
 
     @property
-    def control_mode_sp(self):
+    def control_mode_sp(self) -> str:
         return self._control_mode_sp
```

### Comparing `opensourceleg-1.2.2/opensourceleg/loadcell.py` & `opensourceleg-1.2.3/opensourceleg/loadcell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 
 import numpy as np
 from smbus2 import SMBus
 
+from opensourceleg.constants import Constants
 from opensourceleg.joints import Joint
 from opensourceleg.logger import Logger
 
 
 class StrainAmp:
     """
     A class to directly manage the 6ch strain gauge amplifier over I2C.
@@ -27,16 +28,16 @@
     MEM_R_CH5_L = 17
     MEM_R_CH6_H = 18
     MEM_R_CH6_L = 19
 
     def __init__(self, bus, I2C_addr=0x66) -> None:
         """Create a strainamp object, to talk over I2C"""
         # self._I2CMan = I2CManager(bus)
-        self._SMBus = SMBus(bus)
-        time.sleep(1)
+        self._SMBus = SMBus(bus=bus)
+        time.sleep(secs=1)
         self.bus = bus
         self.addr = I2C_addr
         self.genvars = np.zeros((3, 6))
         self.indx = 0
         self.is_streaming = True
         self.data = []
         self.failed_reads = 0
@@ -61,40 +62,40 @@
                 raise Exception("Load cell unresponsive.")
         # unpack them and return as nparray
         return self.unpack_compressed_strain(self.data)
 
     def update(self):
         """Called to update data of strain amp. Also returns data."""
         self.genvars[self.indx, :] = self.read_compressed_strain()
-        self.indx = (self.indx + 1) % 3
-        return np.median(self.genvars, axis=0)
+        self.indx: int = (self.indx + 1) % 3
+        return np.median(a=self.genvars, axis=0)
 
     @staticmethod
     def unpack_uncompressed_strain(data):
         """Used for an older version of the strain amp firmware (at least pre-2017)"""
         ch1 = (data[0] << 8) | data[1]
         ch2 = (data[2] << 8) | data[3]
         ch3 = (data[4] << 8) | data[5]
         ch4 = (data[6] << 8) | data[7]
         ch5 = (data[8] << 8) | data[9]
         ch6 = (data[10] << 8) | data[11]
-        return np.array([ch1, ch2, ch3, ch4, ch5, ch6])
+        return np.array(object=[ch1, ch2, ch3, ch4, ch5, ch6])
 
     @staticmethod
     def unpack_compressed_strain(data):
         """Used for more recent versions of strainamp firmware"""
         # ch1 = (data[0] << 4) | ( (data[1] >> 4) & 0x0F)
         # ch2 = ( (data[1] << 8) & 0x0F00) | data[2]
         # ch3 = (data[3] << 4) | ( (data[4] >> 4) & 0x0F)
         # ch4 = ( (data[4] << 8) & 0x0F00) | data[5]
         # ch5 = (data[6] << 4) | ( (data[7] >> 4) & 0x0F)
         # ch6 = ( (data[7] << 8) & 0x0F00) | data[8]
         # moved into one line to save 0.02ms -- maybe pointless but eh
         return np.array(
-            [
+            object=[
                 (data[0] << 4) | ((data[1] >> 4) & 0x0F),
                 ((data[1] << 8) & 0x0F00) | data[2],
                 (data[3] << 4) | ((data[4] >> 4) & 0x0F),
                 ((data[4] << 8) & 0x0F00) | data[5],
                 (data[6] << 4) | ((data[7] >> 4) & 0x0F),
                 ((data[7] << 8) & 0x0F00) | data[8],
             ]
@@ -104,15 +105,15 @@
     def strain_data_to_wrench(
         unpacked_strain, loadcell_matrix, loadcell_zero, exc=5, gain=125
     ):
         """Converts strain values between 0 and 4095 to a wrench in N and Nm"""
         loadcell_signed = (unpacked_strain - 2048) / 4095 * exc
         loadcell_coupled = loadcell_signed * 1000 / (exc * gain)
         return np.reshape(
-            np.transpose(loadcell_matrix.dot(np.transpose(loadcell_coupled)))
+            np.transpose(a=loadcell_matrix.dot(np.transpose(a=loadcell_coupled)))
             - loadcell_zero,
             (6,),
         )
 
     @staticmethod
     def wrench_to_strain_data(measurement, loadcell_matrix, exc=5, gain=125):
         """Wrench in N and Nm to the strain values that would give that wrench"""
@@ -121,128 +122,113 @@
         return ((loadcell_signed / exc) * 4095 + 2048).round(0).astype(int)
 
 
 class Loadcell:
     def __init__(
         self,
         dephy_mode: bool = False,
-        joint: Joint = None,
+        joint: Joint = None,  # type: ignore
         amp_gain: float = 125.0,
         exc: float = 5.0,
-        loadcell_matrix: np.array = None,
-        logger: "Logger" = None,
+        loadcell_matrix: np.ndarray = Constants.LOADCELL_MATRIX,
+        logger: "Logger" = None,  # type: ignore
     ) -> None:
-        self._is_dephy = dephy_mode
-        self._joint = joint
-        self._amp_gain = amp_gain
-        self._exc = exc
-        self._adc_range = 2**12 - 1
-        self._offset = (2**12) / 2
+        self._is_dephy: bool = dephy_mode
+        self._joint: Joint = joint
+        self._amp_gain: float = amp_gain
+        self._exc: float = exc
+        self._adc_range: int = 2**12 - 1
+        self._offset: float = (2**12) / 2
         self._lc = None
 
         if not self._is_dephy:
             self._lc = StrainAmp(bus=1, I2C_addr=0x66)
 
-        if not loadcell_matrix:
-            self._loadcell_matrix = np.array(
-                [
-                    (-38.72600, -1817.74700, 9.84900, 43.37400, -44.54000, 1824.67000),
-                    (-8.61600, 1041.14900, 18.86100, -2098.82200, 31.79400, 1058.6230),
-                    (
-                        -1047.16800,
-                        8.63900,
-                        -1047.28200,
-                        -20.70000,
-                        -1073.08800,
-                        -8.92300,
-                    ),
-                    (20.57600, -0.04000, -0.24600, 0.55400, -21.40800, -0.47600),
-                    (-12.13400, -1.10800, 24.36100, 0.02300, -12.14100, 0.79200),
-                    (-0.65100, -28.28700, 0.02200, -25.23000, 0.47300, -27.3070),
-                ]
-            )
-        else:
-            self._loadcell_matrix = loadcell_matrix
-
+        self._loadcell_matrix = loadcell_matrix
         self._loadcell_data = None
         self._prev_loadcell_data = None
 
-        self._loadcell_zero = np.zeros((1, 6), dtype=np.double)
+        self._loadcell_zero = np.zeros(shape=(1, 6), dtype=np.double)
         self._zeroed = False
-        self._log = logger
+        self._log: Logger = logger
 
     def reset(self):
         self._zeroed = False
-        self._loadcell_zero = np.zeros((1, 6), dtype=np.double)
+        self._loadcell_zero = np.zeros(shape=(1, 6), dtype=np.double)
 
-    def update(self, loadcell_zero=None):
+    def update(self, loadcell_zero=None) -> None:
         """
         Computes Loadcell data
 
         """
         if self._is_dephy:
             loadcell_signed = (self._joint.genvars - self._offset) / (
                 self._adc_range * self._exc
             )
         else:
+            assert self._lc is not None
             loadcell_signed = (self._lc.update() - self._offset) / (
                 self._adc_range * self._exc
             )
 
         loadcell_coupled = loadcell_signed * 1000 / (self._exc * self._amp_gain)
 
         if loadcell_zero is None:
             self._loadcell_data = (
-                np.transpose(self._loadcell_matrix.dot(np.transpose(loadcell_coupled)))
+                np.transpose(
+                    a=self._loadcell_matrix.dot(b=np.transpose(a=loadcell_coupled))
+                )
                 - self._loadcell_zero
             )
         else:
             self._loadcell_data = (
-                np.transpose(self._loadcell_matrix.dot(np.transpose(loadcell_coupled)))
+                np.transpose(
+                    a=self._loadcell_matrix.dot(b=np.transpose(a=loadcell_coupled))
+                )
                 - loadcell_zero
             )
 
-    def initialize(self, number_of_iterations: int = 2000):
+    def initialize(self, number_of_iterations: int = 2000) -> None:
         """
         Obtains the initial loadcell reading (aka) loadcell_zero
         """
-        ideal_loadcell_zero = np.zeros((1, 6), dtype=np.double)
+        ideal_loadcell_zero = np.zeros(shape=(1, 6), dtype=np.double)
 
         if not self._zeroed:
 
             if self._is_dephy:
                 if self._joint.is_streaming:
                     self._joint.update()
                     self.update()
                 else:
                     self._log.warning(
-                        "[Loadcell] {self._joint.name} joint isn't streaming data. Please start streaming data before initializing loadcell."
+                        msg="[Loadcell] {self._joint.name} joint isn't streaming data. Please start streaming data before initializing loadcell."
                     )
                     return
             else:
                 self.update()
 
             self._loadcell_zero = self._loadcell_data
 
             for _ in range(number_of_iterations):
                 self.update(ideal_loadcell_zero)
                 loadcell_offset = self._loadcell_data
-                self._loadcell_zero = (loadcell_offset + self._loadcell_zero) / 2.0
+                self._loadcell_zero = (loadcell_offset + self._loadcell_zero) / 2.0  # type: ignore
 
             self._zeroed = True
 
         elif (
             input(f"[Loadcell] Would you like to re-initialize loadcell? (y/n): ")
             == "y"
         ):
             self.reset()
             self.initialize()
 
     @property
-    def is_zeroed(self):
+    def is_zeroed(self) -> bool:
         return self._zeroed
 
     @property
     def fx(self):
         return self.loadcell_data[0]
 
     @property
```

### Comparing `opensourceleg-1.2.2/opensourceleg/logger.py` & `opensourceleg-1.2.3/opensourceleg/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     Methods:
         __init__(self, class_instance: object, file_path: str, logger: logging.Logger = None) -> None
         log(self) -> None
     """
 
     def __init__(
         self,
-        file_path: str,
+        file_path: str = "./osl.log",
         log_format: str = "[%(asctime)s] %(levelname)s: %(message)s",
     ) -> None:
 
-        self._file_path = file_path
+        self._file_path: str = file_path
 
         self._class_instances = []
         self._attributes = []
 
         self._file = open(self._file_path + ".csv", "w")
         self._writer = csv.writer(self._file)
         self._writer.writerow(self._attributes)
@@ -37,54 +37,54 @@
 
         super().__init__(__name__)
         self.setLevel(logging.DEBUG)
 
         self._std_formatter = logging.Formatter(log_format)
 
         self._file_handler = RotatingFileHandler(
-            self._file_path,
+            filename=self._file_path,
             mode="w",
             maxBytes=0,
             backupCount=10,
         )
-        self._file_handler.setLevel(logging.DEBUG)
-        self._file_handler.setFormatter(self._std_formatter)
+        self._file_handler.setLevel(level=logging.DEBUG)
+        self._file_handler.setFormatter(fmt=self._std_formatter)
 
         self._stream_handler = logging.StreamHandler()
-        self._stream_handler.setLevel(logging.INFO)
-        self._stream_handler.setFormatter(self._std_formatter)
+        self._stream_handler.setLevel(level=logging.INFO)
+        self._stream_handler.setFormatter(fmt=self._std_formatter)
 
-        self.addHandler(self._stream_handler)
-        self.addHandler(self._file_handler)
+        self.addHandler(hdlr=self._stream_handler)
+        self.addHandler(hdlr=self._file_handler)
 
         self._is_logging = False
 
     def set_file_level(self, level: str = "DEBUG") -> None:
         """
         Sets the level of the logger
 
         Args:
             level (str): Level of the logger
         """
         if level not in self._log_levels.keys():
-            self.warning(f"Invalid logging level: {level}")
+            self.warning(msg=f"Invalid logging level: {level}")
 
-        self._file_handler.setLevel(self._log_levels[level])
+        self._file_handler.setLevel(level=self._log_levels[level])
 
     def set_stream_level(self, level: str = "INFO") -> None:
         """
         Sets the level of the logger
 
         Args:
             level (str): Level of the logger
         """
         if level not in self._log_levels.keys():
-            self.warning(f"Invalid logging level: {level}")
+            self.warning(msg=f"Invalid logging level: {level}")
 
-        self._stream_handler.setLevel(self._log_levels[level])
+        self._stream_handler.setLevel(level=self._log_levels[level])
 
     def add_attributes(self, class_instance: object, attributes_str: list[str]) -> None:
         """
         Configures the logger to log the attributes of a class
 
         Args:
             class_instance (object): Class instance to log the attributes of
@@ -99,24 +99,24 @@
         """
 
         if not self._is_logging:
             for class_instance, attributes in zip(
                 self._class_instances, self._attributes
             ):
                 self._writer.writerow(
-                    [
+                    row=[
                         f"{class_instance.__class__.__name__}: {attribute}"
                         for attribute in attributes
                     ]
                 )
             self._is_logging = True
 
         for class_instance, attributes in zip(self._class_instances, self._attributes):
             self._writer.writerow(
-                [getattr(class_instance, attribute) for attribute in attributes]
+                row=[getattr(class_instance, attribute) for attribute in attributes]
             )
 
         self._file.flush()
 
     def close(self) -> None:
         """
         Closes the csv file
```

### Comparing `opensourceleg-1.2.2/opensourceleg/osl.py` & `opensourceleg-1.2.3/opensourceleg/osl.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 import time
 
 import numpy as np
 
 sys.path.append("../")
 
 import opensourceleg.utilities as utilities
+from opensourceleg.constants import Constants
 from opensourceleg.joints import Joint
 from opensourceleg.loadcell import Loadcell
 from opensourceleg.logger import Logger
 from opensourceleg.state_machine import State, StateMachine
 from opensourceleg.units import DEFAULT_UNITS, UnitsDefinition
 from opensourceleg.utilities import SoftRealtimeLoop
 
-CURRENT_LIMIT = 8000
-
 
 class OpenSourceLeg:
     """
     OSL class: This class is the main class for the Open Source Leg project. It
     contains all the necessary functions to control the leg.
 
     Returns:
@@ -34,15 +33,15 @@
         if OpenSourceLeg._instance is None:
             OpenSourceLeg()
         return OpenSourceLeg._instance
 
     def __init__(
         self,
         frequency: int = 200,
-        current_limit: float = 8000,
+        current_limit: float = Constants.MAX_CURRENT,
         file_name: str = "./osl.log",
     ) -> None:
         """
         Initialize the OSL class.
 
         Parameters
         ----------
@@ -61,98 +60,97 @@
         self._has_loadcell: bool = False
         self._has_tui: bool = False
         self._has_sm: bool = False
 
         self._current_limit: float = current_limit
         self._set_state_machine_parameters: bool = False
 
-        self._knee: Joint = None
-        self._ankle: Joint = None
-        self._loadcell: Loadcell = None
+        self._knee: Joint = None  # type: ignore
+        self._ankle: Joint = None  # type: ignore
+        self._loadcell: Loadcell = None  # type: ignore
 
         self.log = Logger(
             file_path=file_name, log_format="[%(asctime)s] %(levelname)s: %(message)s"
         )
 
         self.clock = SoftRealtimeLoop(dt=1.0 / self._frequency, report=False, fade=0.1)
-
         self._units: UnitsDefinition = DEFAULT_UNITS
 
         self.tui = None
         self.state_machine = None
 
-    def __enter__(self):
+    def __enter__(self) -> None:
 
         if self.has_knee:
             self._knee.start()
 
         if self.has_ankle:
             self._ankle.start()
 
         if self.has_loadcell:
             self._loadcell.initialize()
 
         if self.has_state_machine:
-            self.state_machine.start()
+            self.state_machine.start()  # type: ignore
 
             if self.has_knee:
-                self.knee.set_mode("impedance")
-                self.knee.set_impedance_gains()
+                self.knee.set_mode(mode="impedance")  # type: ignore
+                self.knee.set_impedance_gains()  # type: ignore
 
             if self.has_ankle:
-                self.ankle.set_mode("impedance")
-                self.ankle.set_impedance_gains()
+                self.ankle.set_mode(mode="impedance")  # type: ignore
+                self.ankle.set_impedance_gains()  # type: ignore
 
-    def __exit__(self, type, value, tb):
+    def __exit__(self, type, value, tb) -> None:
         if self.has_state_machine:
-            self.state_machine.stop()
+            self.state_machine.stop()  # type: ignore
 
         if self.has_knee:
             self._knee.stop()
 
         if self.has_ankle:
             self._ankle.stop()
 
         if self.has_tui:
-            if self.tui.is_running:
-                self.tui.quit()
+            if self.tui.is_running:  # type: ignore
+                self.tui.quit()  # type: ignore
 
     def __repr__(self) -> str:
         return f"OSL object. Frequency: {self._frequency} Hz"
 
     def add_tui(
         self,
         configuration: str = "state_machine",
         layout: str = "vertical",
-    ):
+    ) -> None:
         from opensourceleg.tui import TUI
 
         self._has_tui = True
         self.tui = TUI(
             title="www.opensourceleg.com", frequency=self._frequency, layout=layout
         )
 
         if configuration == "state_machine":
             if self.has_state_machine:
                 self.initialize_sm_tui()
             else:
                 self.log.warn(
-                    "State machine not initialized. Please initialize the state machine before adding the TUI."
+                    msg="State machine not initialized. Please initialize the state machine before adding the TUI."
                 )
 
     def add_joint(
         self,
         name: str = "knee",
-        port: str = None,
+        port: str = None,  # type: ignore
         baud_rate: int = 230400,
         gear_ratio: float = 1.0,
         has_loadcell: bool = False,
         debug_level: int = 0,
         dephy_log: bool = False,
-    ):
+    ) -> None:
         """
         Add a joint to the OSL object.
 
         Parameters
         ----------
         name : str, optional
             The name of the joint, by default "knee"
@@ -175,15 +173,15 @@
             self._has_knee = True
 
             if port is None:
                 ports = utilities.get_active_ports()
 
                 if len(ports) == 0:
                     self.log.warn(
-                        "No active ports found, please ensure that the joint is connected and powered on."
+                        msg="No active ports found, please ensure that the joint is connected and powered on."
                     )
 
                 else:
                     if "knee" in name.lower():
                         port = ports[0]
                     else:
                         port = ports[1]
@@ -212,24 +210,24 @@
                 has_loadcell=has_loadcell,
                 logger=self.log,
                 units=self.units,
                 debug_level=debug_level,
                 dephy_log=dephy_log,
             )
         else:
-            self.log.warning("[OSL] Joint name is not recognized.")
+            self.log.warning(msg="[OSL] Joint name is not recognized.")
 
     def add_loadcell(
         self,
         dephy_mode: bool = False,
-        joint: Joint = None,
+        joint: Joint = None,  # type: ignore
         amp_gain: float = 125.0,
         exc: float = 5.0,
-        loadcell_matrix=None,
-    ):
+        loadcell_matrix=Constants.LOADCELL_MATRIX,
+    ) -> None:
         """
         Add a loadcell to the OSL object.
 
         Parameters
         ----------
         dephy_mode : bool, optional
             Whether the loadcell is in dephy mode ie. connected to the dephy actpack with an FFC cable, by default False
@@ -244,74 +242,74 @@
         """
         self._has_loadcell = True
         self._loadcell = Loadcell(
             dephy_mode=dephy_mode,
             joint=joint,
             amp_gain=amp_gain,
             exc=exc,
-            loadcell_matrix=loadcell_matrix,
+            loadcell_matrix=loadcell_matrix,  # type: ignore
             logger=self.log,
         )
 
     def add_state_machine(
         self,
-    ):
+    ) -> None:
         """
         Add a state machine to the OSL object.
         """
         self.state_machine = StateMachine(osl=self)
         self._has_sm = True
 
     def update(
         self,
-    ):
+    ) -> None:
         if self.has_knee:
             self._knee.update()
 
-            if self.knee.motor_current > self.current_limit:
-                self.log.warn("[KNEE] Current limit reached. Stopping motor.")
-                self.__exit__()
+            if self.knee.motor_current > self.current_limit:  # type: ignore
+                self.log.warn(msg="[KNEE] Current limit reached. Stopping motor.")
+                self.__exit__(type=None, value=None, tb=None)
                 exit()
 
         if self.has_ankle:
             self._ankle.update()
 
-            if self.ankle.motor_current > self.current_limit:
+            if self.ankle.motor_current > self.current_limit:  # type: ignore
                 self.log.warn("[ANKLE] Current limit () reached. Stopping motor.")
-                self.__exit__()
+                self.__exit__(type=None, value=None, tb=None)
                 exit()
 
         if self.has_loadcell:
             self._loadcell.update()
 
         if self.has_state_machine:
-            self.state_machine.update()
+            self.state_machine.update()  # type: ignore
 
             if self._set_state_machine_parameters:
-                if self.has_knee:
-                    self.knee.set_impedance_gains(
-                        K=self.state_machine.current_state.stiffness,
-                        B=self.state_machine.current_state.damping,
+                if self.has_knee and self.state_machine.current_state.is_knee_active:  # type: ignore
+                    self.knee.set_impedance_gains(  # type: ignore
+                        K=self.state_machine.current_state.knee_stiffness,  # type: ignore
+                        B=self.state_machine.current_state.knee_damping,  # type: ignore
                     )
 
-                    self.knee.set_output_position(
-                        self.state_machine.current_state.equilibrium_angle
+                    self.knee.set_output_position(  # type: ignore
+                        position=self.state_machine.current_state.knee_theta  # type: ignore
                     )
 
-                elif self.has_ankle:
-                    self.ankle.set_impedance_gains(
-                        K=self.state_machine.current_state.stiffness,
-                        B=self.state_machine.current_state.damping,
+                elif self.has_ankle and self.state_machine.current_state.is_ankle_active:  # type: ignore
+                    self.ankle.set_impedance_gains(  # type: ignore
+                        K=self.state_machine.current_state.ankle_stiffness,  # type: ignore
+                        B=self.state_machine.current_state.ankle_damping,  # type: ignore
                     )
 
-                    self.ankle.set_output_position(
-                        self.state_machine.current_state.equilibrium_angle
+                    self.ankle.set_output_position(  # type: ignore
+                        position=self.state_machine.current_state.ankle_theta  # type: ignore
                     )
 
-    def run(self, set_state_machine_parameters: bool = False):
+    def run(self, set_state_machine_parameters: bool = False) -> None:
         """
         Run the OpenSourceLeg instance: update the joints, loadcell, and state machine.
         If the instance has a TUI, run the TUI.
         If the instance has a state machine and if set_state_machine_parameters is True,
         set the joint impedance gains and equilibrium angles to the current state's values.
 
         Parameters
@@ -319,27 +317,28 @@
         set_state_machine_parameters : bool, optional
             Whether to set the joint impedance gains and equilibrium angles to the current state's values, by default False
         """
 
         self._set_state_machine_parameters = set_state_machine_parameters
         self.update()
 
-        time.sleep(0.1)
+        time.sleep(secs=0.1)
 
         if not self.has_tui:
             self.update()
 
         else:
-            self.tui.add_update_callback(self.update)
-            self.tui.run()
+            self.tui.add_update_callback(callback=self.update)  # type: ignore
+            self.tui.run()  # type: ignore
 
-    def initialize_sm_tui(self):
+    def initialize_sm_tui(self) -> None:
 
         from opensourceleg.tui import COLORS
 
+        assert self.tui is not None
         self.tui.add_panel(
             name="top",
             layout="horizontal",
             border=False,
         )
 
         self.tui.add_panel(
@@ -375,15 +374,15 @@
             attribute="output_position",
             color=COLORS.yellow,
         )
 
         self.tui.add_state_visualizer(
             name="state_machine",
             parent="bottom",
-            states=self.state_machine.states,
+            states=self.state_machine.states,  # type: ignore
             object=self.state_machine,
             attribute="current_state_name",
             layout="horizontal",
         )
 
         self.tui.add_button(
             name="emergency_stop",
@@ -393,110 +392,106 @@
             border=True,
         )
 
     def estop(self, **kwargs):
         self.log.debug("[OSL] Emergency stop activated.")
 
         if self.has_tui:
-            self.tui.quit()
+            self.tui.quit()  # type: ignore
 
-    def home(self):
+    def home(self) -> None:
         if self.has_knee:
-            self.log.debug("[OSL] Homing knee joint.")
-            self.knee.home()
+            self.log.debug(msg="[OSL] Homing knee joint.")
+            self.knee.home()  # type: ignore
 
         if self.has_ankle:
-            self.log.debug("[OSL] Homing ankle joint.")
-            self.ankle.home()
+            self.log.debug(msg="[OSL] Homing ankle joint.")
+            self.ankle.home()  # type: ignore
 
-    def calibrate_loadcell(self):
-        self.log.debug("[OSL] Calibrating loadcell.")
+    def calibrate_loadcell(self) -> None:
+        self.log.debug(msg="[OSL] Calibrating loadcell.")
         if self.has_loadcell:
-            self.loadcell.reset()
+            self.loadcell.reset()  # type: ignore
 
-    def calibrate_encoders(self):
-        self.log.debug("[OSL] Calibrating encoders.")
+    def calibrate_encoders(self) -> None:
+        self.log.debug(msg="[OSL] Calibrating encoders.")
 
         if self.has_knee:
-            self.knee.make_encoder_map()
+            self.knee.make_encoder_map()  # type: ignore
 
         if self.has_ankle:
-            self.ankle.make_encoder_map()
+            self.ankle.make_encoder_map()  # type: ignore
 
-    def reset(self):
-        self.log.debug("[OSL] Resetting OSL.")
+    def reset(self) -> None:
+        self.log.debug(msg="[OSL] Resetting OSL.")
 
         if self.has_knee:
-            self.knee.set_mode("voltage")
-            self.knee.set_voltage(0, force=True)
+            self.knee.set_mode(mode="voltage")  # type: ignore
+            self.knee.set_voltage(value=0, force=True)  # type: ignore
 
-            time.sleep(0.1)
+            time.sleep(secs=0.1)
 
         if self.has_ankle:
-            self.ankle.set_mode("voltage")
-            self.ankle.set_voltage(0, force=True)
+            self.ankle.set_mode(mode="voltage")  # type: ignore
+            self.ankle.set_voltage(value=0, force=True)  # type: ignore
 
-            time.sleep(0.1)
+            time.sleep(secs=0.1)
 
     @property
     def knee(self):
         if self.has_knee:
             return self._knee
         else:
-            self.log.warning("[OSL] Knee is not connected.")
+            self.log.warning(msg="[OSL] Knee is not connected.")
 
     @property
     def ankle(self):
         if self.has_ankle:
             return self._ankle
         else:
-            self.log.warning("[OSL] Ankle is not connected.")
+            self.log.warning(msg="[OSL] Ankle is not connected.")
 
     @property
     def loadcell(self):
         if self.has_loadcell:
             return self._loadcell
         else:
-            self.log.warning("[OSL] Loadcell is not connected.")
+            self.log.warning(msg="[OSL] Loadcell is not connected.")
 
     @property
-    def current_limit(self):
+    def current_limit(self) -> float:
         return self._current_limit
 
     @property
-    def units(self):
+    def units(self) -> UnitsDefinition:
         return self._units
 
     @property
-    def has_knee(self):
+    def has_knee(self) -> bool:
         return self._has_knee
 
     @property
-    def has_ankle(self):
+    def has_ankle(self) -> bool:
         return self._has_ankle
 
     @property
-    def has_loadcell(self):
+    def has_loadcell(self) -> bool:
         return self._has_loadcell
 
     @property
-    def has_state_machine(self):
+    def has_state_machine(self) -> bool:
         return self._has_sm
 
     @property
-    def loadcell(self):
-        return self._loadcell
-
-    @property
-    def has_tui(self):
+    def has_tui(self) -> bool:
         return self._has_tui
 
 
 if __name__ == "__main__":
     osl = OpenSourceLeg(frequency=200)
 
-    osl.units["position"] = "deg"
+    osl.units["position"] = "deg"  # type: ignore
 
     osl.add_joint(
         name="knee",
         gear_ratio=41.61,
     )
```

### Comparing `opensourceleg-1.2.2/opensourceleg/state_machine.py` & `opensourceleg-1.2.3/opensourceleg/state_machine.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,56 @@
 #!/usr/bin/python3
 # A simple and scalable Finite State Machine module
 
 from typing import Any, Callable, List, Optional
 
+from dataclasses import dataclass, field
+
+
+@dataclass
+class StateMachineData:
+    """
+    A class to represent the data of the state machine.
+    """
+
+    is_knee_active: bool = False
+    knee_stiffness: float = 0.0
+    knee_damping: float = 0.0
+    knee_theta: float = 0.0
+
+    is_ankle_active: bool = False
+    ankle_stiffness: float = 0.0
+    ankle_damping: float = 0.0
+    ankle_theta: float = 0.0
+
+    custom_data: dict[str, Any] = field(default_factory=dict)
+
 
 class State:
     """
     A class to represent a state in a finite state machine.
     """
 
-    def __init__(self, name, theta=0.0, k=0.0, b=0.0) -> None:
+    def __init__(
+        self, name: str = "state", data: StateMachineData = StateMachineData()
+    ) -> None:
         """
         Parameters
         ----------
         name : str
             The name of the state.
         theta : float, optional
             The theta parameter of the impedance model, by default 0.0
         k : float, optional
             The stiffness of the joint in PID units, by default 0.0
         b : float, optional
             The damping of the joint in PID units, by default 0.0
         """
-        self._name = name
-
-        # Impedance parameters
-        self._theta = theta
-        self._k = k
-        self._b = b
+        self._name: str = name
+        self._data: StateMachineData = data
 
         # Callbacks
         self._entry_callbacks: list[Callable[[Any], None]] = []
         self._exit_callbacks: list[Callable[[Any], None]] = []
 
     def __eq__(self, __o) -> bool:
         if __o.name == self._name:
@@ -41,60 +60,96 @@
 
     def __ne__(self, __o) -> bool:
         return not self.__eq__(__o)
 
     def __call__(self, data: Any) -> Any:
         pass
 
-    def set_impedance_paramters(self, theta, k, b) -> None:
-        self._theta = theta
-        self._k = k
-        self._b = b
+    def set_knee_impedance_paramters(self, theta, k, b) -> None:
+        self._data.knee_theta = theta
+        self._data.knee_stiffness = k
+        self._data.knee_damping = b
+
+    def set_ankle_impedance_paramters(self, theta, k, b) -> None:
+        self._data.ankle_theta = theta
+        self._data.ankle_stiffness = k
+        self._data.ankle_damping = b
+
+    def set_custom_data(self, key: str, value: Any) -> None:
+        self._data.custom_data[key] = value
 
-    def get_impedance_paramters(self):
-        return self._theta, self._k, self._b
+    def get_custom_data(self, key: str) -> Any:
+        return self._data.custom_data[key]
 
-    def on_entry(self, callback: Callable[[Any], None]):
+    def on_entry(self, callback: Callable[[Any], None]) -> None:
         self._entry_callbacks.append(callback)
 
-    def on_exit(self, callback: Callable[[Any], None]):
+    def on_exit(self, callback: Callable[[Any], None]) -> None:
         self._exit_callbacks.append(callback)
 
-    def start(self, data: Any):
+    def start(self, data: Any) -> None:
         for c in self._entry_callbacks:
             c(data)
 
-    def stop(self, data: Any):
+    def stop(self, data: Any) -> None:
         for c in self._exit_callbacks:
             c(data)
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self._name
 
     @property
-    def equilibrium_angle(self):
-        return self._theta
+    def knee_stiffness(self) -> float:
+        return self._data.knee_stiffness
 
     @property
-    def stiffness(self):
-        return self._k
+    def knee_damping(self) -> float:
+        return self._data.knee_damping
 
     @property
-    def damping(self):
-        return self._b
+    def knee_theta(self) -> float:
+        return self._data.knee_theta
+
+    @property
+    def ankle_stiffness(self) -> float:
+        return self._data.ankle_stiffness
+
+    @property
+    def ankle_damping(self) -> float:
+        return self._data.ankle_damping
+
+    @property
+    def ankle_theta(self) -> float:
+        return self._data.ankle_theta
+
+    @property
+    def is_knee_active(self) -> bool:
+        return self._data.is_knee_active
+
+    @is_knee_active.setter
+    def is_knee_active(self, value: bool) -> None:
+        self._data.is_knee_active = value
+
+    @property
+    def is_ankle_active(self) -> bool:
+        return self._data.is_ankle_active
+
+    @is_ankle_active.setter
+    def is_ankle_active(self, value: bool) -> None:
+        self._data.is_ankle_active = value
 
 
 class Idle(State):
     def __init__(self) -> None:
         self._name = "idle"
-        super().__init__(self._name)
+        super().__init__(name=self._name)
 
     @property
-    def status(self):
+    def status(self) -> str:
         return self._name
 
 
 class Event:
     """
     Event class
     """
@@ -128,65 +183,67 @@
     """
 
     def __init__(
         self,
         event: Event,
         source: State,
         destination: State,
-        callback: Callable[[Any], bool] = None,
+        callback: Callable[[Any], bool] = None,  # type: ignore
     ) -> None:
-        self._event = event
-        self._source_state = source
-        self._destination_state = destination
+        self._event: Event = event
+        self._source_state: State = source
+        self._destination_state: State = destination
 
         self._criteria: Optional[Callable[[Any], bool]] = callback
         self._action: Optional[Callable[[Any], None]] = None
 
     def __call__(self, data: Any) -> Any:
         raise NotImplementedError
 
-    def add_criteria(self, callback: Callable[[Any], bool]):
+    def add_criteria(self, callback: Callable[[Any], bool]) -> None:
         self._criteria = callback
 
-    def add_action(self, callback: Callable[[Any], Any]):
+    def add_action(self, callback: Callable[[Any], Any]) -> None:
         self._action = callback
 
     @property
-    def event(self):
+    def event(self) -> Event:
         return self._event
 
     @property
-    def source_state(self):
+    def source_state(self) -> State:
         return self._source_state
 
     @property
-    def destination_state(self):
+    def destination_state(self) -> State:
         return self._destination_state
 
 
 class FromToTransition(Transition):
     def __init__(
         self,
         event: Event,
         source: State,
         destination: State,
-        callback: Callable[[Any], bool] = None,
+        callback: Callable[[Any], bool] = None,  # type: ignore
     ) -> None:
-        super().__init__(event, source, destination, callback)
+        super().__init__(
+            event=event, source=source, destination=destination, callback=callback
+        )
 
-        self._from = source
-        self._to = destination
+        self._from: State = source
+        self._to: State = destination
 
-    def __call__(self, data: Any):
+    def __call__(self, data: Any) -> State:
         if not self._criteria or self._criteria(data):
             if self._action:
                 self._action(data)
 
-            self._from.stop(data)
-            self._to.start(data)
+            self._from.stop(data=data)
+            self._to.start(data=data)
 
             return self._to
         else:
             return self._from
 
 
 class StateMachine:
@@ -195,21 +252,21 @@
         self._states: list[State] = []
         self._events: list[Event] = []
         self._transitions: list[Transition] = []
         self._initial_state: Optional[State] = None
         self._current_state: Optional[State] = None
         self._exit_callback: Optional[Callable[[Idle, Any], None]] = None
         self._exit_state = Idle()
-        self.add_state(self._exit_state)
+        self.add_state(state=self._exit_state)
         self._initial_state = self._exit_state
 
         self._exited = True
-        self._osl = osl
+        self._osl: Any = None  # type: ignore
 
-    def add_state(self, state: State, initial_state: bool = False):
+    def add_state(self, state: State, initial_state: bool = False) -> None:
         """
         Add a state to the state machine.
 
         Parameters
         ----------
         state : State
             The state to be added.
@@ -221,23 +278,23 @@
             raise ValueError("State already exists.")
 
         self._states.append(state)
 
         if initial_state:
             self._initial_state = state
 
-    def add_event(self, event: Event):
+    def add_event(self, event: Event) -> None:
         self._events.append(event)
 
     def add_transition(
         self,
         source: State,
         destination: State,
         event: Event,
-        callback: Callable[[Any], bool] = None,
+        callback: Callable[[Any], bool] = None,  # type: ignore
     ) -> Optional[Transition]:
         """
         Add a transition to the state machine.
 
         Parameters
         ----------
         source : State
@@ -252,20 +309,22 @@
         transition = None
 
         if (
             source in self._states
             and destination in self._states
             and event in self._events
         ):
-            transition = FromToTransition(event, source, destination, callback)
+            transition = FromToTransition(
+                event=event, source=source, destination=destination, callback=callback
+            )
             self._transitions.append(transition)
 
         return transition
 
-    def update(self, data: Any = None):
+    def update(self, data: Any = None) -> None:
         validity = False
 
         if not (self._initial_state or self._current_state):
             raise ValueError("OSL isn't active.")
 
         for transition in self._transitions:
             if transition.source_state == self._current_state:
@@ -277,29 +336,30 @@
                     if self._exit_callback:
                         self._exit_callback(self._current_state, data)
 
                 validity = True
                 break
 
         if not validity:
-            self._osl.log.debug(f"Event isn't valid at {self._current_state.name}")
+            assert self._osl is not None
+            self._osl.log.debug(f"Event isn't valid at {self._current_state.name}")  # type: ignore
 
-    def start(self, data: Any = None):
+    def start(self, data: Any = None) -> None:
         if not self._initial_state:
             raise ValueError("Initial state not set.")
 
         self._current_state = self._initial_state
         self._exited = False
-        self._current_state.start(data)
+        self._current_state.start(data=data)
 
-    def stop(self, data: Any = None):
+    def stop(self, data: Any = None) -> None:
         if not (self._initial_state or self._current_state):
             raise ValueError("OSL isn't active.")
 
-        self._current_state.stop(data)
+        self._current_state.stop(data=data)  # type: ignore
         self._current_state = self._exit_state
         self._exited = True
 
     def is_on(self) -> bool:
         if self._current_state and self._current_state != self._exit_state:
             return True
         else:
@@ -314,8 +374,8 @@
 
     @property
     def states(self):
         return [state.name for state in self._states]
 
     @property
     def current_state_name(self):
-        return self.current_state.name
+        return self.current_state.name  # type: ignore
```

### Comparing `opensourceleg-1.2.2/opensourceleg/tui.py` & `opensourceleg-1.2.3/opensourceleg/tui.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,27 @@
     mblue: str = "#00274C"
     maize: str = "#FBEC5D"
 
 
 @dataclass
 class Plot:
     title: str = "plot"
-    parent: ttk.TTkFrame = None
+    parent: ttk.TTkFrame = None  # type: ignore
     object: Any = None
-    attribute: str = None
-    graph: ttk.TTkGraph = None
+    attribute: str = None  # type: ignore
+    graph: ttk.TTkGraph = None  # type: ignore
 
 
 @dataclass
 class StateVisualizer:
-    frame: ttk.TTkFrame = None
+    frame: ttk.TTkFrame = None  # type: ignore
     object: Any = None
-    attribute: str = None
-    states: dict[ttk.TTkButton] = None
-    previous_state: str = None
+    attribute: str = None  # type: ignore
+    states: dict[ttk.TTkButton] = None  # type: ignore
+    previous_state: str = None  # type: ignore
 
 
 COLORS = Colors()
 
 
 class TUI:
     """
@@ -53,28 +53,28 @@
     """
 
     def __init__(
         self,
         title: str = " Open-source Leg ",
         frequency: int = 30,
         layout: str = "horizontal",
-    ):
+    ) -> None:
         self.root_ttk = ttk.TTk()
         self.timer = ttk.TTkTimer()
-        self.dt = 1.0 / frequency
+        self.dt: float = 1.0 / frequency
 
         self._is_running = False
 
         self._layouts = {
             "horizontal": ttk.TTkHBoxLayout,
             "vertical": ttk.TTkVBoxLayout,
             "grid": ttk.TTkGridLayout,
         }
 
-        self.root_ttk.setLayout(self._layouts["grid"]())
+        self.root_ttk.setLayout(layout=self._layouts["grid"]())
 
         self._panels = {}
         self._plots = {}
         self._buttons = {}
         self._radio_buttons = {}
         self._checkboxes = {}
         self._categories = {}
@@ -90,15 +90,15 @@
             title=title,
             titleColor=ttk.TTkColor.BOLD + ttk.TTkColor.fg(COLORS.cyan),
         )
 
         self.frame.setLayout(self._layouts[layout]())
         self._panels["root"] = self.frame
 
-        self._update_callbacks: list[callable] = []
+        self._update_callbacks: list[Callable] = []  # type: ignore
 
         self.timer.timeout.connect(self.update)
         self.timer.start(1)
 
     @ttk.pyTTkSlot()
     def update(self):
         if self._plots:
@@ -138,15 +138,15 @@
                     self._state_vizualisers[_sv].previous_state = _current_state
 
         for callback in self._update_callbacks:
             callback()
 
         self.timer.start(self.dt)
 
-    def add_update_callback(self, callback: callable):
+    def add_update_callback(self, callback: Callable = lambda: None):  # type: ignore
         self._update_callbacks.append(callback)
 
     def set_active_attribute(self, attribute: str):
         self._attribute = attribute
 
     def set_plot_value(self, value: float):
         self._pvalue = [value]
@@ -227,15 +227,15 @@
 
     def add_state_visualizer(
         self,
         name: str = "state_visualizer",
         parent: str = "root",
         states: list[str] = [],
         object: Any = None,
-        attribute: str = None,
+        attribute: str = None,  # type: ignore
         layout: str = "horizontal",
         title_color: str = COLORS.white,
         border_color: str = COLORS.white,
         border: bool = True,
         show_title: bool = True,
         row: int = 0,
         col: int = 0,
@@ -267,43 +267,43 @@
             self._panels[parent].layout().addWidget(
                 _sv_frame,
             )
 
         _state_displays = {}
 
         for state in states:
-            _sv_frame.layout().addWidget(
+            _sv_frame.layout().addWidget(  # type: ignore
                 _button := ttk.TTkButton(
                     text=" ".join(state.split("_")).title(),
                     color=ttk.TTkColor.fg(title_color),
                     border=border,
                 )
             )
 
-            _button.setDisabled(True)
-            _button.setBorderColor(ttk.TTkColor.fg(COLORS.green))
+            _button.setDisabled(disabled=True)
+            _button.setBorderColor(color=ttk.TTkColor.fg(COLORS.green))
             _state_displays[state] = _button
 
         self._state_vizualisers[name] = StateVisualizer(
             frame=_sv_frame,
             object=object,
             attribute=attribute,
             states=_state_displays,
         )
 
     def add_plot(
         self,
         name: str = "plot",
         parent: str = "root",
         object=None,
-        attribute: str = None,
+        attribute: str = None,  # type: ignore
         color: str = COLORS.white,
         row: int = 0,
         col: int = 0,
-    ):
+    ) -> None:
         self._plots[name] = Plot(
             title=" ".join(name.split("_")).title(),
             parent=self._panels[parent],
             object=object,
             attribute=attribute,
             graph=ttk.TTkGraph(
                 color=ttk.TTkColor.fg(
@@ -326,15 +326,15 @@
             self._panels[parent].layout().addWidget(self._plots[name].graph)
 
     def add_dropdown(
         self,
         name: str = "dropdown",
         parent: str = "root",
         options: list[str] = [],
-        callback: callable = None,
+        callback: Callable = lambda: None,
         callback_args: list = [],
         row: int = 0,
         col: int = 0,
     ):
         if (
             self._panels[parent].layout().__class__.__name__
             == ttk.TTkGridLayout.__name__
@@ -393,15 +393,15 @@
             )
 
     def add_value(
         self,
         name: str = "value",
         parent: str = "root",
         default: int = 0,
-        callback: callable = None,
+        callback: Callable = lambda: None,
         callback_args: list = [],
         row: int = 0,
         col: int = 0,
     ):
 
         if (
             self._panels[parent].layout().__class__.__name__
@@ -432,15 +432,15 @@
                 callback_args=callback_args,
             )
 
     def add_button(
         self,
         name: str = "button",
         parent: str = "root",
-        callback: Callable = None,
+        callback: Callable = lambda: None,
         callback_args: list = [],
         color: str = COLORS.white,
         border: bool = True,
         row: int = 0,
         col: int = 0,
     ):
         _name = " ".join(name.split("_")).title()
@@ -477,15 +477,15 @@
             )
 
     def add_radio_button(
         self,
         name: str = "radio_button",
         category: str = "attributes",
         parent: str = "root",
-        callback: Callable = None,
+        callback: Callable = lambda: None,
         callback_args: list = [],
         color: str = COLORS.white,
         is_checked: bool = False,
         row: int = 0,
         col: int = 0,
     ):
         """
@@ -545,15 +545,15 @@
                 callback_args=callback_args,
             )
 
     def add_checkbox(
         self,
         name: str = "Checkbox",
         parent: str = "root",
-        callback: Callable = None,
+        callback: Callable = lambda: None,
         callback_args: list = [],
         color: str = COLORS.white,
         is_checked: bool = False,
         row: int = 0,
         col: int = 0,
     ):
         _name = " ".join(name.split("_")).title()
@@ -587,54 +587,54 @@
             # TODO: Implement a connect checkbox function
             pass
 
     def connect_button(
         self,
         name: str,
         parent: str,
-        callback: Callable = None,
+        callback: Callable = lambda: None,
         callback_args: list = [],
     ):
         self._buttons[parent + "_" + name].clicked.connect(
             lambda: callback(name=name, parent=parent, args=callback_args)
         )
 
     def connect_radio_button(
         self,
         name: str,
         parent: str,
         category: str = "attributes",
-        callback: Callable = None,
+        callback: Callable = lambda: None,
         callback_args: list = [],
     ):
         callback_args.insert(0, category)
 
         self._radio_buttons[parent + "_" + name].clicked.connect(
             lambda: callback(name=name, parent=parent, args=callback_args)
         )
 
     def connect_value(
         self,
         name: str,
         parent: str,
-        callback: Callable = None,
+        callback: Callable = lambda: None,
         callback_args: list = [],
     ):
 
         callback_args.insert(0, self._values[parent + "_" + name].text())
 
         self._values[parent + "_" + name].returnPressed.connect(
             lambda: callback(name=name, parent=parent, args=callback_args)
         )
 
     def connect_dropdown(
         self,
         name: str,
         parent: str,
-        callback: Callable = None,
+        callback: Callable = lambda: None,
         callback_args: list = [],
     ):
         callback_args.insert(0, self._dropdowns[parent + "_" + name].currentIndex())
 
         self._dropdowns[parent + "_" + name].currentIndexChanged.connect(
             lambda x: callback(name=name, parent=parent, args=callback_args)
         )
@@ -649,27 +649,15 @@
 
         self._categories[category] = name
 
     def set_value(
         self,
         **kwargs,
     ):
-
-        name = kwargs["name"]
-        parent = kwargs["parent"]
-        value = int(self._values[parent + "_" + name].text())
-
-        _name = parent + name
-
-        if "knee" in _name.lower():
-            self._knee_values[name] = value
-        elif "ankle" in _name.lower():
-            self._ankle_values[name] = value
-        else:
-            self._other_values[name] = value
+        pass
 
     def test_button(
         self,
         **kwargs,
     ):
         name = kwargs["name"]
         parent = kwargs["parent"]
```

### Comparing `opensourceleg-1.2.2/opensourceleg/units.py` & `opensourceleg-1.2.3/opensourceleg/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,28 +92,28 @@
         super().__setitem__(key, value)
 
     def __getitem__(self, key: str) -> dict:
         if key not in self:
             raise KeyError(f"Invalid key: {key}")
         return super().__getitem__(key)
 
-    def convert_to_default_units(self, value: float, attribute: str) -> None:
+    def convert_to_default_units(self, value: float, attribute: str) -> float:
         """
         convert a value from one unit to the default unit
 
         Args:
             value (float): Value to be converted
             attribute (str): Attribute to be converted
 
         Returns:
             float: Converted value in the default unit
         """
         return value * ALL_UNITS[attribute][self[attribute]]
 
-    def convert_from_default_units(self, value: float, attribute: str) -> None:
+    def convert_from_default_units(self, value: float, attribute: str) -> float:
         """
         convert a value from the default unit to another unit
 
         Args:
             value (float): Value to be converted
             attribute (str): Attribute to be converted
```

### Comparing `opensourceleg-1.2.2/opensourceleg/utilities.py` & `opensourceleg-1.2.3/opensourceleg/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,29 +41,29 @@
 
     def handle_signal(self, signum, frame):
         self.kill_now = True
 
     def get_fade(self):
         # interpolates from 1 to zero with soft fade out
         if self._kill_soon:
-            t = time.time() - self._soft_kill_time
+            t = time.time() - self._soft_kill_time  # type: ignore
             if t >= self._fade_time:
                 return 0.0
             return 1.0 - (t / self._fade_time)
         return 1.0
 
     _kill_now = False
     _kill_soon = False
 
     @property
     def kill_now(self):
         if self._kill_now:
             return True
         if self._kill_soon:
-            t = time.time() - self._soft_kill_time
+            t = time.time() - self._soft_kill_time  # type: ignore
             if t > self._fade_time:
                 self._kill_now = True
         return self._kill_now
 
     @kill_now.setter
     def kill_now(self, val):
         if val:
@@ -138,15 +138,15 @@
             dt = self.dt
         self.t0 = self.t1 = time.time() + dt
         while not self.killer.kill_now:
             ret = function_in_loop()
             if ret == 0:
                 self.stop()
             while time.time() < self.t1 and not self.killer.kill_now:
-                if signal.sigtimedwait(
+                if signal.sigtimedwait(  # type: ignore
                     [signal.SIGTERM, signal.SIGINT, signal.SIGHUP], 0
                 ):
                     self.stop()
             self.t1 += dt
 
     def stop(self):
         self.killer.kill_now = True
@@ -172,15 +172,15 @@
             time.sleep(
                 max(PRECISION_OF_SLEEP, self.t1 - time.time() - PRECISION_OF_SLEEP)
             )
             self.sleep_t_agg += time.time() - t_pre_sleep
 
         while time.time() < self.t1 and not self.killer.kill_now:
             try:
-                if signal.sigtimedwait(
+                if signal.sigtimedwait(  # type: ignore
                     [signal.SIGTERM, signal.SIGINT, signal.SIGHUP], 0
                 ):
                     self.stop()
             except AttributeError:
                 pass
 
         if self.killer.kill_now:
```

### Comparing `opensourceleg-1.2.2/pyproject.toml` & `opensourceleg-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "1.2.2"
+version = "1.2.3"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
 
@@ -23,26 +23,26 @@
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
 ]
 
+
 [virtualenvs]
 in-project = true
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
 pyserial = "^3.5"
-numpy = "^1.22.3"
 flexsea = "^8.0.1"
-sphinx = "^6.1.3"
 pytermtk = "^0.22.0a4"
 smbus2 = "^0.4.2"
+numpy = "^1.24.3"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.1"
 black = {version = "^22.3", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.10.1"}
 mypy = "^0.991"
@@ -55,15 +55,15 @@
 safety = "^1.0"
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
 pytest-cov = "^3.0.0"
 click = "8.1.3"
 py = "^1.11.0"
-
+sphinx = "^7.0.1"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py39"]
 line-length = 88
 color = true
```

### Comparing `opensourceleg-1.2.2/PKG-INFO` & `opensourceleg-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 1.2.2
+Version: 1.2.3
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
 Home-page: https://github.com/neurobionics/opensourceleg
 License: GNU GPL v3.0
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -16,19 +16,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: flexsea (>=8.0.1,<9.0.0)
-Requires-Dist: numpy (>=1.22.3,<2.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
 Requires-Dist: pytermtk (>=0.22.0a4,<0.23.0)
 Requires-Dist: smbus2 (>=0.4.2,<0.5.0)
-Requires-Dist: sphinx (>=6.1.3,<7.0.0)
 Project-URL: Repository, https://github.com/neurobionics/opensourceleg
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # opensourceleg
```

