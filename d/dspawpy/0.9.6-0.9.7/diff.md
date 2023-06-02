# Comparing `tmp/dspawpy-0.9.6-py3-none-any.whl.zip` & `tmp/dspawpy-0.9.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 72855 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-26 05:38 dspawpy/__init__.py
+Zip file size: 73209 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-02 08:47 dspawpy/__init__.py
 -rw-rw-rw-  2.0 fat    29208 b- defN 23-May-23 06:07 dspawpy/plot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/analysis/__init__.py
--rw-rw-rw-  2.0 fat    21567 b- defN 23-May-23 06:07 dspawpy/analysis/aimdtools.py
+-rw-rw-rw-  2.0 fat    23645 b- defN 23-Jun-02 08:45 dspawpy/analysis/aimdtools.py
 -rw-rw-rw-  2.0 fat    20152 b- defN 23-May-23 06:07 dspawpy/analysis/vacf.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 06:07 dspawpy/diffusion/__init__.py
--rw-rw-rw-  2.0 fat     3592 b- defN 23-May-23 06:07 dspawpy/diffusion/neb.py
--rw-rw-rw-  2.0 fat    53467 b- defN 23-May-23 06:07 dspawpy/diffusion/nebtools.py
+-rw-rw-rw-  2.0 fat     3270 b- defN 23-Jun-02 08:39 dspawpy/diffusion/neb.py
+-rw-rw-rw-  2.0 fat    53498 b- defN 23-Jun-02 08:45 dspawpy/diffusion/nebtools.py
 -rw-rw-rw-  2.0 fat    11045 b- defN 23-May-23 06:07 dspawpy/diffusion/pathfinder.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 08:25 dspawpy/io/__init__.py
 -rw-rw-rw-  2.0 fat    53355 b- defN 23-May-23 06:07 dspawpy/io/read.py
 -rw-rw-rw-  2.0 fat     7721 b- defN 23-May-23 06:07 dspawpy/io/read_json.py
 -rw-rw-rw-  2.0 fat     9880 b- defN 23-May-23 06:07 dspawpy/io/structure.py
 -rw-rw-rw-  2.0 fat    25239 b- defN 23-May-23 06:07 dspawpy/io/utils.py
--rw-rw-rw-  2.0 fat    25391 b- defN 23-May-23 06:07 dspawpy/io/write.py
+-rw-rw-rw-  2.0 fat    26180 b- defN 23-Jun-02 08:46 dspawpy/io/write.py
 -rw-rw-rw-  2.0 fat     1761 b- defN 23-May-23 06:07 dspawpy/io/write_json.py
--rw-rw-rw-  2.0 fat     2904 b- defN 23-May-26 05:39 dspawpy-0.9.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-26 05:39 dspawpy-0.9.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-26 05:39 dspawpy-0.9.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1582 b- defN 23-May-26 05:39 dspawpy-0.9.6.dist-info/RECORD
-20 files, 266987 bytes uncompressed, 70305 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     3075 b- defN 23-Jun-02 08:47 dspawpy-0.9.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 08:47 dspawpy-0.9.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-02 08:47 dspawpy-0.9.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1582 b- defN 23-Jun-02 08:47 dspawpy-0.9.7.dist-info/RECORD
+20 files, 269734 bytes uncompressed, 70659 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: dspawpy/io/write.py
 Comment: 
 
 Filename: dspawpy/io/write_json.py
 Comment: 
 
-Filename: dspawpy-0.9.6.dist-info/METADATA
+Filename: dspawpy-0.9.7.dist-info/METADATA
 Comment: 
 
-Filename: dspawpy-0.9.6.dist-info/WHEEL
+Filename: dspawpy-0.9.7.dist-info/WHEEL
 Comment: 
 
-Filename: dspawpy-0.9.6.dist-info/top_level.txt
+Filename: dspawpy-0.9.7.dist-info/top_level.txt
 Comment: 
 
