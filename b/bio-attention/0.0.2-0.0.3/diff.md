# Comparing `tmp/bio-attention-0.0.2.tar.gz` & `tmp/bio-attention-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-attention-0.0.2.tar", last modified: Tue May 30 12:24:22 2023, max compression
+gzip compressed data, was "bio-attention-0.0.3.tar", last modified: Fri Jun  2 14:30:19 2023, max compression
```

## Comparing `bio-attention-0.0.2.tar` & `bio-attention-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.888790 bio-attention-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.880790 bio-attention-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.880790 bio-attention-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-30 12:24:11.000000 bio-attention-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-30 12:24:11.000000 bio-attention-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-30 12:24:11.000000 bio-attention-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-30 12:24:22.888790 bio-attention-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-30 12:24:11.000000 bio-attention-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.880790 bio-attention-0.0.2/bio_attention/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.888790 bio-attention-0.0.2/bio_attention/img/
--rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/img/2Dslidingwindow-attention.png
--rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/img/windowed_implementation.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21740 2023-05-30 12:24:11.000000 bio-attention-0.0.2/bio_attention/positional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:24:22.884790 bio-attention-0.0.2/bio_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-30 12:24:22.000000 bio-attention-0.0.2/bio_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:24:22.000000 bio-attention-0.0.2/bio_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:24:22.000000 bio-attention-0.0.2/bio_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 12:24:22.000000 bio-attention-0.0.2/bio_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 12:24:22.000000 bio-attention-0.0.2/bio_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-30 12:24:11.000000 bio-attention-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-30 12:24:22.888790 bio-attention-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.129676 bio-attention-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.125676 bio-attention-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.125676 bio-attention-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-02 14:30:11.000000 bio-attention-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-02 14:30:11.000000 bio-attention-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-02 14:30:11.000000 bio-attention-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-02 14:30:19.129676 bio-attention-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-02 14:30:11.000000 bio-attention-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.125676 bio-attention-0.0.3/bio_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15822 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.129676 bio-attention-0.0.3/bio_attention/img/
+-rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/img/2Dslidingwindow-attention.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/img/windowed_implementation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21699 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/positional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.125676 bio-attention-0.0.3/bio_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-02 14:30:19.000000 bio-attention-0.0.3/bio_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 14:30:19.000000 bio-attention-0.0.3/bio_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:30:19.000000 bio-attention-0.0.3/bio_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 14:30:19.000000 bio-attention-0.0.3/bio_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 14:30:19.000000 bio-attention-0.0.3/bio_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:30:11.000000 bio-attention-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-02 14:30:19.129676 bio-attention-0.0.3/setup.cfg
```

### Comparing `bio-attention-0.0.2/.github/workflows/publish.yml` & `bio-attention-0.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.2/.gitignore` & `bio-attention-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.2/LICENSE` & `bio-attention-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.2/bio_attention/attention.py` & `bio-attention-0.0.3/bio_attention/attention.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,48 +50,69 @@
 
         Returns
         -------
         _type_
             _description_
         """
         q_shape = q.shape
-        q, k, v = map(lambda t: rearrange(t, "b ... x n h -> (b ...) x n h").permute(0, 2, 1, 3), (q, k, v))
+        q, k, v = map(
+            lambda t: rearrange(t, "b ... x n h -> (b ...) x n h").permute(0, 2, 1, 3),
+            (q, k, v),
+        )
         if mask is not None:
             mask = rearrange(mask, "b ... n q k -> (b ...) n q k")
         if self.use_context_manager:
             with torch.backends.cuda.sdp_kernel(**self.context_manager):
-                return F.scaled_dot_product_attention(
-                    q,k,v,
+                return (
+                    F.scaled_dot_product_attention(
+                        q,
+                        k,
+                        v,
+                        dropout_p=(self.dropout if self.training else 0),
+                        attn_mask=mask,
+                        is_causal=causal,
+                    )
+                    .permute(0, 2, 1, 3)
+                    .view(*q_shape)
+                )
+        else:
+            return (
+                F.scaled_dot_product_attention(
+                    q,
+                    k,
+                    v,
                     dropout_p=(self.dropout if self.training else 0),
                     attn_mask=mask,
                     is_causal=causal,
-                ).permute(0, 2, 1, 3).view(*q_shape)
-        else:
-            return F.scaled_dot_product_attention(
-                q,k,v,
-                dropout_p=(self.dropout if self.training else 0),
-                attn_mask=mask,
-                is_causal=causal,
-            ).permute(0, 2, 1, 3).view(*q_shape)
+                )
+                .permute(0, 2, 1, 3)
+                .view(*q_shape)
+            )
 
 
 class RandomAttention(nn.Module):
-    def __init__(self, n_random_keys=64, dropout=0.2, materialize_full = False, **kwargs,):
+    def __init__(
+        self,
+        n_random_keys=64,
+        dropout=0.2,
+        materialize_full=False,
+        **kwargs,
+    ):
         super().__init__()
         if not materialize_full:
             self.softmax = nn.Softmax(dim=-2)
             self.dropout = nn.Dropout(dropout)
-            
+
             self.forward = self.forward_indexed
         else:
             self.dropout = dropout
             self.forward = self.forward_naive
         self.n = n_random_keys
 
-    def forward_indexed(self, q, k, v, mask = None, causal = False):
+    def forward_indexed(self, q, k, v, mask=None, causal=False):
         """random attention layer
 
         NOTE: causal attention will erase input masks
 
         Parameters
         ----------
         q : B, *, L1, NH, H
