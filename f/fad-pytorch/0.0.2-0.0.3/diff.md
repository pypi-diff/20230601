# Comparing `tmp/fad_pytorch-0.0.2.tar.gz` & `tmp/fad_pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fad_pytorch-0.0.2.tar", last modified: Thu May 25 07:14:45 2023, max compression
+gzip compressed data, was "fad_pytorch-0.0.3.tar", last modified: Wed May 31 23:03:54 2023, max compression
```

## Comparing `fad_pytorch-0.0.2.tar` & `fad_pytorch-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-05-25 07:14:45.586429 fad_pytorch-0.0.2/
--rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-05-24 22:59:09.000000 fad_pytorch-0.0.2/LICENSE
--rw-r--r--   0 shawley    (501) staff       (20)      111 2023-05-24 22:59:09.000000 fad_pytorch-0.0.2/MANIFEST.in
--rw-r--r--   0 shawley    (501) staff       (20)     2290 2023-05-25 07:14:45.586285 fad_pytorch-0.0.2/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)     1488 2023-05-25 07:08:29.000000 fad_pytorch-0.0.2/README.md
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-05-25 07:14:45.585347 fad_pytorch-0.0.2/fad_pytorch/
--rw-r--r--   0 shawley    (501) staff       (20)       22 2023-05-25 06:50:08.000000 fad_pytorch-0.0.2/fad_pytorch/__init__.py
--rw-r--r--   0 shawley    (501) staff       (20)     3033 2023-05-25 06:50:08.000000 fad_pytorch-0.0.2/fad_pytorch/_modidx.py
--rw-r--r--   0 shawley    (501) staff       (20)      142 2023-05-24 22:59:09.000000 fad_pytorch-0.0.2/fad_pytorch/core.py
--rw-r--r--   0 shawley    (501) staff       (20)    10209 2023-05-25 07:08:29.000000 fad_pytorch-0.0.2/fad_pytorch/fad_embed.py
--rw-r--r--   0 shawley    (501) staff       (20)      871 2023-05-24 22:59:09.000000 fad_pytorch-0.0.2/fad_pytorch/fad_gen.py
--rw-r--r--   0 shawley    (501) staff       (20)     3201 2023-05-25 07:08:29.000000 fad_pytorch-0.0.2/fad_pytorch/fad_score.py
--rw-r--r--   0 shawley    (501) staff       (20)   122806 2023-05-25 07:08:29.000000 fad_pytorch-0.0.2/fad_pytorch/pann.py
--rw-r--r--   0 shawley    (501) staff       (20)     9559 2023-05-25 06:50:08.000000 fad_pytorch-0.0.2/fad_pytorch/pann_pytorch_utils.py
--rw-r--r--   0 shawley    (501) staff       (20)     8256 2023-05-25 04:12:34.000000 fad_pytorch-0.0.2/fad_pytorch/sqrtm.py
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-05-25 07:14:45.586111 fad_pytorch-0.0.2/fad_pytorch.egg-info/
--rw-r--r--   0 shawley    (501) staff       (20)     2290 2023-05-25 07:14:45.000000 fad_pytorch-0.0.2/fad_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)      512 2023-05-25 07:14:45.000000 fad_pytorch-0.0.2/fad_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2023-05-25 07:14:45.000000 fad_pytorch-0.0.2/fad_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 shawley    (501) staff       (20)      176 2023-05-25 07:14:45.000000 fad_pytorch-0.0.2/fad_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2023-05-24 22:59:30.000000 fad_pytorch-0.0.2/fad_pytorch.egg-info/not-zip-safe
--rw-r--r--   0 shawley    (501) staff       (20)       81 2023-05-25 07:14:45.000000 fad_pytorch-0.0.2/fad_pytorch.egg-info/requires.txt
--rw-r--r--   0 shawley    (501) staff       (20)       12 2023-05-25 07:14:45.000000 fad_pytorch-0.0.2/fad_pytorch.egg-info/top_level.txt
--rw-r--r--   0 shawley    (501) staff       (20)     1144 2023-05-25 06:50:08.000000 fad_pytorch-0.0.2/settings.ini
--rw-r--r--   0 shawley    (501) staff       (20)       38 2023-05-25 07:14:45.586469 fad_pytorch-0.0.2/setup.cfg
--rw-r--r--   0 shawley    (501) staff       (20)     2596 2023-05-24 22:59:09.000000 fad_pytorch-0.0.2/setup.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-05-31 23:03:54.043086 fad_pytorch-0.0.3/
+-rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-05-24 22:59:09.000000 fad_pytorch-0.0.3/LICENSE
+-rw-r--r--   0 shawley    (501) staff       (20)      111 2023-05-24 22:59:09.000000 fad_pytorch-0.0.3/MANIFEST.in
+-rw-r--r--   0 shawley    (501) staff       (20)     2290 2023-05-31 23:03:54.042942 fad_pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)     1488 2023-05-25 07:08:29.000000 fad_pytorch-0.0.3/README.md
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-05-31 23:03:54.041853 fad_pytorch-0.0.3/fad_pytorch/
+-rw-r--r--   0 shawley    (501) staff       (20)       22 2023-05-31 21:26:13.000000 fad_pytorch-0.0.3/fad_pytorch/__init__.py
+-rw-r--r--   0 shawley    (501) staff       (20)    31046 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/_modidx.py
+-rw-r--r--   0 shawley    (501) staff       (20)      142 2023-05-24 22:59:09.000000 fad_pytorch-0.0.3/fad_pytorch/core.py
+-rw-r--r--   0 shawley    (501) staff       (20)    12366 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/fad_embed.py
+-rw-r--r--   0 shawley    (501) staff       (20)     4423 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/fad_gen.py
+-rw-r--r--   0 shawley    (501) staff       (20)     3773 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/fad_score.py
+-rw-r--r--   0 shawley    (501) staff       (20)   123697 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/pann.py
+-rw-r--r--   0 shawley    (501) staff       (20)     9559 2023-05-25 06:50:08.000000 fad_pytorch-0.0.3/fad_pytorch/pann_pytorch_utils.py
+-rw-r--r--   0 shawley    (501) staff       (20)     8474 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/sqrtm.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-05-31 23:03:54.042769 fad_pytorch-0.0.3/fad_pytorch.egg-info/
+-rw-r--r--   0 shawley    (501) staff       (20)     2290 2023-05-31 23:03:53.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)      512 2023-05-31 23:03:54.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2023-05-31 23:03:53.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 shawley    (501) staff       (20)      176 2023-05-31 23:03:53.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2023-05-24 22:59:30.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/not-zip-safe
+-rw-r--r--   0 shawley    (501) staff       (20)       81 2023-05-31 23:03:53.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/requires.txt
+-rw-r--r--   0 shawley    (501) staff       (20)       12 2023-05-31 23:03:53.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 shawley    (501) staff       (20)     1144 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/settings.ini
+-rw-r--r--   0 shawley    (501) staff       (20)       38 2023-05-31 23:03:54.043126 fad_pytorch-0.0.3/setup.cfg
+-rw-r--r--   0 shawley    (501) staff       (20)     2596 2023-05-24 22:59:09.000000 fad_pytorch-0.0.3/setup.py
```

### Comparing `fad_pytorch-0.0.2/LICENSE` & `fad_pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.2/PKG-INFO` & `fad_pytorch-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fad_pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Frechet Audio Distance evaluation in PyTorch
 Home-page: https://github.com/drscotthawley/fad_pytorch
 Author: Scott H. Hawley
 Author-email: scott.hawley@belmont.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fad_pytorch-0.0.2/README.md` & `fad_pytorch-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.2/fad_pytorch/fad_embed.py` & `fad_pytorch-0.0.3/fad_pytorch/fad_embed.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,87 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_fad_embed.ipynb.
 
 # %% auto 0
