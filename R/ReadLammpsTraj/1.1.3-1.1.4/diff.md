# Comparing `tmp/ReadLammpsTraj-1.1.3.tar.gz` & `tmp/ReadLammpsTraj-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReadLammpsTraj-1.1.3.tar", last modified: Wed May 31 14:30:21 2023, max compression
+gzip compressed data, was "ReadLammpsTraj-1.1.4.tar", last modified: Wed May 31 14:35:19 2023, max compression
```

## Comparing `ReadLammpsTraj-1.1.3.tar` & `ReadLammpsTraj-1.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.834541 ReadLammpsTraj-1.1.3/
--rw-rw-rw-   0        0        0     1087 2023-05-31 03:57:12.000000 ReadLammpsTraj-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      132 2023-05-31 14:29:01.000000 ReadLammpsTraj-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2225 2023-05-31 14:30:21.834541 ReadLammpsTraj-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1936 2023-05-31 05:31:22.000000 ReadLammpsTraj-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.817011 ReadLammpsTraj-1.1.3/demo/
--rw-rw-rw-   0        0        0  2026571 2022-07-19 02:19:38.000000 ReadLammpsTraj-1.1.3/demo/1000.lammpstrj
-drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.820012 ReadLammpsTraj-1.1.3/demo/__pycache__/
--rw-rw-rw-   0        0        0    15185 2023-05-31 05:24:15.000000 ReadLammpsTraj-1.1.3/demo/__pycache__/ReadLammpsTraj.cpython-311.pyc
--rw-rw-rw-   0        0        0     1966 2023-05-31 14:26:43.000000 ReadLammpsTraj-1.1.3/demo/cal_density.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.822010 ReadLammpsTraj-1.1.3/demo/imgs/
--rw-rw-rw-   0        0        0   307101 2023-05-31 14:26:47.000000 ReadLammpsTraj-1.1.3/demo/imgs/density.png
--rw-rw-rw-   0        0        0       30 2023-05-31 05:32:22.000000 ReadLammpsTraj-1.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 14:30:21.835538 ReadLammpsTraj-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      720 2023-05-31 14:30:12.000000 ReadLammpsTraj-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.824011 ReadLammpsTraj-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.832538 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/
--rw-rw-rw-   0        0        0     2225 2023-05-31 14:30:21.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-05-31 14:30:21.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:30:21.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-31 14:30:21.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 14:30:21.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10480 2023-05-31 14:19:00.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.161053 ReadLammpsTraj-1.1.4/
+-rw-rw-rw-   0        0        0     1087 2023-05-31 03:57:12.000000 ReadLammpsTraj-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      132 2023-05-31 14:29:01.000000 ReadLammpsTraj-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2684 2023-05-31 14:35:19.160053 ReadLammpsTraj-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2401 2023-05-31 14:34:42.000000 ReadLammpsTraj-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.143533 ReadLammpsTraj-1.1.4/demo/
+-rw-rw-rw-   0        0        0  2026571 2022-07-19 02:19:38.000000 ReadLammpsTraj-1.1.4/demo/1000.lammpstrj
+drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.146056 ReadLammpsTraj-1.1.4/demo/__pycache__/
+-rw-rw-rw-   0        0        0    15185 2023-05-31 05:24:15.000000 ReadLammpsTraj-1.1.4/demo/__pycache__/ReadLammpsTraj.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1966 2023-05-31 14:26:43.000000 ReadLammpsTraj-1.1.4/demo/cal_density.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.147055 ReadLammpsTraj-1.1.4/demo/imgs/
+-rw-rw-rw-   0        0        0   307101 2023-05-31 14:26:47.000000 ReadLammpsTraj-1.1.4/demo/imgs/density.png
+-rw-rw-rw-   0        0        0       30 2023-05-31 05:32:22.000000 ReadLammpsTraj-1.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 14:35:19.161053 ReadLammpsTraj-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      720 2023-05-31 14:35:10.000000 ReadLammpsTraj-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.149054 ReadLammpsTraj-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 14:35:19.158054 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/
+-rw-rw-rw-   0        0        0     2684 2023-05-31 14:35:18.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-31 14:35:19.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 14:35:18.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-31 14:35:18.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 14:35:18.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10480 2023-05-31 14:19:00.000000 ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.py
```

### Comparing `ReadLammpsTraj-1.1.3/LICENSE` & `ReadLammpsTraj-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.3/PKG-INFO` & `ReadLammpsTraj-1.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,81 @@
 Metadata-Version: 2.1
 Name: ReadLammpsTraj