@@ -112,82 +133,106 @@
         """
         assert not (causal and (mask is not None))
 
         q_shape = q.shape
         q, k, v = map(lambda t: rearrange(t, "b ... x n h -> (b ...) x n h"), (q, k, v))
         if mask is not None:
             mask = rearrange(mask, "b ... n q k -> (b ...) n q k")
-        
+
         b, s2, nh, h = k.shape
         s1 = q.shape[1]
 
-        mask = torch.ones(b, nh, s1, s2, dtype=torch.bool).tril(diagonal=0) if causal else mask
+        mask = (
+            torch.ones(b, nh, s1, s2, dtype=torch.bool).tril(diagonal=0)
+            if causal
+            else mask
+        )
         if mask is not None:
-            mask = (~mask).float().masked_fill(~mask, -float('inf')) if mask.dtype==torch.bool else mask
+            mask = (
+                (~mask).float().masked_fill(~mask, -float("inf"))
+                if mask.dtype == torch.bool
+                else mask
+            )
             mask = mask.to(q)
 
         q = q * (h**-0.5)
 
         indices_select = torch.randint(0, s1, (b, s2, self.n)).to(q.device)
         indexer = torch.arange(b).view(b, 1, 1)
         if mask is not None:
             mask = mask.permute(0, 2, 3, 1)[
-                indexer,
-                torch.arange(s1)[None, :, None],
-                indices_select
-                ].permute(0, 3, 1, 2)
+                indexer, torch.arange(s1)[None, :, None], indices_select
+            ].permute(0, 3, 1, 2)
 
-        
         k = k[indexer, indices_select]
         v = v[indexer, indices_select]
 
-        A = einsum("b q n h, b q k n h -> b q k n", q, k) + (0 if mask is None else mask.permute(0, 2, 3, 1))
+        A = einsum("b q n h, b q k n h -> b q k n", q, k) + (
+            0 if mask is None else mask.permute(0, 2, 3, 1)
+        )
         A = self.softmax(A)
 
         A = self.dropout(A)
         z = einsum("b q k n, b q k n h -> b q n h", A, v)
 
         return z.view(*q_shape)
 
-    def forward_naive(self, q, k, v, mask = None, causal = False):
+    def forward_naive(self, q, k, v, mask=None, causal=False):
         """NOTE: Is incompatible with causal attention.
         NOTE: Is incompatible with input masks attention.
 
         Args:
             q (_type_): _description_
             k (_type_): _description_
             v (_type_): _description_
             mask (_type_, optional): _description_. Defaults to None.
             causal (bool, optional): _description_. Defaults to False.
 
         Returns:
             _type_: _description_
         """
         q_shape = q.shape
-        q, k, v = map(lambda t: rearrange(t, "b ... x n h -> (b ...) x n h").permute(0, 2, 1, 3), (q, k, v))
+        q, k, v = map(
+            lambda t: rearrange(t, "b ... x n h -> (b ...) x n h").permute(0, 2, 1, 3),
+            (q, k, v),
+        )
         if mask is not None:
             mask = rearrange(mask, "b ... n q k -> (b ...) n q k")
 
         b, nh, s2, h = k.shape
         s1 = q.shape[-2]
 
-        mask = (torch.rand(b, 1, s1, s2) < (self.n/s2)).expand(-1, nh, -1, -1).to(k.device)
+        mask = (
+            (torch.rand(b, 1, s1, s2) < (self.n / s2))
+            .expand(-1, nh, -1, -1)
+            .to(k.device)
+        )
 
-        return F.scaled_dot_product_attention(
+        return (
+            F.scaled_dot_product_attention(
                 q,
                 k,
                 v,
                 dropout_p=(self.dropout if self.training else 0),
                 attn_mask=mask,
                 is_causal=causal,
-            ).permute(0, 2, 1, 3).view(*q_shape)
+            )
+            .permute(0, 2, 1, 3)
+            .view(*q_shape)
+        )
 
 
 class WindowAttention(nn.Module):
-    def __init__(self, window = 5, dropout=0.1, materialize_full = False, **kwargs,):
+    def __init__(
+        self,
+        window=5,
+        dropout=0.1,
+        materialize_full=False,
+        **kwargs,
+    ):
         super().__init__()
         assert window % 2 == 1, "Window size should be an odd integer."
 
         self.w = int((window - 1) / 2)
 
         if not materialize_full:
             self.softmax = nn.Softmax(dim=-1)
@@ -201,15 +246,15 @@
             self.mask_k_left[:, : self.w] = True
             self.forward = self.forward_sliced
 
         else:
             self.dropout = dropout
             self.forward = self.forward_naive
 
-    def forward_sliced(self, q, k, v, mask= None, causal = False):
+    def forward_sliced(self, q, k, v, mask=None, causal=False):
         """windowed attention layer
 
         Parameters
         ----------
         q : B, L1, NH, H
             queries
         k : B, L2, NH, H