-__all__ = ['GUDGUD_LICENSE', 'setup_embedder', 'embed_all', 'main']
+__all__ = ['GUDGUD_LICENSE', 'download_file', 'get_ckpt', 'setup_embedder', 'embed_all', 'main']
 
-# %% ../nbs/02_fad_embed.ipynb 4
+# %% ../nbs/02_fad_embed.ipynb 5
 import os
 import argparse
 import laion_clap 
 from laion_clap.training.data import get_audio_features
 from accelerate import Accelerator
 import warnings
 import torch
 
 from aeiou.core import get_device, load_audio, get_audio_filenames, makedir
 from aeiou.datasets import AudioDataset
 from aeiou.hpc import HostPrinter
 from torch.utils.data import DataLoader
 from pathlib import Path
-from .pann import Cnn14_16k
+import requests 
+from tqdm import tqdm
 
+try:
+    from fad_pytorch.pann import Cnn14_16k
+except: 
+    from pann import Cnn14_16k
 
-# %% ../nbs/02_fad_embed.ipynb 5
+# %% ../nbs/02_fad_embed.ipynb 7
+def download_file(url, local_filename):
+    "Includes a progress bar.  from https://stackoverflow.com/a/37573701/4259243"
+    response = requests.get(url, stream=True)
+    total_size_in_bytes= int(response.headers.get('content-length', 0))
+    block_size = 1024 #1 Kilobye
+    progress_bar = tqdm(total=total_size_in_bytes, unit='iB', unit_scale=True)
+    with open(local_filename, 'wb') as file:
+        for data in response.iter_content(block_size):
+            progress_bar.update(len(data))
+            file.write(data)
+    progress_bar.close()
+    if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
+        print("ERROR, something went wrong")
+    return local_filename
+
+def get_ckpt(ckpt_file='music_speech_audioset_epoch_15_esc_89.98.pt',
+             ckpt_base_url='https://huggingface.co/lukewys/laion_clap/blob/main',
+             ckpt_dl_path=os.path.expanduser("~/checkpoints")
+            ):
+    ckpt_path = f"{ckpt_dl_path}/{ckpt_file}"
+    if not os.path.isfile(ckpt_path):
+        print(f"File {ckpt_path} not found, downloading from {ckpt_base_url}/{ckpt_file}")
+        download_file( f"{ckpt_base_url}/{ckpt_file}", ckpt_path)
+    return ckpt_path
+
+# %% ../nbs/02_fad_embed.ipynb 8
 def setup_embedder(
         model_choice='clap', # 'clap' | 'vggish' | 'pann'
-        device='cuda',              
+        device='cuda',
+        ckpt_file='music_speech_audioset_epoch_15_esc_89.98.pt',  # NOTE: 'CLAP_CKPT' env var overrides ckpt_file kwarg
+        ckpt_base_url='https://huggingface.co/lukewys/laion_clap/resolve/main',
+        # https://huggingface.co/lukewys/laion_clap/resolve/main/music_speech_audioset_epoch_15_esc_89.98.pt
+        accelerator=None,
+        ckpt_dl_path=os.path.expanduser("~/checkpoints"),
     ):
     "load the embedder model"
     embedder = None
     
     if model_choice == 'clap':
         clap_fusion, clap_amodel = True, "HTSAT-base"
         #doesn't work:  warnings.filterwarnings('ignore')  # temporarily disable CLAP warnings as they are super annoying. 
         clap_module = laion_clap.CLAP_Module(enable_fusion=clap_fusion, device=device, amodel=clap_amodel).requires_grad_(False).eval()
