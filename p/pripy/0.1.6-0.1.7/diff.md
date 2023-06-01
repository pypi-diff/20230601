# Comparing `tmp/pripy-0.1.6.tar.gz` & `tmp/pripy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pripy-0.1.6.tar", last modified: Mon Apr  4 02:28:49 2022, max compression
+gzip compressed data, was "pripy-0.1.7.tar", last modified: Thu Jun  1 06:34:42 2023, max compression
```

## Comparing `pripy-0.1.6.tar` & `pripy-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,27 @@
-drwxr-xr-x   0 jcranney   (503) staff       (20)        0 2022-04-04 02:28:49.762379 pripy-0.1.6/
--rw-r--r--   0 jcranney   (503) staff       (20)     1327 2022-04-04 02:28:49.762602 pripy-0.1.6/PKG-INFO
--rw-r--r--   0 jcranney   (503) staff       (20)      854 2022-02-08 00:10:30.000000 pripy-0.1.6/README.md
-drwxr-xr-x   0 jcranney   (503) staff       (20)        0 2022-04-04 02:28:49.760349 pripy-0.1.6/pripy/
--rw-r--r--   0 jcranney   (503) staff       (20)      133 2022-03-01 06:28:14.000000 pripy-0.1.6/pripy/__init__.py
--rw-r--r--   0 jcranney   (503) staff       (20)    24756 2022-04-04 02:26:17.000000 pripy-0.1.6/pripy/algos.py
--rw-r--r--   0 jcranney   (503) staff       (20)     5859 2022-02-08 00:09:06.000000 pripy-0.1.6/pripy/core.py
--rw-r--r--   0 jcranney   (503) staff       (20)    17423 2022-03-01 06:28:14.000000 pripy-0.1.6/pripy/util.py
-drwxr-xr-x   0 jcranney   (503) staff       (20)        0 2022-04-04 02:28:49.762016 pripy-0.1.6/pripy.egg-info/
--rw-r--r--   0 jcranney   (503) staff       (20)     1327 2022-04-04 02:28:49.000000 pripy-0.1.6/pripy.egg-info/PKG-INFO
--rw-r--r--   0 jcranney   (503) staff       (20)      239 2022-04-04 02:28:49.000000 pripy-0.1.6/pripy.egg-info/SOURCES.txt
--rw-r--r--   0 jcranney   (503) staff       (20)        1 2022-04-04 02:28:49.000000 pripy-0.1.6/pripy.egg-info/dependency_links.txt
--rw-r--r--   0 jcranney   (503) staff       (20)       12 2022-04-04 02:28:49.000000 pripy-0.1.6/pripy.egg-info/requires.txt
--rw-r--r--   0 jcranney   (503) staff       (20)        6 2022-04-04 02:28:49.000000 pripy-0.1.6/pripy.egg-info/top_level.txt
--rw-r--r--   0 jcranney   (503) staff       (20)      104 2022-03-01 06:28:14.000000 pripy-0.1.6/pyproject.toml
--rw-r--r--   0 jcranney   (503) staff       (20)      581 2022-04-04 02:28:49.763620 pripy-0.1.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:34:42.199560 pripy-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-06-01 06:34:38.000000 pripy-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-06-01 06:34:42.199560 pripy-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-06-01 06:34:38.000000 pripy-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:34:42.198560 pripy-0.1.7/gym_gmtphasing/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-01 06:34:38.000000 pripy-0.1.7/gym_gmtphasing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:34:42.198560 pripy-0.1.7/gym_gmtphasing/envs/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-01 06:34:38.000000 pripy-0.1.7/gym_gmtphasing/envs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7426 2023-06-01 06:34:38.000000 pripy-0.1.7/gym_gmtphasing/envs/gmtphasing_env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:34:42.198560 pripy-0.1.7/gym_phasediversity/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-01 06:34:38.000000 pripy-0.1.7/gym_phasediversity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:34:42.198560 pripy-0.1.7/gym_phasediversity/envs/
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-01 06:34:38.000000 pripy-0.1.7/gym_phasediversity/envs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7938 2023-06-01 06:34:38.000000 pripy-0.1.7/gym_phasediversity/envs/phasediversity_env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:34:42.198560 pripy-0.1.7/pripy/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-01 06:34:38.000000 pripy-0.1.7/pripy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24947 2023-06-01 06:34:38.000000 pripy-0.1.7/pripy/algos.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-06-01 06:34:38.000000 pripy-0.1.7/pripy/core.py
+-rw-r--r--   0 root         (0) root         (0)    13587 2023-06-01 06:34:38.000000 pripy-0.1.7/pripy/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:34:42.199560 pripy-0.1.7/pripy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-06-01 06:34:42.000000 pripy-0.1.7/pripy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      457 2023-06-01 06:34:42.000000 pripy-0.1.7/pripy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 06:34:42.000000 pripy-0.1.7/pripy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-01 06:34:42.000000 pripy-0.1.7/pripy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-01 06:34:42.000000 pripy-0.1.7/pripy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-01 06:34:38.000000 pripy-0.1.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      642 2023-06-01 06:34:42.199560 pripy-0.1.7/setup.cfg
```

### Comparing `pripy-0.1.6/pripy/algos.py` & `pripy-0.1.7/pripy/algos.py`

 * *Files 2% similar despite different names*

```diff
@@ -519,20 +519,22 @@
             cplxim_shft = cp.fft.fft2(cplxpup_shft)
             
             phaseim_shft = cp.angle(cplxim_shft)
             ampim_shft = cp.abs(cplxim_shft)
             
             cplxim_shft2 = ((1.+hio_param)*amp_shft-hio_param*ampim_shft)*cp.exp(1j*phaseim_shft)
             if invalid_pixels is not None:
-                cplxim_shft2[invalid_pixels] = cplxim_shft[invalid_pixels].copy() 
+                cplxim_shft2[invalid_pixels] = cplxim_shft[invalid_pixels].copy()
 
             cplxpup_shft2 = cp.fft.ifft2(cplxim_shft2)
             self._phasepup_shft = cp.angle(cplxpup_shft2)
             amppup_shft = cp.abs(cplxpup_shft2)
         
+        # save the image computed from the GS estimated phase (for debugging):
+        self._gs_im = (cp.fft.fftshift(ampim_shft)**2)*(self._imsum/self._scf)
         return self._phasepup_shft.copy()
 
     def compute_phase(self,im,iters=100,hio_param=0.3,discard_invalid=True):
         """Compute and return the phase estimated by the Gerchberg-Saxton algorithm,
         given an image.
 
         Args:
@@ -540,15 +542,16 @@
             iters (int): Number of iterations of GS to perform.
             hio_param (float): Parameter for the Hybrid Input-Output (HIO) step.
             discard_invalid (bool): If True, discard invalid pixels in WFS image.
 
         Returns:
             np.ndarray: Phase estimate (in wavelength units).
         """
-        im = cp.array(im)*(self._scf/im.sum())
+        self._imsum = im.sum()
+        im = cp.array(im)*(self._scf/self._imsum)
         im = cp.pad(im,(self._fft_width-self._im_width)//2)
         im = im**0.5
         im_shft = cp.fft.fftshift(im)
         
         # check if user wants to discard invalid pixels this time
         if discard_invalid:
             invalid_pixels = self.invalid_pixels
```

### Comparing `pripy-0.1.6/pripy/core.py` & `pripy-0.1.7/pripy/core.py`

 * *Files identical despite different names*

### Comparing `pripy-0.1.6/pripy/util.py` & `pripy-0.1.7/pripy/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 try:
     import cupy as cp
+    def get(x):
+        return x.get()
 except ImportError as ie:
     Warning("No cupy available, using basic numpy")
     import numpy as cp
+    def get(x):
+        return x
 
 import numpy as np
 
 from scipy.special import factorial
 import scipy.linalg as la
 
 class TaylorHModel:
@@ -48,15 +52,15 @@
             CPU = False
         else:
             raise TypeError("input x must be either numpy or cupy array")
         out = self.dny[0].copy()
         for ni in range(1,order+1):
             out += (1/factorial(ni))*cp.einsum(self._einstring_eval[ni],self.dny[ni],*([x]*ni))
         if CPU:
-            return out.get()
+            return get(out)
         else:
             return out
     
     def jacobian(self,x,order=None): 
         if order is None:
             order = self._order
         if type(x) is np.ndarray:
@@ -66,15 +70,15 @@
             CPU = False
         else:
             raise TypeError("input x must be either numpy or cupy array")
         out = self.dny[1].copy()
         for ni in range(1,order+1-1):
             out += (1/factorial(ni))*cp.einsum(self._einstring_jac[ni],self.dny[ni+1],*([x]*ni))
         if CPU:
-            return out.get()
+            return get(out)
         else:
             return out
         
     def hessian(self,x,order=None): 
         if order is None:
             order = self._order
         if type(x) is np.ndarray:
@@ -84,129 +88,31 @@
             CPU = False
         else:
             raise TypeError("input x must be either numpy or cupy array")
         out = self.dny[2].copy()
         for ni in range(1,order+1-2):
             out += (1/factorial(ni))*cp.einsum(self._einstring_hess[ni],self.dny[ni+2],*([x]*ni))
         if CPU:
-            return out.get()
+            return get(out)
         else:
             return out
 
-    def ceo_build_dnys(self,gmt,src,imgr):
-        n_px_fft = imgr.DFT_osf*imgr.N_PX_PUPIL
-        pup = src.amplitude.host()
-        xx,yy = np.meshgrid(np.arange(pup.shape[0]),np.arange(pup.shape[0]))
-
-        pup_mask = pup==1
-
-        phi = pup.copy()
-
-        dft_matrix = la.dft(n_px_fft)
-        dft_matrix = np.concatenate([dft_matrix[n_px_fft//2:,:],dft_matrix[:n_px_fft//2,]],axis=0)
-        dft_matrix = dft_matrix[:,:src.phase.shape[0]]
-        dft_matrix = dft_matrix[(n_px_fft-imgr.N_PX_IMAGE)//2+1:(n_px_fft+imgr.N_PX_IMAGE)//2+1,:]
-        dft_matrix = np.kron(dft_matrix,dft_matrix)
-        dft_matrix = dft_matrix[:,pup_mask.flatten()]
-
-        ~gmt
-
-        mode_to_phase = np.zeros([pup_mask.sum(),self._nstate])
-
-        state = gmt.state
-        x = state["M1"]["Txyz"][:,2]
-        x *= 0.0
-        gmt^=state
-        ~imgr
-        +src
-        
-        for i in range(self._nstate):
-            x *= 0.0
-            delta = 1e-7
-            x[i] = delta
-            gmt^=state
-            +src
-            phi = src.phase.host()
-            mode_to_phase[:,i] = phi[pup_mask]/delta
-
-        wavelength = src.wavelength
-        self.wavelength = wavelength
-
-        g0 = np.exp((1j*2*np.pi*(xx+yy)/pup.shape[0]/4))[pup_mask]
-        self.g = lambda x: np.exp((1j*2*np.pi)*(mode_to_phase@x/wavelength+g0))
-        self.h_true = lambda x: np.abs(dft_matrix @ self.g(x))**2
-        self._mode_to_phase = mode_to_phase        
-        self._dft_matrix    = dft_matrix
-
-        d0h = np.abs(dft_matrix @ g0)**2
-        self.set_dny(d0h,0)
-        if self._order < 1:
-            return
-        
-        d1h = np.zeros([imgr.N_PX_IMAGE**2,self._nstate])
-        for ell1 in range(self._nstate):
-            m_ell_ = mode_to_phase[:,ell1]
-            d1h[:,ell1] = 2*(2*np.pi/wavelength)*((-1j)*((dft_matrix@(g0*m_ell_))).conj()*(dft_matrix@g0)).real
-        self.set_dny(d1h,1)
-        if self._order < 2:
-            return
-
-        d2h = np.zeros([imgr.N_PX_IMAGE**2,self._nstate,self._nstate])
-        for ell1 in range(self._nstate):
-            for ell2 in range(ell1+1):
-                m_ell_1 = mode_to_phase[:,ell1]
-                m_ell_2 = mode_to_phase[:,ell2]
-                tmp = 2*((-1j*2*np.pi/wavelength)**2*(
-                            (dft_matrix@(g0*m_ell_1*m_ell_2)).conj()*(dft_matrix@g0)
-                            - (dft_matrix@(g0*m_ell_1)).conj()*(dft_matrix@(g0*m_ell_2))
-                        )).real
-                d2h[:,ell1,ell2] = tmp
-                d2h[:,ell2,ell1] = tmp
-        self.set_dny(d2h,2)
-        if self._order < 3:
-            return
-            
-        d3h = np.zeros([imgr.N_PX_IMAGE**2,self._nstate,self._nstate,self._nstate])
-        for ell1 in range(self._nstate):
-            for ell2 in range(ell1+1):
-                for ell3 in range(ell2+1):
-                    m_ell_1 = mode_to_phase[:,ell1]
-                    m_ell_2 = mode_to_phase[:,ell2]
-                    m_ell_3 = mode_to_phase[:,ell3]
-                    tmp = 2*((-1j*2*np.pi/wavelength)**3*(
-                            (dft_matrix@(g0*m_ell_1*m_ell_2*m_ell_3)).conj()*(dft_matrix@g0)
-                            - (dft_matrix@(g0*m_ell_1*m_ell_2)).conj()*(dft_matrix@(g0*m_ell_3))
-                            - (dft_matrix@(g0*m_ell_1*m_ell_3)).conj()*(dft_matrix@(g0*m_ell_2))
-                            - (dft_matrix@(g0*m_ell_2*m_ell_3)).conj()*(dft_matrix@(g0*m_ell_1))
-                        )).real
-                    d3h[:,ell1,ell2,ell3] = tmp
-                    d3h[:,ell1,ell3,ell2] = tmp
-                    d3h[:,ell2,ell1,ell3] = tmp
-                    d3h[:,ell2,ell3,ell1] = tmp
-                    d3h[:,ell3,ell1,ell2] = tmp
-                    d3h[:,ell3,ell2,ell1] = tmp
-        self.set_dny(d3h,3)
-        if self._order < 4:
-            return
-        else:
-            raise ValueError("maximum taylor order implemented is 3")
-    
     def exact_jacobian(self,x):
         if type(x) is np.ndarray:
             CPU = True
             x = cp.array(x)
         elif type(x) is cp.ndarray:
             CPU = False
         else:
             raise TypeError("input x must be either numpy or cupy array")
         b = self._dft_matrix_cp*self.g_cp(x)[None,:]
         out = ((b @ self._mode_to_phase_cp) * (b.conj().sum(axis=1))[:,None]).imag
         out *= -(2*cp.pi/self.wavelength)*2 # not sure why negative here, should be positive surely
         if CPU:
-            return out.get()
+            return get(out)
         else:
             return out
     
     def _exact_jacobian(self,x):
         # deprecated, will be deleted soon
         b = self._dft_matrix*self.g(x)[None,:]
         d1h = ((b @ self._mode_to_phase) * (b.conj().sum(axis=1))[:,None]).imag
@@ -256,15 +162,15 @@
             function is a purely linear combination, then delta doesn't matter.
         """
 
         pup_width = pup.shape[0]
         nstate = self._nstate
         nmeas = self._nmeas
 
-        dft_matrix = la.dft(fft_width,scale=None)
+        dft_matrix = la.dft(fft_width,scale="sqrtn")
         dft_matrix = np.concatenate([dft_matrix[fft_width//2:,:],dft_matrix[:fft_width//2,]],axis=0)
         dft_matrix = dft_matrix[:,:pup_width]
         dft_matrix = dft_matrix[fft_width//2-im_width//2:fft_width//2+im_width//2,:]
         dft_matrix = np.kron(dft_matrix,dft_matrix)
         dft_matrix = dft_matrix[:,(pup==1).flatten()]
 
         mode_to_phase = np.zeros([(pup==1).sum(),nstate])
```

### Comparing `pripy-0.1.6/setup.cfg` & `pripy-0.1.7/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pripy
-version = 0.1.6
+version = 0.1.7
 author = Jesse Cranney
 author_email = jesse.cranney@anu.edu.au
 description = Phase Retrieval algorithms in Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcranney/pripy.git
 classifiers = 
@@ -14,13 +14,20 @@
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	numpy
 	scipy
+	aotools
+	torch
+	gym
+	gymnasium
+	pygame
+	ipython
+	matplotlib
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

