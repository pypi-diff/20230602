# Comparing `tmp/pykrak-1.0.1.tar.gz` & `tmp/pykrak-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykrak-1.0.1.tar", last modified: Wed Apr 19 00:50:29 2023, max compression
+gzip compressed data, was "pykrak-2.0.1.tar", last modified: Fri Jun  2 20:30:09 2023, max compression
```

## Comparing `pykrak-1.0.1.tar` & `pykrak-2.0.1.tar`

### file list

```diff
@@ -1,22 +1,49 @@
-drwxrwxr-x   0 hunter    (1001) hunter    (1001)        0 2023-04-19 00:50:29.488679 pykrak-1.0.1/
--rw-rw-r--   0 hunter    (1001) hunter    (1001)      375 2023-04-19 00:50:29.488679 pykrak-1.0.1/PKG-INFO
--rw-rw-r--   0 hunter    (1001) hunter    (1001)    35149 2023-04-19 00:32:05.000000 pykrak-1.0.1/license.txt
-drwxrwxr-x   0 hunter    (1001) hunter    (1001)        0 2023-04-19 00:50:29.488679 pykrak-1.0.1/pykrak/
--rw-rw-r--   0 hunter    (1001) hunter    (1001)     4590 2023-04-19 00:32:05.000000 pykrak-1.0.1/pykrak/attn_pert.py
--rw-rw-r--   0 hunter    (1001) hunter    (1001)    17014 2023-04-19 00:40:37.000000 pykrak-1.0.1/pykrak/coupled_modes.py
--rw-rw-r--   0 hunter    (1001) hunter    (1001)     3123 2023-04-19 00:32:05.000000 pykrak-1.0.1/pykrak/group_pert.py
--rw-rw-r--   0 hunter    (1001) hunter    (1001)     5591 2023-04-19 00:41:23.000000 pykrak-1.0.1/pykrak/inverse_iteration.py
--rw-rw-r--   0 hunter    (1001) hunter    (1001)    10707 2023-04-19 00:32:05.000000 pykrak-1.0.1/pykrak/mesh_routines.py
--rw-rw-r--   0 hunter    (1001) hunter    (1001)     1583 2023-04-19 00:41:29.000000 pykrak-1.0.1/pykrak/misc.py
--rw-rw-r--   0 hunter    (1001) hunter    (1001)    12195 2023-04-19 00:41:26.000000 pykrak-1.0.1/pykrak/pressure_calc.py
--rw-rw-r--   0 hunter    (1001) hunter    (1001)    18750 2023-04-19 00:41:50.000000 pykrak-1.0.1/pykrak/pynm_env.py
--rw-rw-r--   0 hunter    (1001) hunter    (1001)     5077 2023-04-19 00:32:05.000000 pykrak-1.0.1/pykrak/shooting_routines.py
--rw-rw-r--   0 hunter    (1001) hunter    (1001)    11164 2023-04-19 00:41:41.000000 pykrak-1.0.1/pykrak/sturm_seq.py
-drwxrwxr-x   0 hunter    (1001) hunter    (1001)        0 2023-04-19 00:50:29.488679 pykrak-1.0.1/pykrak.egg-info/
--rw-rw-r--   0 hunter    (1001) hunter    (1001)      375 2023-04-19 00:50:29.000000 pykrak-1.0.1/pykrak.egg-info/PKG-INFO
--rw-rw-r--   0 hunter    (1001) hunter    (1001)      402 2023-04-19 00:50:29.000000 pykrak-1.0.1/pykrak.egg-info/SOURCES.txt
--rw-rw-r--   0 hunter    (1001) hunter    (1001)        1 2023-04-19 00:50:29.000000 pykrak-1.0.1/pykrak.egg-info/dependency_links.txt
--rw-rw-r--   0 hunter    (1001) hunter    (1001)       29 2023-04-19 00:50:29.000000 pykrak-1.0.1/pykrak.egg-info/requires.txt
--rw-rw-r--   0 hunter    (1001) hunter    (1001)        7 2023-04-19 00:50:29.000000 pykrak-1.0.1/pykrak.egg-info/top_level.txt
--rw-rw-r--   0 hunter    (1001) hunter    (1001)      108 2023-04-19 00:50:29.488679 pykrak-1.0.1/setup.cfg
--rw-rw-r--   0 hunter    (1001) hunter    (1001)      577 2023-04-19 00:49:41.000000 pykrak-1.0.1/setup.py
+drwxrwxr-x   0 hunter    (1001) hunter    (1001)        0 2023-06-02 20:30:09.008449 pykrak-2.0.1/
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    35149 2023-06-02 20:14:30.000000 pykrak-2.0.1/LICENSE
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)      377 2023-06-02 20:30:09.008449 pykrak-2.0.1/PKG-INFO
+drwxrwxr-x   0 hunter    (1001) hunter    (1001)        0 2023-06-02 20:30:09.004449 pykrak-2.0.1/pykrak/
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)        0 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/__init__.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    23139 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/adjoint.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     6797 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/attn_pert.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    17014 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/coupled_modes.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    11260 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/env_pert.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)      949 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/env_test.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    47076 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/envs.py
+drwxrwxr-x   0 hunter    (1001) hunter    (1001)        0 2023-06-02 20:30:09.004449 pykrak-2.0.1/pykrak/examples/
+drwxrwxr-x   0 hunter    (1001) hunter    (1001)        0 2023-06-02 20:30:09.008449 pykrak-2.0.1/pykrak/examples/at_files/
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    17821 2023-06-02 20:17:32.000000 pykrak-2.0.1/pykrak/examples/at_files/iso.env
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)  2251600 2023-06-02 20:17:32.000000 pykrak-2.0.1/pykrak/examples/at_files/iso.mod
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    18795 2023-06-02 20:17:32.000000 pykrak-2.0.1/pykrak/examples/at_files/iso.prt
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     1666 2023-06-02 20:19:29.000000 pykrak-2.0.1/pykrak/examples/pekeris.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     2306 2023-06-02 20:19:29.000000 pykrak-2.0.1/pykrak/examples/raw_pekeris.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     3719 2023-06-02 20:19:29.000000 pykrak-2.0.1/pykrak/examples/raw_swell.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     3719 2023-06-02 20:19:29.000000 pykrak-2.0.1/pykrak/examples/swell.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     3123 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/group_pert.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     5546 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/inverse_iteration.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    35149 2023-06-02 20:17:32.000000 pykrak-2.0.1/pykrak/license.txt
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    11442 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/likelihoods.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    10849 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/mesh_routines.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     2310 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/misc.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)      902 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/pekeris_test.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    19662 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/pressure_calc.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    18849 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/pykrak_env.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     2065 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/raw_pykrak.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     1447 2023-06-02 20:17:32.000000 pykrak-2.0.1/pykrak/readme
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)      544 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/setup.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     5077 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/shooting_routines.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    12932 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/sturm_seq.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)    11265 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/swell_pert.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     2251 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/test_helpers.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     1440 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/wave_helpers.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     5449 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/wave_inverse_iteration.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     2353 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/wave_mesh_routines.py
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     6371 2023-06-02 20:18:47.000000 pykrak-2.0.1/pykrak/wave_sturm_seq.py
+drwxrwxr-x   0 hunter    (1001) hunter    (1001)        0 2023-06-02 20:30:09.004449 pykrak-2.0.1/pykrak.egg-info/
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)      377 2023-06-02 20:30:08.000000 pykrak-2.0.1/pykrak.egg-info/PKG-INFO
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)      981 2023-06-02 20:30:08.000000 pykrak-2.0.1/pykrak.egg-info/SOURCES.txt
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)        1 2023-06-02 20:30:08.000000 pykrak-2.0.1/pykrak.egg-info/dependency_links.txt
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)       29 2023-06-02 20:30:08.000000 pykrak-2.0.1/pykrak.egg-info/requires.txt
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)        7 2023-06-02 20:30:08.000000 pykrak-2.0.1/pykrak.egg-info/top_level.txt
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)     1502 2023-06-02 20:14:30.000000 pykrak-2.0.1/readme.txt
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)      104 2023-06-02 20:30:09.008449 pykrak-2.0.1/setup.cfg
+-rw-rw-r--   0 hunter    (1001) hunter    (1001)      579 2023-06-02 20:29:45.000000 pykrak-2.0.1/setup.py
```

### Comparing `pykrak-1.0.1/license.txt` & `pykrak-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pykrak-1.0.1/pykrak/coupled_modes.py` & `pykrak-2.0.1/pykrak/coupled_modes.py`

 * *Files identical despite different names*

### Comparing `pykrak-1.0.1/pykrak/group_pert.py` & `pykrak-2.0.1/pykrak/group_pert.py`

 * *Files identical despite different names*

### Comparing `pykrak-1.0.1/pykrak/inverse_iteration.py` & `pykrak-2.0.1/pykrak/inverse_iteration.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,14 @@
     # last value is cut in half (since its an interface pt ?
     depth_val = h*np.square(phi[depth_ind,:]) / rho[-1] / om_sq 
     layer_norm_sq += depth_val #
     return layer_norm_sq, depth_ind
 
 @njit
 def normalize_phi(phi, krs, omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs):