-        clap_ckpt_path = os.environ['CLAP_CKPT']  # you'll need access to this .ckpt file
-        if clap_ckpt_path:
+        clap_ckpt_path = os.getenv('CLAP_CKPT')  # NOTE: CLAP_CKPT env var overrides ckpt_file kwarg
+        if clap_ckpt_path is not None:
             #print(f"Loading CLAP from {clap_ckpt_path}")
             clap_module.load_ckpt(ckpt=clap_ckpt_path, verbose=False)
         else:
-            clap_module.load_ckpt(model_id=1, verbose=False)
+            if accelerator is None or accelerator.is_main_process: print(f"No CLAP checkpoint specified, using {ckpt_file}") 
+            clap_module = laion_clap.CLAP_Module(enable_fusion=False, amodel= 'HTSAT-base')
+            ckpt_path = get_ckpt(ckpt_file=ckpt_file, ckpt_base_url=ckpt_base_url, ckpt_dl_path=ckpt_dl_path)
+            clap_module.load_ckpt(ckpt_path, verbose=False)
+            #clap_module.load_ckpt(model_id=1, verbose=False)
         #warnings.filterwarnings("default")   # turn warnings back on. 
         embedder = clap_module # synonyms 
         sample_rate = 48000
         
     # next two model loading codes from gudgud96's repo: https://github.com/gudgud96/frechet-audio-distance, LICENSE below
     elif model_choice == "vggish":   # https://arxiv.org/abs/1609.09430
         embedder = torch.hub.load('harritaylor/torchvggish', 'vggish')