-Filename: dspawpy-0.9.6.dist-info/RECORD
+Filename: dspawpy-0.9.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspawpy/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.9.6"
+__version__ = "0.9.7"
```

## dspawpy/analysis/aimdtools.py

```diff
@@ -179,15 +179,17 @@
             species = [species]
         ref_species_index = []
         species_index = []
         for i in range(len(self.structures[0].species)):
             ele = str(self.structures[0].species[i])
             if ele in ref_species:
                 ref_species_index.append(i)
-            elif ele in species:
+            if (
+                ele in species
+            ):  # @syyl use if instead of elif in case of `species = ref_species`
                 species_index.append(i)
         all_rdfs = [
             self.get_one_rdf(ref_species_index, species_index, i)[1]
             for i in range(self.n_structures)
         ]
         if is_average:
             all_rdfs = np.mean(all_rdfs, axis=0)
@@ -288,15 +290,15 @@
 
 def get_lagtime_msd(
     datafile: Union[str, List[str]],
     select: Union[str, List[int]] = "all",
     msd_type: str = "xyz",
     timestep: float = 1.0,
 ):
-    """计算不同时间步长下的均方差
+    r"""计算不同时间步长下的均方差
 
     Parameters
     ----------
     datafile : str or list of str
         aimd.h5或aimd.json文件或包含这两个文件之一的文件夹；
         写成列表的话将依次读取数据并合并到一起
     select : str or list of int
@@ -313,39 +315,36 @@
         时间序列
     result : np.ndarray
         均方差序列
 
     Examples
     --------
     >>> from dspawpy.analysis.aimdtools import get_lagtime_msd
-    >>> lagtime, msd = get_lagtime_msd(datafile='aimd.h5', select='all', msd_type='xyz', timestep=1.0)
+    >>> lagtime, msd = get_lagtime_msd(datafile='test/aimd.h5', select='all', msd_type='xyz', timestep=1.0)
+    Reading E:\Dev\dspawpy\test\aimd.h5 ...
+    Calculating MSD...
     >>> lagtime
-    array([  0.,   1.,   2.,   3.,   4.,   5.,   6.,   7.,   8.,   9.,  10.,
-            11.,  12.,  13.,  14.,  15.,  16.,  17.,  18.,  19.,  20.,  21.,
-            ...,
-            990., 991., 992., 993., 994., 995., 996., 997., 998., 999.])
+    array([0., 1., 2., 3., 4., 5., 6., 7., 8., 9.])
     >>> msd
-    array([   0.        ,   67.07025573,  132.46384987,  193.1025821 ,
-            250.1513171 ,  301.71988034,  349.76713326,  397.42586668,
-            ...,
-            1092.833737  , 1067.50385434, 1009.90265319, 1206.1645769 ])
+    array([0.        , 0.00234419, 0.00872255, 0.01706176, 0.02451864,
+           0.02963004, 0.03378312, 0.0395548 , 0.04852066, 0.0596252 ])
     """
     strs = build_Structures_from_datafile(datafile)
 
     msd = MSD(strs, select, msd_type)
     result = msd.run()
 
     nframes = msd.n_frames
     lagtime = np.arange(nframes) * timestep  # make the lag-time axis
 
     return lagtime, result
 
 
 def get_lagtime_rmsd(datafile: Union[str, List[str]], timestep: float = 1.0):
-    """
+    r"""
 
     Parameters
     ----------
     datafile : str or list of str
         aimd.h5或aimd.json文件或包含这两个文件之一的文件夹；
         写成列表的话将依次读取数据并合并到一起
     timestep : float
@@ -357,25 +356,22 @@
         时间序列
     rmsd : numpy.ndarray
         均方根序列
 
     Examples
     --------
     >>> from dspawpy.analysis.aimdtools import get_lagtime_rmsd
-    >>> lagtime, rmsd = get_lagtime_rmsd(datafile='aimd.h5', timestep=1.0)
+    >>> lagtime, rmsd = get_lagtime_rmsd(datafile='test/aimd.h5', timestep=1.0)
+    Reading E:\Dev\dspawpy\test\aimd.h5 ...
+    Calculating RMSD...
     >>> lagtime
-    array([  0.,   1.,   2.,   3.,   4.,   5.,   6.,   7.,   8.,   9.,  10.,
-            11.,  12.,  13.,  14.,  15.,  16.,  17.,  18.,  19.,  20.,  21.,
-            ...,
-            990., 991., 992., 993., 994., 995., 996., 997., 998., 999.])
+    array([0., 1., 2., 3., 4., 5., 6., 7., 8., 9.])
     >>> rmsd
-    array([ 0.        , 19.61783543, 19.62557403, 19.63797614, 19.65407193,
-            27.77329091, 27.7898651 , 19.72260788,  2.34196454,  2.62175006,
-            ...,
-            43.97237636, 39.57388473, 39.67579857, 34.61880282, 34.72988017])
+    array([0.        , 0.03987827, 0.06727018, 0.09707005, 0.14068665,
+           0.1778412 , 0.18981011, 0.19410218, 0.21498126, 0.24418271])
     """
     strs = build_Structures_from_datafile(datafile)
 
     rmsd = RMSD(structures=strs)
     result = rmsd.run()
 
     # Plot