-Version: 1.1.3
+Version: 1.1.4
 Summary: Read lammps dump trajectory.
 Home-page: https://github.com/eastsheng/ReadLammpsTraj
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## ReadLammpsTraj
 - Read lammps dump trajectory
 
 ### Installation
 
-```bash
-git clone https://github.com/eastsheng/ReadLammpsTraj
-cd ReadLammpsTraj
-pip install .
-```
+- github:
+
+  ```bash
+  git clone https://github.com/eastsheng/ReadLammpsTraj
+  cd ReadLammpsTraj
+  pip install .
+  ```
+
+- pip
+
+  ```
+  pip install ReadLammpsTraj
+  ```
+
+  
 
 ### Usage
 
 - A example to calculate density in demo folder:
 
   ```python
   # calculating the density from lammps traj
-  # id mol type mass x y z vx vy vz fx fy fz q
   import numpy as np
   import matplotlib.pyplot as plt
   import ReadLammpsTraj as RLT
   from pathlib import Path
+  import periodictable as pt
   
   def cal_density():
   	path = "./"
   	f = "1000.lammpstrj"
-  
-  	Path(path+"density/").mkdir(parents=True,exist_ok=True)
+  	# lammpsdata = "1_npt_dissociation.data"
+  	Path(path+"imgs/").mkdir(parents=True,exist_ok=True)
   
   	md = RLT.ReadLammpsTraj(path+f)
   	md.read_info()
   	# # number of frames
   	mframe,nframe = 1, 1
   	# # chunk number in z
   	Nz = 100
-  	mol_n = [1,1000]
-  	# 鍒嗗瓙搴忓彿
+  	id_range = [1,10000]
+  	# # element mass
+  	# O_mass = pt.elements.symbol('O').mass
+  	# H_mass = pt.elements.symbol('H').mass
+  	# C_mass = pt.elements.symbol('C').mass
+  	# mass_dict = {1:O_mass,2:H_mass,3:C_mass+4*H_mass,4:C_mass+4*H_mass}
+  	mass_dict = {}
+  	# mass_dict = RLT.read_mass(path+lammpsdata)
+  
+  	direction = "z"
   
   	Calculate = True #True#False
   
   	if Calculate==True:
   		rho_nframe = np.zeros(Nz).reshape(Nz,1)
   		for i in range(mframe,nframe+1):
   			position = md.read_mxyz(i)
-  			z, rho = md.oneframe_alldensity(position,Nz,density_type="mass")
-  			# z, rho = md.oneframe_moldensity(position,Nz,mol_n=mol_n,id_type="mol",density_type="mass")
+  			# z, rho = md.oneframe_alldensity(position,Nz,mass_dict,density_type="mass",direction=direction)
+  			z, rho = md.oneframe_moldensity(position,Nz,id_range,mass_dict,id_type="atom",density_type="mass",direction=direction)
   
   			rho_nframe = rho_nframe+rho
   
   			print(i,"---",nframe)
   		nf = (nframe-mframe+1)
   		rho=rho_nframe/nf #all
   		print("Average density =",rho.mean(),"g/mL")
@@ -71,17 +89,17 @@
   	# ax.legend(loc="center")
   	ax.legend(loc="best")
   
   	ax.set_ylabel('Density(g/mL)',fontweight='bold',size=32)
   	ax.set_xlabel('z(脜)',fontweight='bold',size=32)	
   	# ax.set_ylim(-0.05,1.5)
   
-  	plt.savefig(path+"density/density.png",dpi=300)
+  	plt.savefig(path+"imgs/density.png",dpi=300)
   	plt.show()
   
   
   if __name__ == '__main__':
   	cal_density()
   ```
-
+
```

### Comparing `ReadLammpsTraj-1.1.3/README.md` & `ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,81 @@
+Metadata-Version: 2.1
+Name: ReadLammpsTraj
+Version: 1.1.4
+Summary: Read lammps dump trajectory.
+Home-page: https://github.com/eastsheng/ReadLammpsTraj
+Author: CHENDONGSHENG
+Author-email: eastsheng@hotmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## ReadLammpsTraj
 - Read lammps dump trajectory
 
 ### Installation
 