-    A_size = get_A_size_numba(z_arr, ind_arr)
     num_layers = ind_arr.size
     num_modes = phi.shape[-1]
     om_sq = np.square(omega)
     norm_sq = np.zeros(num_modes)
     depth_ind = 0
     """ Use trapezoid rule to integrate each layer"""
     for j in range(num_layers):
@@ -172,10 +171,10 @@
     h0 = h_arr[0]
     for i in range(len(krs)):
         kr = krs[i]
         lam = np.square(h0*kr)
         a, e1, d1 = get_A_numba(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam)
         eig = inverse_iter(a, e1, d1, lam)
         phi[1:,i] = eig
-    phi = normalize_phi(phi, krs,omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs) 
+    phi = normalize_phi(phi, krs, omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs) 
     return phi
```

### Comparing `pykrak-1.0.1/pykrak/mesh_routines.py` & `pykrak-2.0.1/pykrak/mesh_routines.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,19 @@
 rc('text', usetex=True)
 import matplotlib
 matplotlib.rcParams['mathtext.fontset'] = 'stix'
 matplotlib.rcParams['font.family'] = 'STIXGeneral'
 import numba as nb
 from numba import njit
 
-@njit(nb.f8[:](nb.f8, nb.f8, nb.f8[:], nb.f8[:], nb.f8))
+
+float_arr_type = nb.types.Array(nb.f8, 1, 'A', readonly=True)
+int_arr_type = nb.types.Array(nb.i8, 1, 'A', readonly=True)
+
+@njit(float_arr_type(nb.f8, nb.f8, float_arr_type, float_arr_type, nb.f8))
 def get_a(omega, h, c, rho, h0):
     """
     Compute the diagonal elements a used for depths within a layer
     For the pseudo-Sturm Liouville problem
     I use the layer mesh scaling so that multiple layers can be used with different
     meshes and operate on the same eigenvalue kr^2 h0^2
     which results in
```

### Comparing `pykrak-1.0.1/pykrak/pynm_env.py` & `pykrak-2.0.1/pykrak/pykrak_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,15 @@
 
         # loop over meshes
         for i in range(Nh):  # (max) num Richardson mesh refinements
 
             # refine mesh
             factor = int(np.power(2.0, i))
             curr_N_list = [(x-1)*factor+1 for x in N_list]
+            #print('curr_N_list', curr_N_list)
             tmp_z_list, tmp_c_list, tmp_rho_list, tmp_attn_list = self.interp_env_vals(curr_N_list)
             curr_h_list = [x[1] - x[0] for x in tmp_z_list]
             h_arr, ind_arr, z_arr, c_arr, rho_arr = get_arrs(curr_h_list, tmp_z_list, tmp_c_list, tmp_rho_list)
             h0 = h_arr[0]
 
             # get wavenumbers for this mesh
             lam_min = np.square(h0*kr_min) 
@@ -348,14 +349,15 @@
             else: # manual grid number
                 pass
             z_list, c_list, rho_list, attn_list = self.interp_env_vals(N_list)
             h_list = [x[1] - x[0] for x in z_list]
             h_arr, ind_arr, z_arr, c_arr, rho_arr = get_arrs(h_list, z_list, c_list, rho_list)
             phi = get_phi(krs, self.omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, self.c_hs, self.rho_hs)
         self.phi = phi
+        self.get_phi_z(N_list)
         return phi
 
     def get_phi_z(self, N_list=None):
         """
         Get grid of depths at which the mode functions are evaluated
         """
         # N_list is an optional argument that allows you to specify the number of points in each layer
@@ -368,14 +370,15 @@
             z = self.z_list[i]
             mesh_z = np.linspace(z[0], z[-1], N)
             if i == 0:
                 phi_z = mesh_z
             else:
                 """layers share end interface dpeths"""
                 phi_z = np.concatenate((phi_z, mesh_z[1:])) 
+        self.phi_z = phi_z
         return phi_z
 
     def get_rho_grid(self, N_list=None):
         """
         Get rho at values of mesh used
         N_list is an optional argument that allows you to specify the number of points in each layer
         """
@@ -397,15 +400,15 @@
     def get_phi_zr(self, zr):
         """ Get modes evaluated at depths zr"""
         phi = self.phi
         if np.all(phi==0):
             phi = self.get_phi()
         M = phi.shape[-1]
         phi_zr = np.zeros((zr.size, M))
-        phi_z = self.get_phi_z()
+        phi_z = self.phi_z
         for i in range(M):
             phi_zr[:,i] = np.interp(zr, phi_z, phi[:,i])
         return phi_zr
 
     def get_ugs(self, N_list=None):
         """ Get group speeds of modes """
         if type(N_list) == type(None):# use lambda / 20
```

### Comparing `pykrak-1.0.1/pykrak/shooting_routines.py` & `pykrak-2.0.1/pykrak/shooting_routines.py`

 * *Files identical despite different names*

### Comparing `pykrak-1.0.1/pykrak/sturm_seq.py` & `pykrak-2.0.1/pykrak/sturm_seq.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
+float_arr_type = nb.types.Array(nb.f8, 1, 'A', readonly=True)
+int_arr_type = nb.types.Array(nb.i8, 1, 'A', readonly=True)
+
 @njit
 def get_scale(seq, j, Phi=1e8, Gamma=1e-8):
     """
     For rescaling sturm sequence
     """
     seq_val = abs(seq[j])
     seq_prev_val = abs(seq[j-1])
@@ -100,53 +103,53 @@
     Get the environmental description from a list of arrays
     to a single array
     """
     num_arrs = len(list_of_arrs)
     final_arr = list_of_arrs[0]
     ind_arr = np.zeros(num_arrs, dtype=int)
     for i in range(1, num_arrs):