@@ -390,15 +386,15 @@
     ele1: str,
     ele2: str,
     rmin: float = 0,
     rmax: float = 10,
     ngrid: float = 101,
     sigma: float = 0,
 ):
-    """计算rdf分布函数
+    r"""计算rdf分布函数
 
     Parameters
     ----------
     datafile : str or list of str
         aimd.h5或aimd.json文件路径或包含这两个文件之一的文件夹；
         写成列表的话将依次读取数据并合并到一起
     ele1 : list
@@ -420,25 +416,50 @@
         径向分布网格点
     rdf : numpy.ndarray
         径向分布函数
 
     Examples
     --------
     >>> from dspawpy.analysis.aimdtools import get_rs_rdfs
-    >>> rs, rdfs = get_rs_rdfs(datafile='aimd.h5', ele1='H', ele2='O', rmin=0, rmax=10, ngrid=101, sigma=0)
+    >>> rs, rdfs = get_rs_rdfs(datafile='test/aimd.h5', ele1='H', ele2='O', rmin=0, rmax=10, ngrid=101, sigma=0)
+    Reading E:\Dev\dspawpy\test\aimd.h5 ...
+    Calculating RDF...
     >>> rs
     array([ 0. ,  0.1,  0.2,  0.3,  0.4,  0.5,  0.6,  0.7,  0.8,  0.9,  1. ,
             1.1,  1.2,  1.3,  1.4,  1.5,  1.6,  1.7,  1.8,  1.9,  2. ,  2.1,
-            ...,
+            2.2,  2.3,  2.4,  2.5,  2.6,  2.7,  2.8,  2.9,  3. ,  3.1,  3.2,
+            3.3,  3.4,  3.5,  3.6,  3.7,  3.8,  3.9,  4. ,  4.1,  4.2,  4.3,
+            4.4,  4.5,  4.6,  4.7,  4.8,  4.9,  5. ,  5.1,  5.2,  5.3,  5.4,
+            5.5,  5.6,  5.7,  5.8,  5.9,  6. ,  6.1,  6.2,  6.3,  6.4,  6.5,
+            6.6,  6.7,  6.8,  6.9,  7. ,  7.1,  7.2,  7.3,  7.4,  7.5,  7.6,
+            7.7,  7.8,  7.9,  8. ,  8.1,  8.2,  8.3,  8.4,  8.5,  8.6,  8.7,
+            8.8,  8.9,  9. ,  9.1,  9.2,  9.3,  9.4,  9.5,  9.6,  9.7,  9.8,
             9.9, 10. ])
     >>> rdfs
     array([0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.00458757,
+           0.00495436, 0.00307412, 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
            0.        , 0.        , 0.        , 0.        , 0.        ,
-           ...,
-           0.97097276])]
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        , 0.        , 0.        , 0.        , 0.        ,
+           0.        ])
     """
     strs = build_Structures_from_datafile(datafile)
     # print(strs[0]) # check pbc
     # raise ValueError
 
     # 计算rdf并绘制主要曲线
     obj = RDF(structures=strs, rmin=rmin, rmax=rmax, ngrid=ngrid, sigma=sigma)
@@ -453,15 +474,15 @@
     xlim: List[float] = None,
     ylim: List[float] = None,
     figname: str = None,
     show: bool = True,
     ax=None,
     **kwargs,
 ):
-    """AIMD任务完成后，计算均方差（MSD）
+    r"""AIMD任务完成后，计算均方差（MSD）
 
     Parameters
     ----------
     lagtime : np.ndarray
         时间序列
     result : np.ndarray
         均方差序列
@@ -481,18 +502,26 @@
     Returns
     -------
     MSD分析后的图片
 
     Examples
     --------
     >>> from dspawpy.analysis.aimdtools import get_lagtime_msd, plot_msd
-    # 指定h5文件位置，用 get_lagtime_msd 函数获取数据，select 参数选择第n个原子（不是元素）
-    >>> lagtime, msd = get_lagtime_msd('H2O-aimd1.h5', select=[0])
-    # 用获取的数据画图并保存
-    >>> plot_msd(lagtime, msd, figname='MSD.png')
+
+    指定h5文件位置，用 get_lagtime_msd 函数获取数据，select 参数选择第n个原子（不是元素）
+
+    >>> lagtime, msd = get_lagtime_msd('test/aimd.h5', select=[0])
+    Reading E:\Dev\dspawpy\test\aimd.h5 ...
+    Calculating MSD...
+
+    用获取的数据画图并保存
+
+    >>> plot_msd(lagtime, msd, figname='test/MSD.png', show=False)
+    MSD图片保存在 E:\Dev\dspawpy\test\MSD.png
+    <Axes: xlabel='Time (fs)', ylabel='MSD (Å)'>
     """
     if ax:
         ishow = False
         ax.plot(lagtime, result, c="black", ls="-", **kwargs)
     else:
         ishow = True
         fig, ax = plt.subplots()