@@ -87,24 +127,24 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-# %% ../nbs/02_fad_embed.ipynb 7
+# %% ../nbs/02_fad_embed.ipynb 10
 def embed_all(args): 
     model_choice, real_path, fake_path, chunk_size, sr, max_batch_size = args.embed_model, args.real_path, args.fake_path, args.chunk_size, args.sr, args.batch_size
     local_rank = int(os.environ.get("LOCAL_RANK", 0))
     world_size = int(os.environ.get("WORLD_SIZE", 1))
     ddps = f"[{local_rank}/{world_size}]"  # string for distributed computing info, e.g. "[1/8]" 
 
     accelerator = Accelerator()
     hprint = HostPrinter(accelerator)  # hprint only prints on head node
-    device = accelerator.device  # get_device()
+    device = accelerator.device    # get_device()
     hprint(f"{ddps} args = {args}")
     hprint(f'{ddps} Using device: {device}')
     
  
     """ # let accelerate split up the files among processsors
     # get the list(s) of audio files
     real_filenames = get_audio_filenames(real_path)
@@ -120,15 +160,15 @@
     start = local_rank * num_per_proc
     end =  minlen if local_rank == world_size-1 else (local_rank+1) * num_per_proc
     #print(f"{ddps} start, end = ",start,end) 
     real_filenames, fake_filenames = real_filenames[start:end], fake_filenames[start:end]
     """
 
     # setup embedder and dataloader
-    embedder, emb_sample_rate = setup_embedder(model_choice, device)
+    embedder, emb_sample_rate = setup_embedder(model_choice, device, accelerator)
     if sr != emb_sample_rate:
         hprint(f"\n*******\nWARNING: sr={sr} != {model_choice}'s emb_sample_rate={emb_sample_rate}. Will resample audio to the latter\n*******\n")
         sr = emb_sample_rate
     hprint(f"{ddps} Embedder '{model_choice}' ready to go!")
 
     real_dataset = AudioDataset(real_path, augs='Stereo(), PhaseFlipper()', sample_rate=emb_sample_rate, sample_size=chunk_size, return_dict=True, verbose=args.verbose)
     fake_dataset = AudioDataset(fake_path, augs='Stereo(), PhaseFlipper()', sample_rate=emb_sample_rate, sample_size=chunk_size, return_dict=True, verbose=args.verbose)
@@ -177,24 +217,24 @@
                 hprint(f"embeddings.shape = {embeddings.shape}")
                 # TODO: for now we'll just dump each batch on each proc to its own file; this could be improved
                 outfilename = f"{newdir}/emb_p{local_rank}_b{i}.pt"
                 print(f"{ddps} Saving embeddings to {outfilename}")
                 torch.save(embeddings.cpu().detach(), outfilename)
     return        
 
-# %% ../nbs/02_fad_embed.ipynb 9
+# %% ../nbs/02_fad_embed.ipynb 11
 def main(): 
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('embed_model', help='chioce of embedding model: clap | vggish | pann', default='clap')
+    parser.add_argument('embed_model', help='choice of embedding model: clap | vggish | pann', default='clap')
     parser.add_argument('real_path', help='Path of files of real audio', default='real/')
     parser.add_argument('fake_path', help='Path of files of fake audio', default='fake/')
     parser.add_argument('--chunk_size', type=int, default=24000, help='Length of chunks (in audio samples) to embed')
     parser.add_argument('--batch_size', type=int, default=64, help='MAXIMUM Batch size for computing embeddings (may go smaller)')
     parser.add_argument('--sr', type=int, default=48000, help='sample rate (will resample inputs at this rate)')
     parser.add_argument('--verbose', action='store_true',  help='Show notices of resampling when reading files')
 
     args = parser.parse_args()
     embed_all(args)
 