@@ -260,70 +305,90 @@
                 + [mask_k_right]
             )
         else:
             mask = torch.logical_or(
                 self.mask_k_left.to(A.device), mask_k_right
             ).unsqueeze(0)
         if causal:
-            mask = ~(~mask).tril(diagonal = self.w)
+            mask = ~(~mask).tril(diagonal=self.w)
 
         A.masked_fill_(mask, mask_value)
         A = self.softmax(A)
         A = self.dropout(A)
 
         z = einsum("b n c q k, b c n h k -> b n c q h", A, v)
         z = z.view(b, nh, -1, h)[:, :, :s].permute(0, 2, 1, 3).view(*q_shape)
 
         return z
 
-    def forward_naive(self, q, k, v, mask=None, causal = False):
+    def forward_naive(self, q, k, v, mask=None, causal=False):
         assert mask is None
         assert k.shape[-3] == q.shape[-3], "q and k should have same input length."
 
         q_shape = q.shape
-        q, k, v = map(lambda t: rearrange(t, "b ... x n h -> (b ...) x n h").permute(0, 2, 1, 3), (q, k, v))
+        q, k, v = map(
+            lambda t: rearrange(t, "b ... x n h -> (b ...) x n h").permute(0, 2, 1, 3),
+            (q, k, v),
+        )
 
         b, nh, s2, h = k.shape
         s1 = q.shape[-2]
 
-        u = torch.triu(torch.full((s1, s2), True), diagonal = -self.w)
-        mask = torch.logical_and(u, torch.flip(u, [0, 1])).expand(b, nh, -1, -1).to(k.device)
+        u = torch.triu(torch.full((s1, s2), True), diagonal=-self.w)
+        mask = (
+            torch.logical_and(u, torch.flip(u, [0, 1]))
+            .expand(b, nh, -1, -1)
+            .to(k.device)
+        )
         if causal:
             mask = torch.tril(mask)