-        ind_arr[i] = final_arr.size
+        ind_arr[i] = final_arr.size # index to access the first entry in ith layer
         final_arr = np.concatenate((final_arr, list_of_arrs[i]))
     return final_arr, ind_arr
 
 def get_arrs(h_list, z_list, c_list, rho_list):
     """
     Convert env_lists to arrays for numba-ing
     """
     h_arr = np.array(h_list)
     z_arr, ind_arr = cat_list_to_arr(z_list)
     c_arr, ind_arr = cat_list_to_arr(c_list)
     rho_arr, ind_arr = cat_list_to_arr(rho_list)
     return h_arr, ind_arr, z_arr, c_arr, rho_arr
     
-@njit(nb.f8(nb.f8, nb.f8[:], nb.i8[:], nb.f8[:], nb.f8[:], nb.f8[:], nb.f8, nb.f8, nb.f8))
+@njit(nb.f8(nb.f8, float_arr_type, int_arr_type, float_arr_type, float_arr_type, float_arr_type, nb.f8, nb.f8, nb.f8))
 def get_sturm_seq(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam):
     """
     Compute sturm sequence  for given parameters
     Return final element and number of eigenvalues greater than lam
     """
 
     a_diag, e1, d1 = get_A_numba(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam)
     
     sturm_seq, count = sturm_subroutine(a_diag, e1, d1, lam)
     return sturm_seq[-1]
 