-```bash
-git clone https://github.com/eastsheng/ReadLammpsTraj
-cd ReadLammpsTraj
-pip install .
-```
+- github:
+
+  ```bash
+  git clone https://github.com/eastsheng/ReadLammpsTraj
+  cd ReadLammpsTraj
+  pip install .
+  ```
+
+- pip
+
+  ```
+  pip install ReadLammpsTraj
+  ```
+
+  
 
 ### Usage
 
 - A example to calculate density in demo folder:
 
   ```python
   # calculating the density from lammps traj
-  # id mol type mass x y z vx vy vz fx fy fz q
   import numpy as np
   import matplotlib.pyplot as plt
   import ReadLammpsTraj as RLT
   from pathlib import Path
+  import periodictable as pt
   
   def cal_density():
   	path = "./"
   	f = "1000.lammpstrj"
-  
-  	Path(path+"density/").mkdir(parents=True,exist_ok=True)
+  	# lammpsdata = "1_npt_dissociation.data"
+  	Path(path+"imgs/").mkdir(parents=True,exist_ok=True)
   
   	md = RLT.ReadLammpsTraj(path+f)
   	md.read_info()
   	# # number of frames
   	mframe,nframe = 1, 1
   	# # chunk number in z
   	Nz = 100
-  	mol_n = [1,1000]
-  	# 分子序号
+  	id_range = [1,10000]
+  	# # element mass
+  	# O_mass = pt.elements.symbol('O').mass
+  	# H_mass = pt.elements.symbol('H').mass
+  	# C_mass = pt.elements.symbol('C').mass
+  	# mass_dict = {1:O_mass,2:H_mass,3:C_mass+4*H_mass,4:C_mass+4*H_mass}
+  	mass_dict = {}
+  	# mass_dict = RLT.read_mass(path+lammpsdata)
+  
+  	direction = "z"
   
   	Calculate = True #True#False
   
   	if Calculate==True:
   		rho_nframe = np.zeros(Nz).reshape(Nz,1)
   		for i in range(mframe,nframe+1):
   			position = md.read_mxyz(i)
-  			z, rho = md.oneframe_alldensity(position,Nz,density_type="mass")
-  			# z, rho = md.oneframe_moldensity(position,Nz,mol_n=mol_n,id_type="mol",density_type="mass")
+  			# z, rho = md.oneframe_alldensity(position,Nz,mass_dict,density_type="mass",direction=direction)
+  			z, rho = md.oneframe_moldensity(position,Nz,id_range,mass_dict,id_type="atom",density_type="mass",direction=direction)
   
   			rho_nframe = rho_nframe+rho
   
   			print(i,"---",nframe)
   		nf = (nframe-mframe+1)
   		rho=rho_nframe/nf #all
   		print("Average density =",rho.mean(),"g/mL")
@@ -58,20 +86,20 @@
   	ax=fig.add_subplot(111)
   	ax.plot(z,rho,'r--',label='All',linewidth=2)
   
   	# ax.legend(loc="center")
   	ax.legend(loc="best")
   
   	ax.set_ylabel('Density(g/mL)',fontweight='bold',size=32)
-  	ax.set_xlabel('z(Å)',fontweight='bold',size=32)	
+  	ax.set_xlabel('z(脜)',fontweight='bold',size=32)	
   	# ax.set_ylim(-0.05,1.5)
   
-  	plt.savefig(path+"density/density.png",dpi=300)
+  	plt.savefig(path+"imgs/density.png",dpi=300)
   	plt.show()
   
   
   if __name__ == '__main__':
   	cal_density()
   ```
-
+
```

### Comparing `ReadLammpsTraj-1.1.3/demo/1000.lammpstrj` & `ReadLammpsTraj-1.1.4/demo/1000.lammpstrj`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.3/demo/__pycache__/ReadLammpsTraj.cpython-311.pyc` & `ReadLammpsTraj-1.1.4/demo/__pycache__/ReadLammpsTraj.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.3/demo/cal_density.py` & `ReadLammpsTraj-1.1.4/demo/cal_density.py`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.3/demo/imgs/density.png` & `ReadLammpsTraj-1.1.4/demo/imgs/density.png`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.3/setup.py` & `ReadLammpsTraj-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'ReadLammpsTraj',
-version      = '1.1.3',
+version      = '1.1.4',
 py_modules   = ['ReadLammpsTraj'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/ReadLammpsTraj',
```