@@ -522,15 +551,15 @@
     xlim: list = None,
     ylim: list = None,
     figname: str = None,
     show: bool = True,
     ax: plt.Axes = None,
     **kwargs,
 ):
-    """AIMD计算后分析rdf并画图
+    r"""AIMD计算后分析rdf并画图
 
     Parameters
     ----------
     rs : numpy.ndarray
         径向分布网格点
     rdfs : numpy.ndarray
         径向分布函数
@@ -554,18 +583,25 @@
     Returns
     -------
     rdf分析后的图片
 
     Examples
     --------
     >>> from dspawpy.analysis.aimdtools import get_rs_rdfs, plot_rdf
-    # 先获取rs和rdfs数据作为xy轴数据
-    >>> rs, rdfs = get_rs_rdfs(['LiO-aimd1.h5','LiO-aimd2.h5','LiO-aimd3.h5'], 'Li', 'O', rmax=6)
-    # 将xy轴数据传入plot_rdf函数绘图
-    >>> plot_rdf(rs, rdfs, 'Li','O', xlim=[0,6], ylim=[0,35], color='red')
+
+    先获取rs和rdfs数据作为xy轴数据
+
+    >>> rs, rdfs = get_rs_rdfs('test/aimd.h5', 'H', 'O', rmax=6)
+    Reading E:\Dev\dspawpy\test\aimd.h5 ...
+    Calculating RDF...
+
+    将xy轴数据传入plot_rdf函数绘图
+
+    >>> plot_rdf(rs, rdfs, 'H','O', figname='test/RDF.png', show=False)
+    图片已保存到 E:\Dev\dspawpy\test\RDF.png
     """
     if ax:
         ax.plot(
             rs,
             rdfs,
             label=r"$g_{\alpha\beta}(r)$" + f"[{ele1},{ele2}]",
             **kwargs,
@@ -604,15 +640,15 @@
     xlim: list = None,
     ylim: list = None,
     figname: str = None,
     show: bool = True,
     ax=None,
     **kwargs,
 ):
-    """AIMD计算后分析rmsd并画图
+    r"""AIMD计算后分析rmsd并画图
 
     Parameters
     ----------
     lagtime:
         时间序列
     result:
         均方根序列
@@ -632,18 +668,26 @@
     Returns
     -------
     rmsd分析结构的图片
 
     Examples
     --------
     >>> from dspawpy.analysis.aimdtools import get_lagtime_rmsd, plot_rmsd
-    # timestep 表示时间步长
-    >>> lagtime, rmsd = get_lagtime_rmsd(datafile='H2O-aimd1.h5', timestep=0.1)
-    # 直接保存为RMSD.png图片
-    >>> plot_rmsd(lagtime, rmsd, figname='RMSD.png', show=True)
+
+    timestep 表示时间步长
+
+    >>> lagtime, rmsd = get_lagtime_rmsd(datafile='test/aimd.h5', timestep=0.1)
+    Reading E:\Dev\dspawpy\test\aimd.h5 ...
+    Calculating RMSD...
+
+    直接保存为RMSD.png图片
+
+    >>> plot_rmsd(lagtime, rmsd, figname='test/RMSD.png', show=False)
+    图片已保存到 E:\Dev\dspawpy\test\RMSD.png
+    <Axes: xlabel='Time (fs)', ylabel='RMSD (Å)'>
     """
     # 参数初始化
     if not ax:
         ishow = True
     else:
         ishow = False
 