-@njit(nb.f8[:](nb.f8, nb.f8[:], nb.i8[:], nb.f8[:], nb.f8[:], nb.f8[:], nb.f8, nb.f8, nb.f8))
+@njit(float_arr_type(nb.f8, float_arr_type, int_arr_type, float_arr_type, float_arr_type, float_arr_type, nb.f8, nb.f8, nb.f8))
 def get_sturm_seq_count(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam):
     """
     Compute sturm sequence  for given parameters
     Return final element and number of eigenvalues greater than lam
     """
 
     a_diag, e1, d1 = get_A_numba(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam)
     
     sturm_seq, count = sturm_subroutine(a_diag, e1, d1, lam)
     return np.array([sturm_seq[-1], count])
 
-@njit(nb.f8(nb.f8, nb.f8[:], nb.i8[:], nb.f8[:], nb.f8[:], nb.f8[:], nb.f8, nb.f8, nb.f8, nb.f8, nb.f8))
+@njit(nb.f8(nb.f8, float_arr_type, int_arr_type, float_arr_type, float_arr_type, float_arr_type, nb.f8, nb.f8, nb.f8, nb.f8, nb.f8))
 def layer_brent(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, a, b, t):
     """
       Licensing:
     
         This code is distributed under the GNU LGPL license.
     
       Modified:
@@ -241,33 +244,20 @@
             fc = fa
             e = sb - sa
             d = e
 
     value = sb
     return value
 
+@njit
 def find_root(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam_min, lam_max):
-    try:
-        tol = 1e-16 # close to machine precision
-        root = layer_brent(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam_min, lam_max, tol)
-    except ValueError:
-        kr_left = np.sqrt(lam_min)/h_arr[0]
-        kr_right = np.sqrt(lam_max)/h_arr[0]
-        print(kr_left, kr_right, omega/1500)
-        print('c eff', omega / kr_left )
-        print('c eff', omega / kr_right )
-        raise ValueError
-    if root == 0:
-        x = np.linspace(lam_min, lam_max, 100)
-        plt.figure()
-        plt.plot([fun(i) for i in x])
-        plt.show()
-        raise ValueError('brent returned 0. lam min, lam_max = ', lam_min, lam_max, root) 
+    tol = 1e-16 # close to machine precision
+    root = layer_brent(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam_min, lam_max, tol)
     return root
-        
+    
 def get_krs(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam_min, lam_max, N=-1, Nr_max=-1):
     """
     Recursively bisect the domain, counting the modes in each 
     subdomain and employing Brentq root finder once the number 
     of modes has been isolated
     """
     if z_arr[0] != 0:
@@ -321,7 +311,65 @@
             kr_right = find_root(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam, lam_max)
             kr_right = np.sqrt(kr_right)/h0
             return kr_left+ [kr_right]
         else:
             #kr_right = get_krs(omega, h, z, c, rhow, cb, rhob, avec, lam, lam_max, N-sub_Nl, Nr_max=Nr_max)
             kr_right = get_krs(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam, lam_max, N-sub_Nl, Nr_max=Nr_max)
             return kr_left+ kr_right
+
+@njit
+def get_comp_krs(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam_min, lam_max):
+    """
+    Recursively bisect the domain, counting the modes in each 
+    subdomain and employing Brentq root finder once the number 
+    of modes has been isolated
+    """
+    h0 = h_arr[0]
+    dz0 = z_arr[1] - z_arr[0]
+    det, Nr = get_sturm_seq_count(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam_max)
+
+    det, Nl = get_sturm_seq_count(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam_min)
+    M = int(Nl - Nr)
+
+
+    
+    max_num_bisections = 50
+    
+    lam_l = lam_min*np.ones((M))
+    lam_r = lam_max*np.ones((M))
+
+    krs = np.zeros((M))
+    for i in range(M-1):
+        lam1 = lam_l[i] 
+        lam2 = lam_r[i]
+
+        for k in range(max_num_bisections):
+            lam_prop = .5*(lam1 + lam2)
+            det, N = get_sturm_seq_count(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam_prop)
+
+            Nz = N - Nr # number of zeros in interval from lam_prop to lam_max
+            if Nz < i + 1: # move the right boundary
+                lam2 = lam_prop
+                lam_r[i] = lam_prop
+            else: # move the left boundary
+                lam1 = lam_prop
+                # also give the clue to all coming modes
+                for mode_i in range(i, M):
+                    if Nz >= mode_i+1:
+                        lam_l[mode_i] = lam_prop
+                    if Nz < mode_i + 1:
+                        lam_r[mode_i] = lam_prop
+            if Nz == i +1: # found the right interval  
+                # lam_prop is the left boundary
+                lam_l[i] = lam_prop
+                lam_r[i+1] = lam_prop
+                break
+        root = find_root(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam_l[i], lam_r[i])
+        krs[i] = np.sqrt(root)/h0
+    root = find_root(omega, h_arr, ind_arr, z_arr, c_arr, rho_arr, c_hs, rho_hs, lam_l[M-1], lam_r[M-1])
+    krs[M-1] = np.sqrt(root)/h0
+    krs = krs[::-1]
+    return krs
+
+
+
+
```

### Comparing `pykrak-1.0.1/setup.py` & `pykrak-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 
 setup(
     name="pykrak",
-    version="1.0.1",
+    version="2.0.1",
     description="Normal mode wave equation solver for stratified fluids",
-    url="https://github.com/hunterakins/pynm",
+    url="https://github.com/hunterakins/pykrak",
     author="F. Hunter Akins",
     author_email="fakins@ucsd.edu",
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
     ],
     packages=["pykrak"],
     python_requires=">=3.7, <4",
```

