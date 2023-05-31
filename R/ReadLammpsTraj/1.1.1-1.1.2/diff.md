# Comparing `tmp/ReadLammpsTraj-1.1.1.tar.gz` & `tmp/ReadLammpsTraj-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReadLammpsTraj-1.1.1.tar", last modified: Wed May 31 05:46:12 2023, max compression
+gzip compressed data, was "ReadLammpsTraj-1.1.2.tar", last modified: Wed May 31 14:20:58 2023, max compression
```

## Comparing `ReadLammpsTraj-1.1.1.tar` & `ReadLammpsTraj-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 05:46:12.892638 ReadLammpsTraj-1.1.1/
--rw-rw-rw-   0        0        0     1087 2023-05-31 03:57:12.000000 ReadLammpsTraj-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       90 2023-05-31 05:35:57.000000 ReadLammpsTraj-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2225 2023-05-31 05:46:12.887637 ReadLammpsTraj-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1936 2023-05-31 05:31:22.000000 ReadLammpsTraj-1.1.1/README.md
--rw-rw-rw-   0        0        0       30 2023-05-31 05:32:22.000000 ReadLammpsTraj-1.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 05:46:12.892638 ReadLammpsTraj-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      720 2023-05-31 05:46:05.000000 ReadLammpsTraj-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:46:12.874637 ReadLammpsTraj-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 05:46:12.884637 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/
--rw-rw-rw-   0        0        0     2225 2023-05-31 05:46:12.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-05-31 05:46:12.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 05:46:12.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-31 05:46:12.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 05:46:12.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8088 2023-05-31 05:24:13.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:20:58.891399 ReadLammpsTraj-1.1.2/
+-rw-rw-rw-   0        0        0     1087 2023-05-31 03:57:12.000000 ReadLammpsTraj-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      106 2023-05-31 14:20:55.000000 ReadLammpsTraj-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2225 2023-05-31 14:20:58.891399 ReadLammpsTraj-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1936 2023-05-31 05:31:22.000000 ReadLammpsTraj-1.1.2/README.md
+-rw-rw-rw-   0        0        0       30 2023-05-31 05:32:22.000000 ReadLammpsTraj-1.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 14:20:58.892399 ReadLammpsTraj-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      720 2023-05-31 14:20:07.000000 ReadLammpsTraj-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:20:58.878403 ReadLammpsTraj-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 14:20:58.888401 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/
+-rw-rw-rw-   0        0        0     2225 2023-05-31 14:20:58.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-05-31 14:20:58.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 14:20:58.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-31 14:20:58.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 14:20:58.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10480 2023-05-31 14:19:00.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.py
```

### Comparing `ReadLammpsTraj-1.1.1/LICENSE` & `ReadLammpsTraj-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.1/PKG-INFO` & `ReadLammpsTraj-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReadLammpsTraj
-Version: 1.1.1
+Version: 1.1.2
 Summary: Read lammps dump trajectory.
 Home-page: https://github.com/eastsheng/ReadLammpsTraj
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ReadLammpsTraj-1.1.1/README.md` & `ReadLammpsTraj-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.1/setup.py` & `ReadLammpsTraj-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'ReadLammpsTraj',
-version      = '1.1.1',
+version      = '1.1.2',
 py_modules   = ['ReadLammpsTraj'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/ReadLammpsTraj',
```

### Comparing `ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/PKG-INFO` & `ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReadLammpsTraj
-Version: 1.1.1
+Version: 1.1.2
 Summary: Read lammps dump trajectory.
 Home-page: https://github.com/eastsheng/ReadLammpsTraj
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.py` & `ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,47 @@
 # calculating the density,msd and rdf from lammps traj
 # id mol type mass x y z vx vy vz fx fy fz q
 import numpy as np 
 import pandas as pd
 
+
+def read_mass(lammpsdata):
+	"""
+	read atomic mass from lammps data. 
+	"""
+	data = open(lammpsdata,"r")
+	lines = data.read()
+	mass = []
+	(header,mass_other)=lines.split("\n\nMasses\n\n")
+	try:
+		try:
+			try:
+				(mass,other)=mass_other.split("\n\nPair Coeffs ")
+			except:
+				(mass,other)=mass_other.split("\n\nBond Coeffs ")
+		except:
+			(mass,other)=mass_other.split("\n\nAngle Coeffs ")
+	except:
+		(mass,other)=mass_other.split("\n\nAtoms # ")
+
+	mass=list(mass.split('\n'))
+	mass = list(filter(None, mass))
+	mass_id,mass_sub = [], []
+	for i in range(len(mass)):
+		mass_uu = mass[i].strip(" ").split(" ")
+		mass_id.append(int(mass_uu[0]))
+		mass_sub.append(float(mass_uu[1]))
+
+	pairs = zip(mass_id,mass_sub)
+	mass_dict = {k: v for k, v in pairs}
+
+	return mass_dict
+
+
+
 class ReadLammpsTraj(object):
 	"""docstring for ClassName"""
 	def __init__(self,f,timestep=1):
 		super(ReadLammpsTraj, self).__init__()
 		self.f = f
 		self.amu2g = 6.02214076208112e23
 		self.A2CM = 1e-8 
@@ -70,15 +105,18 @@
 		xL = vol_xyz[0,1]-vol_xyz[0,0]
 		yL = vol_xyz[1,1]-vol_xyz[1,0]
 		zL = vol_xyz[2,1]-vol_xyz[2,0]
 		vol = xL*yL*zL
 		return  vol
 
 	def read_mxyz(self,nframe):
-		# 不区分分子类型，计算所有的密度所需
+		"""
+		read mass, and x, y, z coordinates of nth frame from traj...
+		nframe: number of frame 
+		"""
 		traj = self.read_traj(nframe)
 		try:
 			self.mol = traj.loc[:,"mol"].values.astype(np.int64)#id mol type
 		except:
 			print("No molecule types in traj...")
 
 		try:
@@ -96,110 +134,159 @@
 		mxyz = np.hstack((mass.reshape(-1,1),xyz))
 
 		position = mxyz
 
 		return position
 
 	def read_traj(self,nframe):
-		# 读取所有数据
+		"""
+		read data of nth frame from traj...
+		nframe: number of frame 
+		"""
 		skip = 9*nframe+self.atom_n*(nframe-1)
 		traj = np.loadtxt(self.f,skiprows=skip,max_rows=self.atom_n,dtype="str")
 		print("Labels in traj is:",self.col)
 		traj = pd.DataFrame(traj,columns=self.col)
 		print(traj)
 		return traj
 
-	def oneframe_alldensity(self,mxyz,Nz,density_type="mass"):
-		# 只计算一帧的密度
+	def oneframe_alldensity(self,mxyz,Nbin,mass_dict={},density_type="mass",direction="z"):
+		"""
+		calculating density of all atoms......
+		mxyz: array of mass, x, y, and z;
+		Nbin: number of bins in x/y/z-axis
+		mass_dict: masses of atoms ,default={} 
+		density_type: calculated type of density 
+		"""
+
 		unitconvert = self.amu2g*(self.A2CM)**3
-		dZ = self.Lz/Nz #z方向bin
+		if direction=="z" or direction=="Z":
+			dr = self.Lz/Nbin #z方向bin
+			L = mxyz[:,3]
+			lo = self.zlo
+			vlo = (self.Lx*self.Ly*dr)*unitconvert
+		elif direction=="y" or direction=="Y":
+			dr = self.Ly/Nbin
+			L = mxyz[:,2]
+			lo = self.ylo
+			vlo = (self.Lx*self.Lz*dr)*unitconvert
+		elif direction=="x" or direction=="X":
+			dr = self.Lx/Nbin
+			L = mxyz[:,1]
+			lo = self.xlo
+			vlo = (self.Ly*self.Lz*dr)*unitconvert
+
+		mass_key=list(mass_dict.keys())
+		for i in range(len(self.atom)):
+			for j in range(len(mass_key)):
+				if self.atom[i] == mass_key[j]:
+					mxyz[i,0] = mass_dict[mass_key[j]]
 		MW = mxyz[:,0] #相对分子质量
+
 		if np.all(MW==0):
 			density_type = "number"
 			print("\nNo provided mass, will calculate number density!\n")
 		else:
 			density_type = "mass"
 
-		Z = mxyz[:,3] #z
 		rho_n = [] #average density list in every bins
-		zc_n  = []
-		# print(MW.shape,Z.shape)
-		for n in range(Nz):
+		lc_n  = []
+		for n in range(Nbin):
 			mass_n=0 #tot mass in bin
-			z0 = self.zlo+dZ*n #down coord of bin
-			z1 = self.zlo+dZ*(n+1)#up coord of bin
-			zc = (z0+z1)*0.5
-			# print(z0,z1,zc)
+			l0 = lo+dr*n #down coord of bin
+			l1 = lo+dr*(n+1)#up coord of bin
+			lc = (l0+l1)*0.5
 			for i in range(self.atom_n):
-				# if i atom in [z0:z1] 
-				if Z[i]>=z0 and Z[i]<=z1:
+				if L[i]>=l0 and L[i]<=l1:
 					if density_type == "mass":
 						mass_n = MW[i]+mass_n
 					else:
 						mass_n = mass_n+1
-			# print(mass_n)
-			vlo = (self.Lx*self.Ly*dZ)*unitconvert
-			# print(vlo)
 			rho = mass_n/vlo
 			# print(rho)
 			rho_n.append(rho)
-			zc_n.append(zc)
-		zc_n = np.array(zc_n).reshape(-1,1)
+			lc_n.append(lc)
+		lc_n = np.array(lc_n).reshape(-1,1)
 		rho_n = np.array(rho_n).reshape(-1,1)
 
-		return zc_n,rho_n
+		return lc_n,rho_n
 
-	def oneframe_moldensity(self,mxyz,Nz,mol_n,id_type="mol",density_type="mass"):
-		# 只计算一帧的密度
+	def oneframe_moldensity(self,mxyz,Nbin,id_range,mass_dict={},id_type="mol",density_type="mass",direction="z"):
+		"""
+		calculating density of some molecules......
+		mxyz: array of mass, x, y, and z;
+		Nbin: number of bins in x/y/z-axis
+		id_range: range of molecule/atom id;
+		mass_dict: masses of atoms ,default={} 
+		id_type: according to the molecule/atom id, to recognize atoms, args: mol, atom
+		density_type: calculated type of density 
+		"""
 		unitconvert = self.amu2g*(self.A2CM)**3
-		dZ = self.Lz/Nz #z方向bin
+		if direction=="z" or direction=="Z":
+			dr = self.Lz/Nbin #z方向bin
+			L = mxyz[:,3]
+			lo = self.zlo
+			vlo = (self.Lx*self.Ly*dr)*unitconvert
+		elif direction=="y" or direction=="Y":
+			dr = self.Ly/Nbin
+			L = mxyz[:,2]
+			lo = self.ylo
+			vlo = (self.Lx*self.Lz*dr)*unitconvert
+		elif direction=="x" or direction=="X":
+			dr = self.Lx/Nbin
+			L = mxyz[:,1]
+			lo = self.xlo
+			vlo = (self.Ly*self.Lz*dr)*unitconvert
+
+		mass_key=list(mass_dict.keys())
+		for i in range(len(self.atom)):
+			for j in range(len(mass_key)):
+				if self.atom[i] == mass_key[j]:
+					mxyz[i,0] = mass_dict[mass_key[j]]
 		MW = mxyz[:,0] #相对分子质量
 		if np.all(MW==0):
 			density_type = "number"
 			print("\nNo provided mass, will calculate number density!\n")
 		else:
 			density_type = "mass"
-		Z = mxyz[:,3] #z
+
 		rho_n = [] #average density list in every bins
-		zc_n  = []
+		lc_n  = []
 		# print(MW.shape,Z.shape)
 		if id_type == "mol":
 			id_know = self.mol
 		elif id_type == "atom":
 			id_know = self.atom
-		for n in range(Nz):
+		for n in range(Nbin):
 			mass_n=0 #tot mass in bin
-			z0 = self.zlo+dZ*n #down coord of bin
-			z1 = self.zlo+dZ*(n+1)#up coord of bin
-			zc = (z0+z1)*0.5
+			l0 = lo+dr*n #down coord of bin
+			l1 = lo+dr*(n+1)#up coord of bin
+			lc = (l0+l1)*0.5
 			# print(z0,z1,zc)
 			for i in range(self.atom_n):
-				if id_know[i]>=mol_n[0] and id_know[i]<=mol_n[1]:
+				if id_know[i]>=id_range[0] and id_know[i]<=id_range[1]:
 					# if i atom in [z0:z1]
-					if Z[i]>=z0 and Z[i]<=z1:
+					if L[i]>=l0 and L[i]<=l1:
 						if density_type == "mass":
 							mass_n = MW[i]+mass_n
 						else:
 							mass_n = mass_n+1
-			# print(mass_n)
-			vlo = (self.Lx*self.Ly*dZ)*unitconvert
-			# print(vlo)
 			rho = mass_n/vlo
 			# print(rho)
 			rho_n.append(rho)
-			zc_n.append(zc)
-		zc_n = np.array(zc_n).reshape(-1,1)
+			lc_n.append(lc)
+		lc_n = np.array(lc_n).reshape(-1,1)
 		rho_n = np.array(rho_n).reshape(-1,1)	
-		return zc_n,rho_n
+		return lc_n,rho_n
 
-	def TwoD_Density(self,mxyz,mol_n,Nx=1,Ny=1,Nz=1,mass_or_number="mass"):
+	def TwoD_Density(self,mxyz,id_range,Nx=1,Ny=1,Nz=1,mass_or_number="mass"):
 		'''
 		mxyz: mass x y z
 		atom_n: tot number of atoms
-		mol_n: type of molecules,list,mol_n=[1,36], the 1 is the first mol type and 36 is the last one mol type
+		id_range: type of molecules,list,id_range=[1,36], the 1 is the first mol type and 36 is the last one mol type
 		Nx,Ny,Nz: layer number of x , y, z for calculating density, which is relate to the precision of density,
 		and default is 1, that is, the total density.
 		mass_or_number: "mass: mass density; number: number density"
 		'''
 		unitconvert = self.amu2g*(self.A2CM)**3
 		dX = self.Lz/Nx #x方向bin
 		dY = self.Lz/Ny #y方向bin
@@ -229,15 +316,15 @@
 					zc = (z0+z1)*0.5
 					zc_n.append(zc)
 		
 					n=0 #tot mass or number in bin
 
 					for i in range(self.atom_n):
 						
-						if self.mol[i]>=mol_n[0] and self.mol[i]<=mol_n[1]:
+						if self.mol[i]>=id_range[0] and self.mol[i]<=id_range[1]:
 							if X[i]>=x0 and X[i]<=x1 and Y[i]>=y0 and Y[i]<=y1 and Z[i]>=z0 and Z[i]<=z1:
 								if mass_or_number == "mass":
 									n = MW[i]+n
 								elif mass_or_number == "number":
 									n = n+1
 									# print(i,'---',self.atom_n,MW[i])
 					vlo = (dX*dY*dZ)*unitconvert
```