-        return F.scaled_dot_product_attention(
-                q,k,v,
+        return (
+            F.scaled_dot_product_attention(
+                q,
+                k,
+                v,
                 dropout_p=(self.dropout if self.training else 0),
                 attn_mask=mask,
                 is_causal=False,
-            ).permute(0, 2, 1, 3).view(*q_shape)
+            )
+            .permute(0, 2, 1, 3)
+            .view(*q_shape)
+        )
+
 
 class AttnLayer(nn.Module):
     def __init__(self, dim, attn, nh=4, plugin=None):
         super().__init__()
         assert dim % nh == 0, "dim should be divisible by number of heads"
 
         self.lin = nn.Linear(dim, 3 * dim)
         self.attn = attn
         self.nh = nh
 
         self.plugin = plugin if plugin is not None else positional.Base()
 
     def forward(self, x, pos=None, mask=None, causal=False, **mod_kwargs):
-        x = self.plugin.mod_x(x, pos = pos, **mod_kwargs)
+        x = self.plugin.mod_x(x, pos=pos, **mod_kwargs)
         b, l, h = (x.size(0), x.size(-2), x.size(-1))
         q, k, v = torch.split(self.lin(x), h, dim=-1)
-        q, k, v = map(lambda t: rearrange(t, "... (n h) -> ... n h", n = self.nh), (q, k, v))
+        q, k, v = map(
+            lambda t: rearrange(t, "... (n h) -> ... n h", n=self.nh), (q, k, v)
+        )
 
         mod_kwargs |= {"pos_q_k": pos}
 
         q, k, v = self.plugin.mod_qkv(q, k, v, **mod_kwargs)
 
         mask = self.plugin.mod_mask(mask, q, k, v, **mod_kwargs)
 
-        return rearrange(self.attn(q, k, v, mask=mask, causal=causal), "... n h -> ... (n h)", n = self.nh)
+        return rearrange(
+            self.attn(q, k, v, mask=mask, causal=causal),
+            "... n h -> ... (n h)",
+            n=self.nh,
+        )
 
 
 class Residual(nn.Module):
     def __init__(self, fn):
         super().__init__()
         self.fn = fn
 
@@ -367,45 +432,45 @@
                 nn.LayerNorm(dim),
                 project_in,
                 nn.Dropout(dropout),
                 nn.Linear(4 * dim, dim),
             )
         )
 
-    def forward(self, x, pos = None, mask = None, causal = False, **mod_kwargs):
+    def forward(self, x, pos=None, mask=None, causal=False, **mod_kwargs):
         x = self.attn(self.norm(x), pos=pos, mask=mask, causal=causal, **mod_kwargs) + x
         return self.ff(x)
 
 
 class TransformerEncoder(nn.Module):
     def __init__(
         self,
         depth,
         dim,
         nh,
-        attentiontype = "vanilla",
-        attention_args = {},
+        attentiontype="vanilla",
+        attention_args={},
         plugintype="none",
-        plugin_args = {},
-        only_apply_plugin_at_first = False,
+        plugin_args={},
+        only_apply_plugin_at_first=False,
         dropout=0.2,
         glu_ff=True,
         activation="swish",
     ):
         super().__init__()
 
         assert attentiontype in ["vanilla", "random", "window"]
-        
+
         if attentiontype == "vanilla":
             attn_op = Attention(**attention_args)
         elif attentiontype == "random":
             attn_op = RandomAttention(**attention_args)
         elif attentiontype == "window":
             attn_op = WindowAttention(**attention_args)
-        
+
         if plugintype == "none":
             plugin = positional.Base()
         elif plugintype == "sinusoidal":
             plugin = positional.Sinusoidal(**plugin_args)
         elif plugintype == "learned":
             plugin = positional.LearnedVocab(**plugin_args)
         elif plugintype == "learnedcont":
@@ -416,21 +481,51 @@
             plugin = positional.ALiBi(**plugin_args)
         elif plugintype == "DPB":
             plugin = positional.DPB(**plugin_args)
         elif plugintype == "XL":
             plugin = positional.XL(**plugin_args)
 
         layers = []
-        layers.append(TransformerLayer(attn_op, dim, nh, plugin=plugin, dropout=dropout, glu_ff=glu_ff, activation=activation))
+        layers.append(
+            TransformerLayer(
+                attn_op,
+                dim,
+                nh,
+                plugin=plugin,
+                dropout=dropout,
+                glu_ff=glu_ff,
+                activation=activation,
+            )
+        )
         if only_apply_plugin_at_first:
-            for _ in range(depth-1):
-                layers.append(TransformerLayer(attn_op, dim, nh, plugin=plugin, dropout=dropout, glu_ff=glu_ff, activation=activation))
+            for _ in range(depth - 1):
+                layers.append(
+                    TransformerLayer(
+                        attn_op,
+                        dim,
+                        nh,
+                        plugin=plugin,
+                        dropout=dropout,
+                        glu_ff=glu_ff,
+                        activation=activation,
+                    )
+                )
         else:
-            for _ in range(depth-1):
-                layers.append(TransformerLayer(attn_op, dim, nh, plugin=None, dropout=dropout, glu_ff=glu_ff, activation=activation))
+            for _ in range(depth - 1):
+                layers.append(
+                    TransformerLayer(
+                        attn_op,
+                        dim,
+                        nh,
+                        plugin=None,
+                        dropout=dropout,
+                        glu_ff=glu_ff,
+                        activation=activation,
+                    )
+                )
 
         self.layers = nn.ModuleList(layers)
 
-    def forward(self, x, pos = None, mask = None, causal = False, **mod_kwargs):
+    def forward(self, x, pos=None, mask=None, causal=False, **mod_kwargs):
         for layer in self.layers:
-            x = layer(x, pos = pos, mask = mask, causal = causal, **mod_kwargs)
-        return x
+            x = layer(x, pos=pos, mask=mask, causal=causal, **mod_kwargs)
+        return x
```

### Comparing `bio-attention-0.0.2/bio_attention/embed.py` & `bio-attention-0.0.3/bio_attention/embed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch
 from torch import nn
 
+
 class DiscreteEmbedding(nn.Module):
     def __init__(
         self,
         num_embeddings,
         embedding_dim,
         cls=False,
         cls_axis=-2,
@@ -44,16 +45,16 @@
         return x
 
 
 class ContinuousEmbedding(nn.Module):
     def __init__(
         self,
         embedding_dim,
-        depth = 1,
-        norm = False,
+        depth=1,
+        norm=False,
         cls=False,
         cls_axis=-2,
         init_cls_as_bias=False,
         init_mask_as_bias=False,
         init_cls_as_mask=False,
     ):
         """Embedding module for continuous data. Uses `nn.Linear` with added support for masking tokens cls tokens.
@@ -78,15 +79,15 @@
         for _ in range(depth - 1):
             layers.append(nn.SiLU())
             layers.append(nn.Linear(embedding_dim, embedding_dim))
             layers.append(nn.LayerNorm(embedding_dim) if norm else nn.Identity())
         self.embedder = nn.Sequential(*layers)
 
         with torch.no_grad():
-            bias = self.embedder(torch.tensor([[0.]])).unsqueeze(0)
+            bias = self.embedder(torch.tensor([[0.0]])).unsqueeze(0)
 
         if init_mask_as_bias:
             self.mask_embedding = nn.Parameter(bias)
         else:
             self.mask_embedding = nn.Parameter(torch.empty(embedding_dim))
             nn.init.uniform_(self.mask_embedding, -1, 1)
```

### Comparing `bio-attention-0.0.2/bio_attention/img/2Dslidingwindow-attention.png` & `bio-attention-0.0.3/bio_attention/img/2Dslidingwindow-attention.png`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.2/bio_attention/img/windowed_implementation.svg` & `bio-attention-0.0.3/bio_attention/img/windowed_implementation.svg`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.2/bio_attention/positional.py` & `bio-attention-0.0.3/bio_attention/positional.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import torch
 import torch.nn as nn
 from einops import rearrange, repeat, einsum
 import math
 
+
 class Base(nn.Module):
     def __init__(self, divide=1.0, learned=False):
         super().__init__()
         self.learned = learned
         if not learned:
             self.div = divide
         else:
             self.div = nn.Parameter(torch.tensor(math.log(divide)))
 
         self.forward = self.mod_x
 
     def mod_x(self, x, pos=None, **kwargs):
         return x
-    
+
     def mod_qkv(self, q, k, v, pos=None, **kwargs):
         return q, k, v
 
     def mod_mask(self, mask, q, k, v, pos=None, **kwargs):
         return mask
 
     def apply_pos_division(self, x):
         if not self.learned:
             return x / self.div
         else:
             return x / self.div.exp().clamp(min=1e-8)
 
     @staticmethod
     def default_pos_x(x):
-        return (
-            torch.arange(x.size(-2), device = x.device).expand(*x.shape[:-1])
-        )
+        return torch.arange(x.size(-2), device=x.device).expand(*x.shape[:-1])
+
 
 class Sinusoidal(Base):
     def __init__(self, dim, divide=1.0, learned_div=False):
         """Sinusoidal positional embedding as in Vaswani et al. (2017)
         Supports specifying positions, masking, and division of positional range.
 
         Args:
@@ -45,15 +45,14 @@
             divide (float, optional): divide positions by this factor, useful for large (or small) numerical ranges. Defaults to 1.0.
             learned_div (bool, optional): Whether to learn the division factor. Defaults to False.
         """
         super().__init__(divide=divide, learned=learned_div)
         self.dim = dim
         inv_freq = 1 / (10000 ** (torch.arange(0.0, dim, 2) / dim))
         self.register_buffer("inv_freq", inv_freq)
-        
 
     def mod_x(self, x, pos=None, mask=None, **kwargs):
         """
         Args:
             x (torch.tensor): (B,*,L,H)
             pos (torch.tensor, optional): (B,*,L). Defaults to None for computing positions from 0 to L-1 (only possible for 1-D sequence inputs x B,L,H).
             mask (torch.tensor, optional): (B,*,L). A boolean mask to indicate where positions should not have positional encodings added.
@@ -74,14 +73,15 @@
             .to(x.dtype)
         )
         if mask is not None:
             pos_emb = pos_emb * mask.unsqueeze(-1)
 
         return x + pos_emb
 