### Comparing `ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/PKG-INFO` & `ReadLammpsTraj-1.1.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,71 @@
-Metadata-Version: 2.1
-Name: ReadLammpsTraj
-Version: 1.1.3
-Summary: Read lammps dump trajectory.
-Home-page: https://github.com/eastsheng/ReadLammpsTraj
-Author: CHENDONGSHENG
-Author-email: eastsheng@hotmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## ReadLammpsTraj
 - Read lammps dump trajectory
 
 ### Installation
 
-```bash
-git clone https://github.com/eastsheng/ReadLammpsTraj
-cd ReadLammpsTraj
-pip install .
-```
+- github:
+
+  ```bash
+  git clone https://github.com/eastsheng/ReadLammpsTraj
+  cd ReadLammpsTraj
+  pip install .
+  ```
+
+- pip
+
+  ```
+  pip install ReadLammpsTraj
+  ```
+
+  
 
 ### Usage
 
 - A example to calculate density in demo folder:
 
   ```python
   # calculating the density from lammps traj
-  # id mol type mass x y z vx vy vz fx fy fz q
   import numpy as np
   import matplotlib.pyplot as plt
   import ReadLammpsTraj as RLT
   from pathlib import Path
+  import periodictable as pt
   
   def cal_density():
   	path = "./"
   	f = "1000.lammpstrj"
-  
-  	Path(path+"density/").mkdir(parents=True,exist_ok=True)
+  	# lammpsdata = "1_npt_dissociation.data"
+  	Path(path+"imgs/").mkdir(parents=True,exist_ok=True)
   
   	md = RLT.ReadLammpsTraj(path+f)
   	md.read_info()
   	# # number of frames
   	mframe,nframe = 1, 1
   	# # chunk number in z
   	Nz = 100
-  	mol_n = [1,1000]
-  	# 鍒嗗瓙搴忓彿
+  	id_range = [1,10000]
+  	# # element mass
+  	# O_mass = pt.elements.symbol('O').mass
+  	# H_mass = pt.elements.symbol('H').mass
+  	# C_mass = pt.elements.symbol('C').mass
+  	# mass_dict = {1:O_mass,2:H_mass,3:C_mass+4*H_mass,4:C_mass+4*H_mass}
+  	mass_dict = {}
+  	# mass_dict = RLT.read_mass(path+lammpsdata)
+  
+  	direction = "z"
   
   	Calculate = True #True#False
   
   	if Calculate==True:
   		rho_nframe = np.zeros(Nz).reshape(Nz,1)
   		for i in range(mframe,nframe+1):
   			position = md.read_mxyz(i)
-  			z, rho = md.oneframe_alldensity(position,Nz,density_type="mass")
-  			# z, rho = md.oneframe_moldensity(position,Nz,mol_n=mol_n,id_type="mol",density_type="mass")
+  			# z, rho = md.oneframe_alldensity(position,Nz,mass_dict,density_type="mass",direction=direction)
+  			z, rho = md.oneframe_moldensity(position,Nz,id_range,mass_dict,id_type="atom",density_type="mass",direction=direction)
   
   			rho_nframe = rho_nframe+rho
   
   			print(i,"---",nframe)
   		nf = (nframe-mframe+1)
   		rho=rho_nframe/nf #all
   		print("Average density =",rho.mean(),"g/mL")
@@ -68,20 +76,20 @@
   	ax=fig.add_subplot(111)
   	ax.plot(z,rho,'r--',label='All',linewidth=2)
   
   	# ax.legend(loc="center")
   	ax.legend(loc="best")
   
   	ax.set_ylabel('Density(g/mL)',fontweight='bold',size=32)
-  	ax.set_xlabel('z(脜)',fontweight='bold',size=32)	
+  	ax.set_xlabel('z(Å)',fontweight='bold',size=32)	
   	# ax.set_ylim(-0.05,1.5)
   
-  	plt.savefig(path+"density/density.png",dpi=300)
+  	plt.savefig(path+"imgs/density.png",dpi=300)
   	plt.show()
   
   
   if __name__ == '__main__':
   	cal_density()
   ```
-
+
```

### Comparing `ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.py` & `ReadLammpsTraj-1.1.4/src/ReadLammpsTraj.py`

 * *Files identical despite different names*