@@ -658,11 +702,12 @@
     if xlim:
         ax.set_xlim(xlim)
     if ylim:
         ax.set_ylim(ylim)
 
     if figname:
         plt.savefig(figname)
+        print(f"图片已保存到 {os.path.abspath(figname)}")
     if show and ishow:  # 画子图的话，不应每个子图都show
         plt.show()  # show会自动清空图片
 
     return ax
```

## dspawpy/diffusion/neb.py

```diff
@@ -11,24 +11,14 @@
     ----------
     initial_structure: Structure
         初态
     final_structure: Structure
         终态
     nimages: int
         中间构型数
-
-    Examples
-    --------
-    >>> from pymatgen.core import Structure
-    # 先调用pymatgen写好的from_file方法读取cif构型文件，生成structure对象
-    >>> initial_structure = Structure.from_file("initial.cif")
-    >>> final_structure = Structure.from_file("final.cif")
-    # 初始化对象，后续可以调用两个插值算法，详见下方write_neb_structures
-    >>> from dspawpy.diffusion.neb import NEB
-    >>> neb = NEB(initial_structure,final_structure,10)
     """
 
     def __init__(self, initial_structure, final_structure, nimages):
         """
 
         Args:
             initial_structure:
@@ -61,15 +51,15 @@
 def write_neb_structures(
     structures,
     coords_are_cartesian=True,
     fmt: str = "json",
     path: str = ".",
     prefix="structure",
 ):
-    """插值并生成中间构型文件
+    r"""插值并生成中间构型文件
 
     Parameters
     ----------
     structures: list
         构型列表
     coords_are_cartesian: bool
         坐标是否为笛卡尔坐标
@@ -85,27 +75,29 @@
 
     Examples
     --------
 
     先读取as文件创建structure对象
 
     >>> from dspawpy.io.structure import build_Structures_from_datafile
-    >>> initial_structure = build_Structures_from_datafile("structure00.as")[0]
-    >>> final_structure = build_Structures_from_datafile("structure06.as")[0]
+    >>> initial_structure = build_Structures_from_datafile("test/initial.as")[0]
+    >>> final_structure = build_Structures_from_datafile("test/final.as")[0]
 
     然后，插值并生成中间构型文件
 
     >>> from dspawpy.diffusion.neb import NEB,write_neb_structures
-    >>> neb = NEB(initial_structure,final_structure,10)
-    >>> neb = NEB(init_struct,final_struct,5) # 设置插点个数
+    >>> neb = NEB(initial_structure,final_structure,3) # 计划获取3个构型
     >>> structures = neb.idpp_interpolate() # idpp插值，生成中间构型
 
     插值完成的构型可指定保存到neb文件夹下
 