-# %% ../nbs/02_fad_embed.ipynb 10
+# %% ../nbs/02_fad_embed.ipynb 12
 if __name__ == '__main__' and "get_ipython" not in dir():
     main()
```

### Comparing `fad_pytorch-0.0.2/fad_pytorch/fad_score.py` & `fad_pytorch-0.0.3/fad_pytorch/fad_score.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,49 +27,55 @@
 def calc_mu_sigma(emb): 
     "calculates mean and covariance matrix of batched embeddings"
     mu = torch.mean(emb, axis=0)
     sigma = torch.cov(emb.T)
     return mu, sigma
 
 # %% ../nbs/03_fad_score.ipynb 10
-def calc_score(args, debug=False): 
-    real_emb_path, fake_emb_path = args.real_emb_path, args.fake_emb_path
+def calc_score(real_emb_path, # where real embeddings are stored
+               fake_emb_path, # where fake embeddings are stored
+               method='maji', # sqrtm calc method: 'maji'|'li'
+               debug=False
+               ): 
     print(f"Calculating FAD score for files in {real_emb_path}/ vs. {fake_emb_path}/")
     emb_real = read_embeddings(emb_path=real_emb_path, debug=debug)
     emb_fake = read_embeddings(emb_path=fake_emb_path, debug=debug)
     if debug: print(emb_real.shape, emb_fake.shape)
     
     mu_real, sigma_real = calc_mu_sigma(emb_real) 
     mu_fake, sigma_fake = calc_mu_sigma(emb_fake) 
     if debug:
         print("mu_real.shape, sigma_real.shape =",mu_real.shape, sigma_real.shape)
         print("mu_fake.shape, sigma_fake.shape =",mu_fake.shape, sigma_fake.shape)
     
-    diff = mu_real - mu_fake
+    mu_diff = mu_real - mu_fake
     if debug:
-        print("diff = ",diff) 
-        score1 = diff.dot(diff)
-        print("score1 = ",score1)
+        print("mu_diff = ",mu_diff) 
+        score1 = mu_diff.dot(mu_diff)
+        print("score1: mu_diff.dot(mu_diff) = ",score1)
         score2 = torch.trace(sigma_real)
-        print("score2 = ", score2)
+        print("score2: torch.trace(sigma_real) = ", score2)
         score3 = torch.trace(sigma_fake)
-        print("score3 = ",score3)
+        print("score3: torch.trace(sigma_fake) = ",score3)
         score_p = sqrtm( torch.matmul( sigma_real, sigma_fake) )
-        print("score_p.shape = ",score_p.shape) 
-        score4 = -2* torch.trace ( torch.real ( sqrtm( torch.matmul( sigma_real, sigma_fake)  ) ) )
-        print("score4 = ",score4) 
+        print("score_p.shape (matmul) = ",score_p.shape) 
+        score4 = -2* torch.trace ( torch.real ( sqrtm( torch.matmul( sigma_real, sigma_fake) , method=method ) ) )
+        print("score4 (-2*tr(sqrtm(matmul(sigma_r sigma_f))))  = ",score4) 
         score = score1 + score2 + score3 + score4
-    score = diff.dot(diff) + torch.trace(sigma_real) + torch.trace(sigma_fake) -2* torch.trace ( torch.real ( sqrtm( torch.matmul( sigma_real, sigma_fake)  ) ) )
+    score = mu_diff.dot(mu_diff) + torch.trace(sigma_real) + torch.trace(sigma_fake) -2* torch.trace ( torch.real ( sqrtm( torch.matmul( sigma_real, sigma_fake), method=method  ) ) )
     return score
 
-# %% ../nbs/03_fad_score.ipynb 12
+# %% ../nbs/03_fad_score.ipynb 16
 def main(): 
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('real_emb_path', help='Path of files of embeddings of real data', default='real_emb_clap/')
     parser.add_argument('fake_emb_path', help='Path of files of embeddings of fake data', default='fake_emb_clap/')
+    parser.add_argument('-d','--debug', action='store_true', help='Enable debugging')
+    parser.add_argument('-m','--method', default='maji', help='Method for sqrtm calculation: "maji" or "li" ')
+
     args = parser.parse_args()
