# Comparing `tmp/readlog-1.1.4.tar.gz` & `tmp/readlog-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readlog-1.1.4.tar", last modified: Wed May 31 05:43:01 2023, max compression
+gzip compressed data, was "readlog-1.1.5.tar", last modified: Fri Jun  2 08:51:46 2023, max compression
```

## Comparing `readlog-1.1.4.tar` & `readlog-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.998133 readlog-1.1.4/
--rw-rw-rw-   0        0        0      102 2023-05-31 05:41:04.000000 readlog-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      823 2023-05-31 05:43:00.997134 readlog-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-05-30 16:19:07.000000 readlog-1.1.4/README.md
--rw-rw-rw-   0        0        0       49 2023-05-30 13:49:56.000000 readlog-1.1.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 05:43:00.998133 readlog-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-05-31 05:42:46.000000 readlog-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.985081 readlog-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.994133 readlog-1.1.4/src/readlog.egg-info/
--rw-rw-rw-   0        0        0      823 2023-05-31 05:43:00.000000 readlog-1.1.4/src/readlog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-31 05:43:00.000000 readlog-1.1.4/src/readlog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 05:43:00.000000 readlog-1.1.4/src/readlog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-31 05:43:00.000000 readlog-1.1.4/src/readlog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 05:43:00.000000 readlog-1.1.4/src/readlog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3029 2023-05-30 13:09:29.000000 readlog-1.1.4/src/readlog.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.863226 readlog-1.1.5/
+-rw-rw-rw-   0        0        0      128 2023-06-02 08:43:49.000000 readlog-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      745 2023-06-02 08:51:46.862226 readlog-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-06-02 08:50:15.000000 readlog-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.818194 readlog-1.1.5/demo/
+drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.820178 readlog-1.1.5/demo/__pycache__/
+-rw-rw-rw-   0        0        0     5361 2023-06-02 08:42:26.000000 readlog-1.1.5/demo/__pycache__/readlog.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.822178 readlog-1.1.5/demo/imgs/
+-rw-rw-rw-   0        0        0   220194 2023-06-02 08:49:13.000000 readlog-1.1.5/demo/imgs/PotEng.png
+-rw-rw-rw-   0        0        0    80925 2023-06-02 08:38:09.000000 readlog-1.1.5/demo/log.lammps
+-rw-rw-rw-   0        0        0    76031 2023-06-02 08:50:50.000000 readlog-1.1.5/demo/log_incomplete.lammps
+-rw-rw-rw-   0        0        0     1235 2023-06-02 08:51:24.000000 readlog-1.1.5/demo/plot_themo.py
+-rw-rw-rw-   0        0        0       49 2023-05-30 13:49:56.000000 readlog-1.1.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 08:51:46.863226 readlog-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-06-02 08:43:18.000000 readlog-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.825177 readlog-1.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.859223 readlog-1.1.5/src/readlog.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-06-02 08:51:46.000000 readlog-1.1.5/src/readlog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-06-02 08:51:46.000000 readlog-1.1.5/src/readlog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 08:51:46.000000 readlog-1.1.5/src/readlog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-02 08:51:46.000000 readlog-1.1.5/src/readlog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 08:51:46.000000 readlog-1.1.5/src/readlog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3000 2023-06-02 08:51:40.000000 readlog-1.1.5/src/readlog.py
```

### Comparing `readlog-1.1.4/setup.py` & `readlog-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'readlog',
-version      = '1.1.4',
+version      = '1.1.5',
 py_modules   = ['readlog'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/readlog',
```

### Comparing `readlog-1.1.4/src/readlog.py` & `readlog-1.1.5/src/readlog.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,54 +40,56 @@
 		# print(thermou_list,thermod_list)
 		print("Tot number of line:",self.tot_line_number)
 		for i in range(len(thermou_list)):
 			try:
 				print("Frame-"+str(i)+":","["+str(thermou_list[i])+",",str(thermod_list[i])+"]")
 			except:
 				print("Frame-"+str(i)+":","["+str(thermou_list[i])+", ~]")
-				print("Your logfile is incomplete..., please check it.")
+				print("Warning: Your logfile is incomplete..., please check it.")
 
 		return thermou_list,thermod_list
 
 	def ReadThermo(self,LogFile,thermou_list,thermod_list,nf_log=0):
 		L_u = len(thermou_list)
 		L_d = len(thermod_list)
 
 		for i in range(L_u):
-			if i==L_u-1:
-				n_line = self.tot_line_number-1-thermou_list[i]-1
-			else:
+			if L_u == L_d:
 				n_line = thermod_list[i]-thermou_list[i]-1
+			elif L_u>L_d:
+				if i==L_u-1:
+					n_line = self.tot_line_number-1-thermou_list[i]-1
+
 			if nf_log==i:
 				thermo_col = np.loadtxt(LogFile,dtype="str",encoding='utf-8',skiprows=thermou_list[i]-1,max_rows=1)
 				thermo_data = np.loadtxt(LogFile,skiprows=thermou_list[i],max_rows=n_line,encoding='utf-8')#.reshape((1,-1))
 				pd_thermo = pd.DataFrame(thermo_data,columns=thermo_col)
 			else:
 				pass
 		return pd_thermo
 
-# if __name__ == '__main__':
-# 	path = "./"
-# 	logfile = "1_hydrate_dissociation_log.lammps"
-# 	atm2mPa = 0.101325
-# 	nf_log = 3 # The number of logs in logfile
-
-# 	Path(path+"imgs/").mkdir(parents=True,exist_ok=True)
-# 	rl = ReadLog(path+logfile) 
-# 	print("*",20*"-","Reading frames of themo",20*"-","*")
-# 	thermou_list,thermod_list = rl.ReadUD(path+logfile)
-# 	pd_thermo = rl.ReadThermo(path+logfile,thermou_list,thermod_list,nf_log)
-# 	print("Your label list of thermo :\n",pd_thermo.columns)
-# 	print("*",20*"-","Reading END!!!!!!!!!!!!",20*"-","*")
-# 	plt.rc('font', family='Times New Roman', size=22)
-# 	fig = plt.figure(figsize=(12, 10))
-# 	ax = fig.add_subplot(1,1,1)
-# 	ax.plot(pd_thermo["Step"]*1e-3,pd_thermo['PotEng'],color='r',label="PotEng")
-# 	plt.legend(loc="best")
-# 	# ax.set_xlim([0,10000])
-# 	# ax.set_ylim([-800,800])
-# 	ax.set_xlabel("Time (ps)")
-# 	ax.set_ylabel("PotEng (kcal/mol)")
-# 	# ax.grid(True)
+if __name__ == '__main__':
+	path = "./"
+	logfile = "log.lammps"
+	atm2mPa = 0.101325
+	nf_log = 0 # The number of logs in logfile
+
+	# Path(path+"imgs/").mkdir(parents=True,exist_ok=True)
+	rl = ReadLog(path+logfile) 
+	print("*",20*"-","Reading frames of themo",20*"-","*")
+	thermou_list,thermod_list = rl.ReadUD(path+logfile)
+	pd_thermo = rl.ReadThermo(path+logfile,thermou_list,thermod_list,nf_log)
+	print("Your label list of thermo :\n",pd_thermo.columns)
+	print("*",20*"-","Reading END!!!!!!!!!!!!",20*"-","*")
+	plt.rc('font', family='Times New Roman', size=22)
+	fig = plt.figure(figsize=(12, 10))
+	ax = fig.add_subplot(1,1,1)
+	ax.plot(pd_thermo["Step"]*1e-3,pd_thermo['PotEng'],color='r',label="PotEng")
+	plt.legend(loc="best")
+	# ax.set_xlim([0,10000])
+	# ax.set_ylim([-800,800])
+	ax.set_xlabel("Time (ps)")
+	ax.set_ylabel("PotEng (kcal/mol)")
+	# ax.grid(True)
 	
-# 	# plt.savefig(path+"imgs/PressTemp.png",dpi=300)
-# 	plt.show()		
+	# plt.savefig(path+"imgs/PressTemp.png",dpi=300)
+	plt.show()
```