-    >>> write_neb_structures(structures,coords_are_cartesian=True,fmt="as",path="neb")
+    >>> write_neb_structures(structures,coords_are_cartesian=True,fmt="as",path="test/neb")
+    --> 成功写入文件 E:\Dev\dspawpy\test\neb\00\structure00.as
+    --> 成功写入文件 E:\Dev\dspawpy\test\neb\01\structure01.as
+    --> 成功写入文件 E:\Dev\dspawpy\test\neb\02\structure02.as
     """
     N = len(str(len(structures)))
     if N <= 2:
         N = 2
     for i, structure in enumerate(structures):
         path_name = str(i).zfill(N)
         os.makedirs(os.path.join(path, path_name), exist_ok=True)
```

## dspawpy/diffusion/nebtools.py

```diff
@@ -35,27 +35,27 @@
 
     Examples
     --------
 
     先读取两个构型的分数坐标、元素列表和晶胞信息
 
     >>> from dspawpy.io.read import pel_from_as
-    >>> spo1, ele1, lat1 = pel_from_as('structure01.as', sacled=True)
+    >>> spo1, ele1, lat1 = pel_from_as('structure01.as', scaled=True)
     >>> spo1
     array([[0.25      , 0.25      , 0.11784996],
            [0.75      , 0.25      , 0.11784996],
            ...，
            [0.04062186, 0.45937779, 0.43038044]])
     >>> ele1
     ['Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt']
     >>> lat1
     array([[ 5.6058,  0.    ,  0.    ],
            [ 0.    ,  5.6058,  0.    ],
            [ 0.    ,  0.    , 16.8174]])
-    >>> spo2, ele2, lat2 = pel_from_as('structure02.as', sacled=True)
+    >>> spo2, ele2, lat2 = pel_from_as('structure02.as', scaled=True)
     >>> spo2
     array([[0.25      , 0.25      , 0.11784996],
            ...，
            [0.08124389, 0.41875557, 0.41408303]])
     >>> ele2
     ['Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt']
     >>> lat2
@@ -71,14 +71,15 @@
     0.5987379724194888
     """
     diff_spo = spo1 - spo2  # 分数坐标差
     avglatv = 0.5 * (lat1 + lat2)  # 平均晶格矢量
     pbc_diff_spo = set_pbc(diff_spo)  # 笛卡尔坐标差
     # 分数坐标点乘平均晶胞，转回笛卡尔坐标
     pbc_diff_pos = np.dot(pbc_diff_spo, avglatv)  # 笛卡尔坐标差
+    print(f"{pbc_diff_pos=}")
     distance = np.sqrt(np.sum(pbc_diff_pos**2))
 
     return distance
 
 
 def get_neb_subfolders(directory: str = "."):
     """将directory路径下的子文件夹名称列表按照数字大小排序
```

## dspawpy/io/write.py

```diff
@@ -2,14 +2,15 @@
 Functions to write files
 """
 
 import json
 import os
 
 import numpy as np