-    score = calc_score( args )
+    score = calc_score( args.real_emb_path, args.fake_emb_path, method=args.method, debug=args.debug )
     print("FAD score = ",score.cpu().numpy())
 
-# %% ../nbs/03_fad_score.ipynb 13
+# %% ../nbs/03_fad_score.ipynb 17
 if __name__ == '__main__' and "get_ipython" not in dir():
     main()
```

### Comparing `fad_pytorch-0.0.2/fad_pytorch/pann.py` & `fad_pytorch-0.0.3/fad_pytorch/pann.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/05_pann.ipynb.
+
+# %% auto 0
+__all__ = ['LICENSE_KONG', 'init_layer', 'init_bn', 'ConvBlock', 'ConvBlock5x5', 'AttBlock', 'Cnn14', 'Cnn14_no_specaug',
+           'Cnn14_no_dropout', 'Cnn6', 'Cnn10', 'ResNet22', 'ResNet38', 'ResNet54', 'Cnn14_emb512', 'Cnn14_emb128',
+           'Cnn14_emb32', 'MobileNetV1', 'InvertedResidual', 'MobileNetV2', 'LeeNetConvBlock', 'LeeNet11',
+           'LeeNetConvBlock2', 'LeeNet24', 'DaiNetResBlock', 'DaiNet19', 'Res1dNet31', 'Res1dNet51', 'ConvPreWavBlock',
+           'Wavegram_Cnn14', 'Wavegram_Logmel_Cnn14', 'Wavegram_Logmel128_Cnn14', 'Cnn14_16k', 'Cnn14_8k',
+           'Cnn14_mixup_time_domain', 'Cnn14_mel32', 'Cnn14_mel128', 'Cnn14_DecisionLevelMax', 'Cnn14_DecisionLevelAvg',
+           'Cnn14_DecisionLevelAtt']
+
+# %% ../nbs/05_pann.ipynb 4
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+from torchlibrosa.stft import Spectrogram, LogmelFilterBank
+from torchlibrosa.augmentation import SpecAugmentation
+from .pann_pytorch_utils import do_mixup, interpolate, pad_framewise_output
+
+# %% ../nbs/05_pann.ipynb 5
 """
 From: https://github.com/qiuqiangkong/audioset_tagging_cnn/blob/d2f4b8c18eab44737fcc0de1248ae21eb43f6aa4/pytorch/models.py
 
 Copyright (c) 2018-2020 Qiuqiang Kong
 """
 
 LICENSE_KONG = """
@@ -23,24 +43,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE."""
 
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from torchlibrosa.stft import Spectrogram, LogmelFilterBank
-from torchlibrosa.augmentation import SpecAugmentation
-
-from .pann_pytorch_utils import do_mixup, interpolate, pad_framewise_output
- 
-
+# %% ../nbs/05_pann.ipynb 7
 def init_layer(layer):
     """Initialize a Linear or Convolutional layer. """
     nn.init.xavier_uniform_(layer.weight)
  
     if hasattr(layer, 'bias'):
         if layer.bias is not None:
             layer.bias.data.fill_(0.)
@@ -3339,8 +3350,8 @@
         # Get framewise output
         framewise_output = interpolate(segmentwise_output, self.interpolate_ratio)
         framewise_output = pad_framewise_output(framewise_output, frames_num)
 
         output_dict = {'framewise_output': framewise_output, 
             'clipwise_output': clipwise_output}
 
-        return output_dict
+        return output_dict
```

### Comparing `fad_pytorch-0.0.2/fad_pytorch/pann_pytorch_utils.py` & `fad_pytorch-0.0.3/fad_pytorch/pann_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.2/fad_pytorch/sqrtm.py` & `fad_pytorch-0.0.3/fad_pytorch/sqrtm.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
            'sqrt_newton_schulz_autograd', 'sqrt_newton_schulz', 'sqrtm']
 
 # %% ../nbs/04_sqrtm.ipynb 4
 import torch
 from torch.autograd import Function, Variable
 
 # %% ../nbs/04_sqrtm.ipynb 6