+
 class LearnedVocab(Base):
     def __init__(self, dim, max_seq_len):
         """Learned vocab as in Devlin et al. (2018)
         Supports specifying positions and masking.
         Only works for discrete positional indices.
 
         Args:
@@ -107,17 +107,18 @@
         assert shp[-1] == self.emb.embedding_dim
         pos = self.default_pos_x(x).long() if pos is None else pos
 
         pos_emb = self.emb(pos)
         if mask is not None:
             pos_emb = pos_emb * mask.unsqueeze(-1)
         return x + pos_emb
-    
+
+
 class LearnedContinuous(Base):
-    def __init__(self, dim, depth=3, norm = False, divide=1.0, learned_div=False):
+    def __init__(self, dim, depth=3, norm=False, divide=1.0, learned_div=False):
         """Learned embeddings with a continuity between absolute positional indices, as learned by a series of linear layers.
         Supports specifying positions, masking, and division of positional range.
 
         Args:
             dim (int): Hidden size of the embeddings
             depth (int, optional): number of hidden layers in the positional embedding network. Defaults to 3
             norm (bool, optional): Whether to use layernorms in the MLP. Defaults to False
@@ -161,14 +162,15 @@
         for layer in self.mlp:
             pos_emb = layer(pos_emb)
 
         if mask is not None:
             pos_emb = pos_emb * mask.unsqueeze(-1)
         return x + pos_emb
 
+
 class Rotary(Base):
     def __init__(self, head_dim, n_dims=None, divide=1.0, learned_div=False):
         """Rotary embedding as in RoFormer / RoPE
         Supports specifying positions and division of positional range.
 
         Args:
             head_dim (int): Hidden dimensions per head
@@ -191,15 +193,15 @@
         self,
         q,
         k,
         v,
         pos_q_k=None,
         pos_q=None,
         pos_k=None,
-        self_attn_mode = True,
+        self_attn_mode=True,
         **kwargs,
     ):
         """
         Args:
             q (torch.tensor): (B,*,NH,H)
             k (torch.tensor): (B,*,NH,H)
             v (torch.tensor): (B,*,NH,H)