+from pymatgen.core.structure import Structure
 
 from dspawpy.io.read import _get_lammps_non_orthogonal_box, load_h5
 
 
 def _write_xyz_traj(
     structures,
     xyzfile="aimdTraj.xyz",
@@ -316,15 +317,15 @@
                     ind = ind + 1
                     if ind % 5 == 0:
                         out.write("\n")
 
     print(f"成功写入 {output}")
 
 
-def to_file(structure, filename: str, fmt=None, coords_are_cartesian=True):
+def to_file(structure, filename: str, fmt=None, coords_are_cartesian=True, si=None):
     r"""往结构文件中写入信息
 
     Parameters
     ----------
     structure : Structure
         pymatgen的Structure对象
     filename : str
@@ -332,14 +333,16 @@
     fmt : str
         - 结构文件类型，目前支持 'json', 'as', 'hzw', 'pdb', 'xyz', 'dump', 'cif', 'poscar', 'cssr', 'xsf', 'mcsqs', 'prismatic', 'yaml', 'fleur-inpgen'
         - 若不指定，则根据文件名后缀判断
         - 'pdb', 'xyz' 和 'dump' 支持传入多个结构，structure参数可以是一个Structure对象列表；其他类型的文件只支持传入单个结构
     coords_are_cartesian : bool
         - 是否写作笛卡尔坐标，默认为True；否则写成分数坐标形式
         - 此选项暂时仅对 as 和 json 格式有效
+    si : int
+        结构编号索引
 
     Examples
     --------
 
     如果不指定 fmt 参数，将尝试根据文件名后缀判断。
 
     如果要生成 as 结构文件（可用于开始新任务），可参考如下命令:
@@ -378,47 +381,72 @@
     --> 成功写入文件 E:\Dev\dspawpy\test\new\PtH.hzw
 
     写成 pdb 文件，也将忽略磁矩和自由度信息
 
     >>> to_file(s, filename='PtH.pdb')
     --> 成功写入文件 E:\Dev\dspawpy\test\new\PtH.pdb
     """
+    if si is not None:
+        assert isinstance(si, int), "si 应当是用于索引列表的整数"
+    if isinstance(structure, Structure):
+        structure = [structure]
 
     if fmt is None:
         fmt = filename.split(".")[-1]
 
-    if fmt == "json":  # 单个构型
-        assert not isinstance(structure, list), "只接受单个构型"
-        _to_dspaw_json(structure, filename, coords_are_cartesian)
-    elif fmt == "as":
-        assert not isinstance(structure, list), "只接受单个构型"
-        _to_dspaw_as(structure, filename, coords_are_cartesian)
-    elif fmt == "hzw":
-        assert not isinstance(structure, list), "只接受单个构型"
-        _to_hzw(structure, filename)
-    elif fmt == "pdb":  # 可以是多个构型
-        _to_pdb(structure, filename)
+    if fmt == "pdb":  # 可以是多个构型
+        if si:
+            _to_pdb(structure[si], filename)
+        else:
+            _to_pdb(structure, filename)
     elif fmt == "xyz":  # 可以是多个构型
-        _write_xyz_traj(structure, filename)
+        if si:
+            _write_xyz_traj(structure[si], filename)
+        else:
+            _write_xyz_traj(structure, filename)
     elif fmt == "dump":  # 可以是多个构型
-        _write_dump_traj(structure, filename)
+        if si:
+            _write_dump_traj(structure[si], filename)
+        else:
+            _write_dump_traj(structure, filename)
+
+    elif fmt == "json":  # 单个构型
+        if si:
+            _to_dspaw_json(structure[si], filename, coords_are_cartesian)
+        else:
+            _to_dspaw_json(structure[-1], filename, coords_are_cartesian)
+    elif fmt == "as":
+        if si:
+            _to_dspaw_as(structure[si], filename, coords_are_cartesian)
+        else:
+            _to_dspaw_as(structure[-1], filename, coords_are_cartesian)
+    elif fmt == "hzw":
+        if si:
+            _to_hzw(structure[si], filename)
+        else:
+            _to_hzw(structure[-1], filename)
+
     elif fmt in [
         "cif",
         "poscar",
         "cssr",
         "xsf",
         "mcsqs",
         "prismatic",
         "yaml",
         "fleur-inpgen",
     ]:
-        assert not isinstance(structure, list), "只接受单个构型"
-        structure.to(filename, fmt=fmt)
+        if si:
+            structure[si].to(filename, fmt=fmt)
+        else:
+            structure[-1].to(filename, fmt=fmt)
     else:
-        raise NotImplementedError(f"暂不支持写成 {fmt} 格式")
+        raise NotImplementedError(
+            f"暂不支持写成 {fmt} 格式，支持的格式包括：pdb, xyz, dump, json, as, hzw, cif, poscar, cssr, xsf, mcsqs, prismatic, yaml, fleur-inpgen"
+        )
 
     print(f"--> 成功写入文件 {os.path.abspath(filename)} ")
 
 
 def _write_atoms(fileobj, hdf5):
     fileobj.write("DS-PAW Structure\n")
     fileobj.write("  1.00\n")
```

## Comparing `dspawpy-0.9.6.dist-info/METADATA` & `dspawpy-0.9.7.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 0.9.6
+Version: 0.9.7
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: pymatgen (>=2021.2.8.1)
@@ -28,17 +28,22 @@
 
 再重新用pip安装。
 
 详见 https://stackoverflow.com/questions/75542688/conda-installed-pip-failed-to-find-packages/75542962#75542962
 
 ## 版本更新简述
 
+### 0.9.7
+
+- BUG修复： get_rdf 元素对自己计算RDF时的索引
+- 新增功能：to_file 增加 si 参数，支持读入单个structure以及Structure列表
+
 ### 0.9.6
 
-- BUG修复：pymatgen支持的几类结构文件的读取接口
+- BUG修复： pymatgen支持的几类结构文件的读取接口
 
 ### 0.9.5
 
 - 重要变更： get_band_data 的 shift_efermi 参数改名为 zero_to_fermi
 
 ### 0.9.4
```

## Comparing `dspawpy-0.9.6.dist-info/RECORD` & `dspawpy-0.9.7.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-dspawpy/__init__.py,sha256=DUP796j17_h9tFqkdOpSu_66sw_6eSK4S2hN7yd9i9o,23
+dspawpy/__init__.py,sha256=83qFJMFAgvdHV5e8Nh9ByUaQinNxBUPlTKjxfpge3xM,23
 dspawpy/plot.py,sha256=ocLkU08WfMb2fyETrBSSZvxZFSg2sPX8rLusXZLT5BM,29208
 dspawpy/analysis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dspawpy/analysis/aimdtools.py,sha256=72N58P2EBA5z8EZwaY1W6ab8ZGZVwefQCjME8490HqU,21567
+dspawpy/analysis/aimdtools.py,sha256=iAUHcBECcmpG8gmBELoaiwfDT1KxTjrehzcotOufnEg,23645
 dspawpy/analysis/vacf.py,sha256=g5IS6Q7QGYa17XBVnYEH-MubGSpkUsDPpMaI_ELacw4,20152
 dspawpy/diffusion/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dspawpy/diffusion/neb.py,sha256=U6J7lSlE_xp1rCON5mgfWWi5DFHVZYVb5xjqLlGxXXI,3592
-dspawpy/diffusion/nebtools.py,sha256=tfQCQPUmZKELz7ImwyiJiiFfXahC9U3doarExspL-DU,53467
+dspawpy/diffusion/neb.py,sha256=h2n3wYmEEpVhF5EeiDnColcotw3CyEHaiAfSHyb0BMU,3270
+dspawpy/diffusion/nebtools.py,sha256=wK-W9_8AQZHaZ_Q9Kvh95Olgduz2s9u0zQFZRemJrbw,53498
 dspawpy/diffusion/pathfinder.py,sha256=HhCVoh42Q2qIksBAruZ1atULfR5D55uzZvbaCtUxSig,11045
 dspawpy/io/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dspawpy/io/read.py,sha256=ZDcow03EV2TGBnQ8cO68r3a0l4P1wqh99W1xWFofZLc,53355
 dspawpy/io/read_json.py,sha256=2bcNQP51SR2yMyFE7c2TIutYp93K8IH-dpLmH5yy4bo,7721
 dspawpy/io/structure.py,sha256=HenUYKsB4YRa8I5F_WtlZ5Mq226cOGQXmHx2BpXi2qI,9880
 dspawpy/io/utils.py,sha256=ff2182s8KQWQ53bHYdlWuXuN3lkDLAH6zrNub1t_9wA,25239
-dspawpy/io/write.py,sha256=8oQikD6Iyo7Bxy5_1Fl7SaSyZK3o6oBCwC82Raqa9cY,25391
+dspawpy/io/write.py,sha256=jimEccJMmL2ybY1gjSaf0A5JNJ783XOZ6YJRLksEaG0,26180
 dspawpy/io/write_json.py,sha256=n3GhdDnFFtW7eY4U5u7czdlpbSWnsGP7WUD5eS1ZmqI,1761
-dspawpy-0.9.6.dist-info/METADATA,sha256=7OP0zcmKL90pnCExlyd-1PC08z9Xd-2c4c-qSZoo9nQ,2904
-dspawpy-0.9.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dspawpy-0.9.6.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
-dspawpy-0.9.6.dist-info/RECORD,,
+dspawpy-0.9.7.dist-info/METADATA,sha256=Pzg-TDwjVSz1dmQa4PmYFwVMgJtTheh-f-sPH09t1Go,3075
+dspawpy-0.9.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+dspawpy-0.9.7.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
+dspawpy-0.9.7.dist-info/RECORD,,
```