-use_li = False  # come back and turn this on if you want to see/use the full code
+use_li = True  # come back and turn this on if you want to see/use the full code
 
 if use_li:      # lighten the load of imports since we won't use li's in production
     import numpy as np
     import scipy.linalg
 
 # %% ../nbs/04_sqrtm.ipynb 7
 class MatrixSquareRoot_li(Function):
@@ -82,16 +82,16 @@
     normA = torch.sqrt(torch.sum(torch.sum(A * A, dim=1),dim=1))
     error = A - torch.bmm(sA, sA)
     error = torch.sqrt((error * error).sum(dim=1).sum(dim=1)) / normA
     return torch.mean(error)
 
 
 def sqrt_newton_schulz_autograd(A, 
-                                numIters=7, # 7 found experimentally by SHH, comparing w/ Li's method
-                               ):
+                                numIters=20, # found experimentally by SHH, comparing w/ Li's method
+                                calc_error=False,):
     """Modified from from https://people.cs.umass.edu/~smaji/projects/matrix-sqrt/
     "The drawback of the autograd approach [i.e., this approach] is that a naive implementation stores all the intermediate results. 
     Thus the memory overhead scales linearly with the number of iterations which is problematic for large matrices."
     """
     if len(A.data.shape) < 3: A = A.unsqueeze(0)
     batchSize, dim1, dim2 = A.data.shape
     assert dim1==dim2
@@ -105,21 +105,23 @@
 
     for i in range(numIters):
         T = 0.5*(3.0*I - Z.bmm(Y))
         Y = Y.bmm(T)
         Z = T.bmm(Z)
     
     sA = Y*torch.sqrt(normA).view(batchSize, 1, 1).expand_as(A)
-    error = compute_error(A, sA)
-    return sA, error
+    if calc_error:
+        error = compute_error(A, sA)
+        return sA, error
+    return sA
 
 
 def sqrt_newton_schulz(A,               # matrix to be sqrt-ified
-                       numIters=7,      # numIters=7 found via experimentation
-                       calc_error=True, # setting False disables Maji's error reporting
+                       numIters=20,      # numIters=7 found via experimentation
+                       calc_error=False, # setting False disables Maji's error reporting
                       ):
     """
     Sqrt of matrix via Newton-Schulz algorithm
     Modified from https://github.com/msubhransu/matrix-sqrt/blob/cc2289a3ed7042b8dbacd53ce8a34da1f814ed2f/matrix_sqrt.py#LL72C1-L87C19
     # Forward via Newton-Schulz iterations (non autograd version)
     # Seems to be slighlty faster and has much lower memory overhead
     
@@ -185,12 +187,17 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-# %% ../nbs/04_sqrtm.ipynb 26
-def sqrtm(A, numIters=7):
-    "wrapper function for matrix sqrt algorithm of choice: sqrt_newton_schulz. Also we'll turn off all gradients"
+# %% ../nbs/04_sqrtm.ipynb 27
+def sqrtm(A, method='maji', numIters=20):
+    "wrapper function for matrix sqrt algorithm of choice. Also we'll turn off all gradients"
     with torch.no_grad():
-        return sqrt_newton_schulz(A, numIters=numIters, calc_error=False).squeeze()  # get rid of any useless batch dimensions
+        if method=='maji':
+            return sqrt_newton_schulz(A, numIters=numIters, calc_error=False).squeeze()  # get rid of any useless batch dimensions
+        elif method=='li': 
+            return sqrtm_li(A)
+        else:
+            raise ValueError(f"Invalid method: {method}")
```

### Comparing `fad_pytorch-0.0.2/fad_pytorch.egg-info/PKG-INFO` & `fad_pytorch-0.0.3/fad_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fad-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Frechet Audio Distance evaluation in PyTorch
 Home-page: https://github.com/drscotthawley/fad_pytorch
 Author: Scott H. Hawley
 Author-email: scott.hawley@belmont.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fad_pytorch-0.0.2/fad_pytorch.egg-info/SOURCES.txt` & `fad_pytorch-0.0.3/fad_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.2/settings.ini` & `fad_pytorch-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fad_pytorch
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fad_pytorch
```

### Comparing `fad_pytorch-0.0.2/setup.py` & `fad_pytorch-0.0.3/setup.py`

 * *Files identical despite different names*