@@ -230,15 +232,17 @@
 
             q = q * cos_q.to(q) + self.rotate_every_two(q) * sin_q.to(q)
             k = k * cos_k.to(k) + self.rotate_every_two(k) * sin_k.to(k)
 
         return q, k, v
 
     def get_rotations(self, pos):
-        mthetas = self.apply_pos_division(pos).to(self.thetas)[..., None] * self.thetas # B, *, h
+        mthetas = (
+            self.apply_pos_division(pos).to(self.thetas)[..., None] * self.thetas
+        )  # B, *, h
         sin, cos = map(
             lambda t: repeat(t, "b ... h  -> b ... (h j)", j=2),
             (mthetas.sin(), mthetas.cos()),
         )
         sin, cos = map(lambda t: t.unsqueeze(-2), (sin, cos))
         return sin, cos
 
@@ -246,14 +250,15 @@
     def rotate_every_two(x):
         x = x.clone()
         x = rearrange(x, "... (d j) -> ... d j", j=2)
         x1, x2 = x.unbind(dim=-1)
         x = torch.stack((-x2, x1), dim=-1)
         return rearrange(x, "... d j -> ... (d j)")
 
+
 class ALiBi(Base):
     def __init__(
         self, n_heads, use_n_heads=None, asymmetric=False, divide=1.0, learned_div=False
     ):
         """Attention with linear biases as in Press et al. 2022
         Supports specifying positions, division of positional range, using only a fraction of the heads, and asymmetric bias for bidirectional cases.
 
@@ -284,15 +289,15 @@
             slopes = [slopes[(i // 2) * 2] for i in range((len(slopes)))]
             slopes = torch.tensor(slopes + [0] * (n_heads - use_n_heads))
         slopes = rearrange(slopes, "h -> h 1 1")
         self.register_buffer("slopes", slopes)
 
         self.div = divide
 
-    def mod_mask(self, mask, q, k, v, pos_q_k = None, pos_q=None, pos_k=None, **kwargs):
+    def mod_mask(self, mask, q, k, v, pos_q_k=None, pos_q=None, pos_k=None, **kwargs):
         """
         Args:
             mask (torch.tensor): B, *, NH, L1, L2, optional, eg B, NH, L1, L2, or for multi-dim: B, S, NH, L1, L2
             q (torch.tensor): (B,*,NH,H)
             k (torch.tensor): (B,*,NH,H)
             v (torch.tensor): (B,*,NH,H)
             pos_q_k (torch.tensor, optional): (B, *) eg (B, L). Positions of q and k in self attention mode. Requires L1 = L2.
@@ -306,15 +311,15 @@
             **kwargs: ignored. Kept for compatibility.
         Returns:
             mask (torch.tensor): (B, *, NH, L1, L2)
         """
 
         if pos_q_k is not None:
             pos_q = pos_k = pos_q_k
-        
+
         elif (pos_q is None) and (pos_k is None):
             pos_q = self.default_pos_x(q[..., 0, :]) if pos_q is None else pos_q
             pos_k = self.default_pos_x(k[..., 0, :]) if pos_k is None else pos_k
 
         relative_pos = pos_q[..., :, None] - pos_k[..., None, :]
         bias = self.apply_pos_division(relative_pos.unsqueeze(-3) * self.slopes)
 
@@ -344,16 +349,19 @@
 
     @staticmethod
     def asymmetric_bias(bias):
         bias[:, ::2][bias[:, ::2] > 0] = torch.finfo(bias.dtype).max
         bias[:, 1::2][bias[:, 1::2] < 0] = torch.finfo(bias.dtype).max
         return bias
 
+
 class DPB(Base):
-    def __init__(self, dim, n_heads, depth=3, norm=False, divide=1.0, learned_div=False):
+    def __init__(
+        self, dim, n_heads, depth=3, norm=False, divide=1.0, learned_div=False
+    ):
         """Dynamic positional bias.
         Computes a bias to every element of the attention matrix based on their relative position via a parameterized MLP
         Described in https://arxiv.org/abs/2108.00154, https://arxiv.org/abs/2111.09883,
         https://github.com/lucidrains/x-transformers#dynamic-positional-bias
         Supports specifying positions and division of positional range
 
 
@@ -384,15 +392,15 @@
                 )
             )
 
         self.mlp.append(nn.Linear(dim, n_heads))
 
         self.div = divide
 
-    def mod_mask(self, mask, q, k, v, pos_q_k = None, pos_q=None, pos_k=None, **kwargs):
+    def mod_mask(self, mask, q, k, v, pos_q_k=None, pos_q=None, pos_k=None, **kwargs):
         """
         Args:
             mask (torch.tensor): B, *, NH, L1, L2, optional, eg B, NH, L1, L2, or for multi-dim: B, S, NH, L1, L2
             q (torch.tensor): (B,*,NH,H)
             k (torch.tensor): (B,*,NH,H)
             v (torch.tensor): (B,*,NH,H)
             pos_q_k (torch.tensor, optional): (B, *). Positions of q and k in self attention mode. Requires L1 = L2.
@@ -417,14 +425,15 @@
 
         for layer in self.mlp:
             bias = layer(bias)
         bias = bias.transpose(-1, -2).transpose(-2, -3).to(q)
 
         return (0 if mask is None else mask) - bias
 
+
 class XL(Base):
     def __init__(self, dim, n_heads, divide=1, learned_div=False):
         """Relative positional biases as in Transformer-XL (Dai et al 2019)
         Supports specifying positions and division of positional range
 
         Args:
             dim (int): number of hidden of x (total, not per head)
@@ -453,23 +462,23 @@
             k (torch.tensor): (B,*,NH,H)
             v (torch.tensor): (B,*,NH,H)
         Returns:
             q, k, v (all torch.tensor)
         """
         return q + self.bias_r_w, k, v
 
-    def mod_mask(self, mask, q, k, v, pos_q_k = None, pos_q=None, pos_k=None, **kwargs):
+    def mod_mask(self, mask, q, k, v, pos_q_k=None, pos_q=None, pos_k=None, **kwargs):
         """
         Args:
             mask (torch.tensor): B, *, NH, L1, L2, optional, eg B, NH, L1, L2, or for multi-dim: B, S, NH, L1, L2
             q (torch.tensor): (B,*,NH,H)
             k (torch.tensor): (B,*,NH,H)
             v (torch.tensor): (B,*,NH,H)
             pos_q_k (torch.tensor, optional): (B, *). Positions of q and k in self attention mode. Requires L1 = L2.
-                Defaults to None for computing positions from 0 to L-1. 
+                Defaults to None for computing positions from 0 to L-1.
             pos_q (torch.tensor, optional): (B, *). Positions of q in cross attention mode.
                 Defaults to None for computing positions from 0 to L1-1
             pos_k (torch.tensor, optional): (B, *). Positions of k in cross attention mode.
                 Defaults to None for computing positions from 0 to L2-1
             **kwargs: ignored. Kept for compatibility.
         Returns:
             mask (torch.tensor): (B, *, NH, L1, L2)
@@ -480,27 +489,25 @@
             pos_q = self.default_pos_x(q[..., 0, :]) if pos_q is None else pos_q
             pos_k = self.default_pos_x(k[..., 0, :]) if pos_k is None else pos_k
 
         relative_pos = (pos_q[..., :, None] - pos_k[..., None, :]).to(
             self.inv_freq.dtype
         )
 
-        sinusoid_inp = self.apply_pos_division(
-            relative_pos[..., None] * self.inv_freq
-        )
+        sinusoid_inp = self.apply_pos_division(relative_pos[..., None] * self.inv_freq)
         pos_emb = torch.stack((sinusoid_inp.sin(), sinusoid_inp.cos()), dim=-1)
-        
+
         pos_emb = rearrange(pos_emb, "... d j -> ... (d j)")
 
         r = rearrange(
             self.embed_lin(pos_emb),
             "... (nh h) -> ... nh h",
             nh=self.n_heads,
             h=q.shape[-1],
         )
         q_r = q + self.bias_r_w
         BD = einsum(q_r, r, "... q n h, ... q k n h -> ... n q k")
         return (0 if mask is None else mask) + BD
 
     def _init_bias(self, bias):
-        bound = 1/bias.size(1)**0.5
+        bound = 1 / bias.size(1) ** 0.5
         return nn.init.uniform_(bias, -bound, bound)
```

