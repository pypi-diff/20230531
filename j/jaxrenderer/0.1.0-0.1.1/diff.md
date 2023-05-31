# Comparing `tmp/jaxrenderer-0.1.0.tar.gz` & `tmp/jaxrenderer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrenderer-0.1.0.tar", max compression
+gzip compressed data, was "jaxrenderer-0.1.1.tar", max compression
```

## Comparing `jaxrenderer-0.1.0.tar` & `jaxrenderer-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11367 2023-05-29 20:54:00.387848 jaxrenderer-0.1.0/LICENSE
--rw-r--r--   0        0        0     1700 2023-05-29 20:54:00.387848 jaxrenderer-0.1.0/README.md
--rw-r--r--   0        0        0     1541 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4851 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/README.md
--rw-r--r--   0        0        0      360 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/__init__.py
--rw-r--r--   0        0        0    30966 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/geometry.py
--rw-r--r--   0        0        0     9697 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/model.py
--rw-r--r--   0        0        0    11913 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/pipeline.py
--rw-r--r--   0        0        0    15537 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/renderer.py
--rw-r--r--   0        0        0     8615 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/scene.py
--rw-r--r--   0        0        0    10102 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shader.py
--rw-r--r--   0        0        0     4600 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/README.md
--rw-r--r--   0        0        0     1256 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/depth.py
--rw-r--r--   0        0        0     3252 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/gouraud.py
--rw-r--r--   0        0        0     4804 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/gouraud_texture.py
--rw-r--r--   0        0        0     5079 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/phong.py
--rw-r--r--   0        0        0     9571 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/phong_darboux.py
--rw-r--r--   0        0        0     7926 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/phong_reflection.py
--rw-r--r--   0        0        0     9650 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/phong_reflection_shadow.py
--rw-r--r--   0        0        0     4166 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shadow.py
--rw-r--r--   0        0        0    71549 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shapes/capsule.py
--rw-r--r--   0        0        0     3574 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shapes/cube.py
--rw-r--r--   0        0        0     3270 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/types.py
--rw-r--r--   0        0        0     2531 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/utils.py
--rw-r--r--   0        0        0      833 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/value_checker.py
--rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 jaxrenderer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11367 2023-05-31 09:43:25.069668 jaxrenderer-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1700 2023-05-31 09:43:25.069668 jaxrenderer-0.1.1/README.md
+-rw-r--r--   0        0        0     3019 2023-05-31 09:43:25.069668 jaxrenderer-0.1.1/changelog.md
+-rw-r--r--   0        0        0     1541 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4851 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/README.md
+-rw-r--r--   0        0        0      459 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/__init__.py
+-rw-r--r--   0        0        0    33807 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/geometry.py
+-rw-r--r--   0        0        0    14829 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/model.py
+-rw-r--r--   0        0        0    11913 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/pipeline.py
+-rw-r--r--   0        0        0    13303 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/renderer.py
+-rw-r--r--   0        0        0     9726 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/scene.py
+-rw-r--r--   0        0        0    10102 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shader.py
+-rw-r--r--   0        0        0     4600 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/README.md
+-rw-r--r--   0        0        0     1256 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/depth.py
+-rw-r--r--   0        0        0     3252 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/gouraud.py
+-rw-r--r--   0        0        0     4804 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/gouraud_texture.py
+-rw-r--r--   0        0        0     5079 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/phong.py
+-rw-r--r--   0        0        0     9571 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/phong_darboux.py
+-rw-r--r--   0        0        0     7926 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/phong_reflection.py
+-rw-r--r--   0        0        0     9650 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/phong_reflection_shadow.py
+-rw-r--r--   0        0        0     4166 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shadow.py
+-rw-r--r--   0        0        0    71549 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shapes/capsule.py
+-rw-r--r--   0        0        0     3574 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shapes/cube.py
+-rw-r--r--   0        0        0     3270 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/types.py
+-rw-r--r--   0        0        0     3074 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/utils.py
+-rw-r--r--   0        0        0      833 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/value_checker.py
+-rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 jaxrenderer-0.1.1/PKG-INFO
```

### Comparing `jaxrenderer-0.1.0/LICENSE` & `jaxrenderer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/README.md` & `jaxrenderer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/pyproject.toml` & `jaxrenderer-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaxrenderer"
-version = "0.1.0"
+version = "0.1.1"
 description = "Jax implementation of rasterizer renderer."
 authors = ["Joey Teng <joey.teng.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JoeyTeng/jaxrenderer"
 repository = "https://github.com/JoeyTeng/jaxrenderer"
 classifiers = [
```

### Comparing `jaxrenderer-0.1.0/renderer/README.md` & `jaxrenderer-0.1.1/renderer/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/geometry.py` & `jaxrenderer-0.1.1/renderer/geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import enum
 from functools import partial
-from typing import Any, NamedTuple, Optional
+from typing import Any, NamedTuple, Optional, Union
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Float, Integer, Num, jaxtyped
 
 from .types import Triangle2Df, Vec2f, Vec3f, Vec4f
@@ -820,14 +820,102 @@
 @jax.jit
 def compute_normals(batch_verts: Float[Array, "b 3 3"]) -> Float[Array, "b 3"]:
     return jax.vmap(compute_normal)(batch_verts)
 
 
 @jaxtyped
 @jax.jit
+def quaternion(
+    rotation_axis: Union[Vec3f, tuple[float, float, float]],
+    rotation_angle: Union[Float[Array, ""], float],
+) -> Vec4f:
+    """Generate a quaternion rotation from a rotation axis and angle.
+
+    The rotation axis is normalised internally. The angle is specified in
+    degrees (NOT radian). The rotation is clockwise.
+    """
+    axis = normalise(jnp.asarray(rotation_axis))
+    angle = jnp.radians(jnp.asarray(rotation_angle))
+    assert isinstance(axis, Vec3f), f"{rotation_axis}"
+    assert isinstance(angle, Float[Array, ""]), f"{rotation_angle}"
+
+    quaternion: Vec4f = (
+        jnp.zeros(4)  #
+        .at[:3].set(axis * jnp.sin(angle / 2))  #
+        .at[3].set(jnp.cos(angle / 2))  #
+    )
+
+    return quaternion
+
+
+@jaxtyped
+@jax.jit
+def quaternion_mul(quatA: Vec4f, quatB: Vec4f) -> Vec4f:
+    """Multiply two quaternion rotations, as to composite them.
+
+    Noticed that all quaternions here are in order of (x, y, z, w), thus
+    shuffles are used here to convert from (w, x, y, z) to (x, y, z, w).
+
+    References:
+      - [Quaternion multiplication](https://www.mathworks.com/help/nav/ref/quaternion.mtimes.html)
+    """
+    assert isinstance(quatA, Vec4f)
+    assert isinstance(quatB, Vec4f)
+
+    with jax.ensure_compile_time_eval():
+        shuffle = jnp.array((3, 0, 1, 2))
+        idx103 = jnp.array((1, 0, 3))
+        idx230 = jnp.array((2, 3, 0))
+        idx013 = jnp.array((0, 1, 3))
+        idx320 = jnp.array((3, 2, 0))
+
+    quatA = quatA[shuffle]
+    quatB = quatB[shuffle]
+
+    return jnp.array((
+        quatA[0] * quatB[0] - quatA[1:] @ quatB[1:],
+        quatA[:3] @ quatB[idx103] - quatA[3] * quatB[2],
+        quatA[idx230] @ quatB[:3] - quatA[1] * quatB[3],
+        quatA[idx013] @ quatB[idx320] - quatA[2] * quatB[1],
+    ))[shuffle]
+
+
+@jaxtyped
+@jax.jit
+def rotation_matrix(
+    rotation_axis: Union[Vec3f, tuple[float, float, float]],
+    rotation_angle: Union[Float[Array, ""], float],
+) -> Float[Array, "3 3"]:
+    """Generate a rotation matrix from a rotation axis and angle.
+
+    The rotation axis is normalised internally. The angle is specified in
+    degrees (NOT radian). The rotation is clockwise.
+
+    References:
+      - [glRotated](https://registry.khronos.org/OpenGL-Refpages/gl2.1/xhtml/glRotate.xml)
+    """
+    axis = normalise(jnp.asarray(rotation_axis))
+    angle = jnp.radians(jnp.asarray(rotation_angle))
+    assert isinstance(axis, Vec3f), f"{rotation_axis}"
+    assert isinstance(angle, Float[Array, ""]), f"{rotation_angle}"
+
+    s = jnp.sin(angle)
+    c = jnp.cos(angle)
+
+    rotation_matrix: Float[Array, "3 3"] = (
+        jnp.identity(3) * c  # +c at main diagonal
+        - jnp.sin(angle) * jnp.cross(axis, jnp.identity(3))  # second term
+        + (1 - c) * jnp.outer(axis, axis)  # first term
+    )
+
+    return rotation_matrix
+
+
+@jaxtyped
+@jax.jit
 def transform_matrix_from_rotation(rotation: Vec4f) -> Float[Array, "3 3"]:
     """Generate a transform matrix from a quaternion rotation.
 
     Supports non-unit rotation.
 
     References:
           - [Quaternions and spatial rotation#Quaternion-derived rotation matrix](https://en.wikipedia.org/wiki/Quaternions_and_spatial_rotation#Quaternion-derived_rotation_matrix)
```

### Comparing `jaxrenderer-0.1.0/renderer/pipeline.py` & `jaxrenderer-0.1.1/renderer/pipeline.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/renderer.py` & `jaxrenderer-0.1.1/renderer/renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from functools import partial
-from typing import Any, NamedTuple, Optional, Union
+from typing import NamedTuple, Optional, Sequence, Union
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
-from jaxtyping import Array, Bool, Float, Integer, Num, jaxtyped
+from jaxtyping import Array, Bool, Integer, Num, jaxtyped
 
-from .geometry import Camera, View, Projection, Viewport, normalise
-from .model import MergedModel, ModelMatrix, ModelObject
+from .geometry import Camera, Projection, View, Viewport, normalise
+from .model import MergedModel, ModelObject, merge_objects
 from .pipeline import render
 from .shaders.phong_reflection import (PhongReflectionTextureExtraInput,
                                        PhongReflectionTextureShader)
 from .shaders.phong_reflection_shadow import (
     PhongReflectionShadowTextureExtraInput, PhongReflectionShadowTextureShader)
 from .shadow import Shadow
 from .types import (Buffers, Canvas, Colour, DtypeInfo, LightSource, Vec3f,
-                    Vertices, ZBuffer)
+                    ZBuffer)
 
 DoubleSidedFaces = Bool[Array, "faces"]
 """Whether to render both sides of each face (triangle primitive)."""
-ObjectsT = Union[list[ModelObject], tuple[ModelObject, ...]]
-"""A list or tuple of model objects. TODO: Change to `PyTree[ModelObject]`."""
 
 
 class CameraParameters(NamedTuple):
     """Parameters for rendering from camera.
 
     Default values come from [erwincoumans/tinyrenderer::TinyRendererCamera](https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/python/pytinyrenderer.cc#L56)
     """
@@ -38,19 +36,19 @@
     """near clipping plane."""
     far: float = 1000.
     """far clipping plane."""
     hfov: float = 58.
     """horizontal field of view, in degrees."""
     vfov: float = 45.
     """vertical field of view, in degrees."""
-    position: Vec3f = jnp.ones(3)
+    position: Union[Vec3f, tuple[float, float, float]] = jnp.ones(3)
     """position of the camera in world space."""
-    target: Vec3f = jnp.zeros(3)
+    target: Union[Vec3f, tuple[float, float, float]] = jnp.zeros(3)
     """target of the camera."""
-    up: Vec3f = jnp.array((0., 0., 1.))
+    up: Union[Vec3f, tuple[float, float, float]] = jnp.array((0., 0., 1.))
     """up direction of the camera."""
 
 
 class LightParameters(NamedTuple):
     """Parameters for directional light in rendering.
 
     Default values come from [erwincoumans/tinyrenderer::TinyRenderLight](https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/python/pytinyrenderer.cc#L74).
@@ -97,139 +95,26 @@
 
 
 class Renderer:
 
     @staticmethod
     @jaxtyped
     @partial(jax.jit, inline=True)
-    def merge_objects(objects: ObjectsT) -> MergedModel:
-        """Merge objects into a single model.
-
-        Parameters:
-          - objects: a list of objects to merge.
-
-        Returns: A model containing the merged objects into one single mesh.
-        """
-        with jax.ensure_compile_time_eval():
-            models = [obj.model for obj in objects]
-
-            # broadcasted per vertex info
-            counts: list[int] = [len(m.verts) for m in models]
-
-            map_indices: Integer[Array, "vertices"]
-            map_indices = MergedModel.generate_object_vert_info(
-                counts,
-                list(range(len(models))),
-            )
-            assert isinstance(map_indices, Integer[Array, "vertices"])
-
-            map_wh_per_object = jnp.asarray(
-                [m.diffuse_map.shape[:2] for m in models])
-            assert isinstance(map_wh_per_object, Integer[Array, "objects 2"])
-
-            double_sided: Bool[Array, "vertices"]
-            double_sided = MergedModel.generate_object_vert_info(
-                counts,
-                [obj.double_sided for obj in objects],
-            )
-            assert isinstance(double_sided, Bool[Array, "vertices"])
-
-        # merge maps
-        diffuse_map, single_map_shape = MergedModel.merge_maps(
-            [m.diffuse_map for m in models])
-        specular_map, _ = MergedModel.merge_maps(
-            [m.specular_map for m in models])
-
-        @jaxtyped
-        @partial(jax.jit, inline=True)
-        def transform_vert(
-            verts: Float[Array, "N 3"],
-            local_scaling: Vec3f,
-            transform: ModelMatrix,
-        ) -> Vertices:
-            """Apply transforms defined in `ModelObject` to vertices."""
-            world: Float[Array, "N 3"] = Camera.apply_pos(
-                verts * local_scaling,
-                transform,
-            )
-            assert isinstance(world, Float[Array, "N 3"])
-
-            return world
-
-        # merge verts
-        verts, faces = MergedModel.merge_verts(
-            [
-                transform_vert(
-                    verts=obj.model.verts,
-                    local_scaling=obj.local_scaling,
-                    transform=obj.transform,
-                ) for obj in objects
-            ],
-            [m.faces for m in models],
-        )
-
-        @jaxtyped
-        @partial(jax.jit, inline=True)
-        def transform_normals(
-            normals: Float[Array, "N 3"],
-            transform: ModelMatrix,
-        ) -> Vertices:
-            """Apply transforms defined in `ModelObject` to vertex normals."""
-            world: Float[Array, "N 3"] = Camera.apply_vec(
-                normals,
-                # transform by inverse transpose
-                jnp.linalg.inv(transform).T,
-            )
-            assert isinstance(world, Float[Array, "N 3"])
-
-            return world
-
-        norms, faces_norm = MergedModel.merge_verts(
-            [
-                transform_normals(obj.model.norms, obj.transform)
-                for obj in objects
-            ],
-            [m.faces_norm for m in models],
-        )
-        uvs, faces_uv = MergedModel.merge_verts(
-            [m.uvs for m in models],
-            [m.faces_uv for m in models],
-        )
-
-        return MergedModel(
-            verts=verts,
-            norms=norms,
-            uvs=uvs,
-            faces=faces,
-            faces_norm=faces_norm,
-            faces_uv=faces_uv,
-            texture_shape=map_wh_per_object,
-            texture_index=map_indices,
-            double_sided=double_sided,
-            offset=single_map_shape[0],
-            diffuse_map=diffuse_map,
-            specular_map=specular_map,
-        )
-
-    @staticmethod
-    @jaxtyped
-    @partial(jax.jit, inline=True)
     def create_camera_from_parameters(camera: CameraParameters) -> Camera:
         """Create a camera from camera parameters."""
-        view_mat: View = Camera.view_matrix(
-            eye=camera.position,
-            centre=camera.target,
-            up=camera.up,
-        )
+        eye: Vec3f = jnp.asarray(camera.position)
+        assert isinstance(eye, Vec3f), f"{eye}"
+        centre: Vec3f = jnp.asarray(camera.target)
+        assert isinstance(centre, Vec3f), f"{centre}"
+        up: Vec3f = jnp.asarray(camera.up)
+        assert isinstance(up, Vec3f), f"{up}"
+
+        view_mat: View = Camera.view_matrix(eye=eye, centre=centre, up=up)
         assert isinstance(view_mat, View), f"{view_mat}"
-        view_inv: View = Camera.view_matrix_inv(
-            eye=camera.position,
-            centre=camera.target,
-            up=camera.up,
-        )
+        view_inv: View = Camera.view_matrix_inv(eye=eye, centre=centre, up=up)
         assert isinstance(view_inv, View), f"{view_inv}"
         projection_mat: Projection = Camera.perspective_projection_matrix(
             fovy=camera.vfov,
             aspect=(lax.tan(jnp.radians(camera.hfov) / 2.) /
                     lax.tan(jnp.radians(camera.vfov) / 2.)),
             z_near=camera.near,
             z_far=camera.far,
@@ -248,14 +133,54 @@
             viewport=viewport_mat,
             view_inv=view_inv,
         )
         assert isinstance(_camera, Camera), f"{_camera}"
 
         return _camera
 
+    @staticmethod
+    @jaxtyped
+    def create_buffers(
+        width: int,
+        height: int,
+        batch: Optional[int] = None,
+        colour_default: Colour = jnp.array((1., 1., 1.), dtype=jnp.single),
+        zbuffer_default: Num[Array, ""] = jnp.array(1, dtype=jnp.single),
+    ) -> Buffers:
+        """Render the scene with the given camera.
+
+        The dtype of `colour_default` and `zbuffer_default` will be used as the
+        dtype of canvas and zbuffer.
+
+        Parameters:
+          - width, height: the size of the image to render.
+          - batch: if specified, will produce a batch of buffers, with batch
+            axis at axis 0.
+          - colour_default: default colours to fill the image with.
+          - zbuffer_default: default zbuffer values to fill with.
+          - shadow_param: the shadow parameters to render the scene with. Keep
+
+        Returns: Buffers, with zbuffer and (coloured image, ).
+        """
+        _batch = (batch, ) if batch is not None else ()
+        zbuffer: ZBuffer = lax.full(
+            (*_batch, width, height),
+            zbuffer_default,
+        )
+        canvas: Canvas = jnp.full(
+            (*_batch, width, height, colour_default.size),
+            colour_default,
+        )
+        buffers: Buffers = Buffers(
+            zbuffer=zbuffer,
+            targets=(canvas, ),
+        )
+
+        return buffers
+
     @classmethod
     @jaxtyped
     @partial(jax.jit, static_argnames=("cls", ), donate_argnums=(4, ))
     def render(
         cls,
         model: MergedModel,
         light: LightParameters,
@@ -367,60 +292,58 @@
 
             return buffers
 
     @classmethod
     @jaxtyped
     def get_camera_image(
         cls,
-        objects: ObjectsT,
+        objects: Sequence[ModelObject],
         light: LightParameters,
         camera: Union[Camera, CameraParameters],
         width: int,
         height: int,
         colour_default: Colour = jnp.array((1., 1., 1.), dtype=jnp.single),
-        zbuffer_default: Num[Array, ""] = jnp.array(1),
-        zbuffer_dtype: jnp.dtype[Any] = jnp.single,
+        zbuffer_default: Num[Array, ""] = jnp.array(1, dtype=jnp.single),
         shadow_param: Optional[ShadowParameters] = None,
     ) -> Canvas:
         """Render the scene with the given camera.
 
+        The dtype of `colour_default` and `zbuffer_default` will be used as the
+        dtype of canvas and zbuffer.
+
         Parameters:
           - objects: the objects to render.
           - light: the light to render the scene with.
           - camera: the camera to render the scene with.
           - width, height: the size of the image to render.
-          - colourChannels: the number of colour channels to render.
+          - colour_default: default colours to fill the image with.
+          - zbuffer_default: default zbuffer values to fill with.
           - shadow_param: the shadow parameters to render the scene with. Keep
 
         Returns: Buffers, with zbuffer and (coloured image, ).
         """
         _camera: Camera
         if isinstance(camera, CameraParameters):
             _camera = cls.create_camera_from_parameters(camera)
         else:
             _camera = camera
 
         assert isinstance(_camera, Camera), f"{_camera}"
 
-        zbuffer: ZBuffer = lax.full(
-            (width, height),
-            jnp.array(zbuffer_default, dtype=zbuffer_dtype),
-        )
-        canvas: Canvas = jnp.full(
-            (width, height, colour_default.size),
-            colour_default,
-        )
-        buffers: Buffers = Buffers(
-            zbuffer=zbuffer,
-            targets=(canvas, ),
+        buffers: Buffers = cls.create_buffers(
+            width=width,
+            height=height,
+            colour_default=colour_default,
+            zbuffer_default=zbuffer_default,
         )
 
-        model: MergedModel = cls.merge_objects(objects)
+        model: MergedModel = merge_objects(objects)
         assert isinstance(model, MergedModel), f"{model}"
 
+        canvas: Canvas
         _, (canvas, ) = cls.render(
             model=model,
             light=light,
             camera=_camera,
             buffers=buffers,
             shadow_param=shadow_param,
         )
```

### Comparing `jaxrenderer-0.1.0/renderer/scene.py` & `jaxrenderer-0.1.1/renderer/scene.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import NamedTuple, NewType, Union
+from typing import NamedTuple, NewType, Optional, Union
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, jaxtyped
 
 from .geometry import transform_matrix_from_rotation
@@ -48,34 +48,37 @@
         return new_scene, guid
 
     @jaxtyped
     def add_cube(
         self,
         half_extents: Union[Float[Array, "3"], tuple[float, float, float]],
         diffuse_map: Texture,
-        texture_scaling: Union[Float[Array, "2"], tuple[float, float]],
+        texture_scaling: Union[Float[Array, "2"], tuple[float, float], float],
     ) -> tuple["Scene", GUID]:
         """Add a cube to the scene.
 
         Parameters:
           - half_extents: the half-size of the cube. The final cube would have
             x-y-z dimension of 2 * half_extents.
           - diffuse_map: the diffuse map of the cube.
-          - texture_scaling: the scaling factor of the texture, in x and y.
+          - texture_scaling: the scaling factor of the texture, in x and y. If
+            only one number is given, it is used for both x and y.
         """
         # reference: https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/model.cpp#L215
         specular_map: SpecularMap = lax.full(diffuse_map.shape[:2], 2.0)
 
         _half_extents = jnp.asarray(half_extents)
         assert isinstance(_half_extents, Float[Array, "3"]), (
-            "Expected 2 floats in half_extends, got {half_extents}")
+            f"Expected 2 floats in half_extends, got {half_extents}")
 
         _texture_scaling = jnp.asarray(texture_scaling)
+        if _texture_scaling.size == 1:
+            _texture_scaling = lax.full((2, ), _texture_scaling)
         assert isinstance(_texture_scaling, Float[Array, "2"]), (
-            "Expected 2 floats in texture_scaling, got {texture_scaling}")
+            f"Expected 2 floats in texture_scaling, got {texture_scaling}")
 
         model: Model = create_cube(
             half_extents=_half_extents,
             texture_scaling=_texture_scaling,
             diffuse_map=diffuse_map,
             specular_map=specular_map,
         )
@@ -198,43 +201,62 @@
 
         return self._replace(objects=self.objects | {object_id: new_obj})
 
     @jaxtyped
     def set_object_orientation(
         self,
         object_id: GUID,
-        orientation: Vec4f,
+        orientation: Optional[Union[Vec4f, tuple[float, float, float,
+                                                 float]]] = None,
+        rotation_matrix: Optional[Float[Array, "3 3"]] = None,
     ) -> "Scene":
         """Set the orientation of an object in the scene.
 
+        If rotation_matrix is specified, it takes precedence over orientation.
+        If none is specified, the object's orientation is set to identity.
+
         Parameters:
           - object_id: the unique identifier of the object.
-          - orientation: the new orientation of the object.
+          - orientation: the new orientation of the object, optional.
+          - rotation_matrix: the new rotation matrix of the object, optional
         """
-        mat: Float[Array, "3 3"] = transform_matrix_from_rotation(orientation)
-        assert isinstance(mat, Float[Array, "3 3"]), f"{mat}"
+        if rotation_matrix is None:
+            if orientation is None:
+                orientation = (0., 0., 0., 1.)
+
+            _orientation = jnp.asarray(orientation, dtype=float)
+            assert isinstance(_orientation, Vec4f), f"{orientation}"
+            rotation_matrix = transform_matrix_from_rotation(_orientation)
+
+        assert isinstance(
+            rotation_matrix,
+            Float[Array, "3 3"],
+        ), f"{rotation_matrix}"
 
         obj: ModelObject = self.objects[object_id]
-        new_mat: Float[Array, "4 4"] = obj.transform.at[:3, :3].set(mat)
+        new_mat: Float[Array, "4 4"]
+        new_mat = obj.transform.at[:3, :3].set(rotation_matrix)
         new_obj: ModelObject = obj._replace(transform=new_mat)
 
         return self._replace(objects=self.objects | {object_id: new_obj})
 
     @jaxtyped
     def set_object_local_scaling(
         self,
         object_id: GUID,
-        local_scaling: Vec3f,
+        local_scaling: Union[Vec3f, tuple[float, float, float]],
     ) -> "Scene":
         """Set the local scaling of an object in the scene.
 
         Parameters:
           - object_id: the unique identifier of the object.
           - local_scaling: the new local scaling of the object.
         """
+        local_scaling = jnp.asarray(local_scaling, dtype=float)
+        assert isinstance(local_scaling, Vec3f), f"{local_scaling}"
         obj: ModelObject = self.objects[object_id]
         new_obj: ModelObject = obj._replace(local_scaling=local_scaling)
 
         return self._replace(objects=self.objects | {object_id: new_obj})
 
     @jaxtyped
     def set_object_double_sided(
```

### Comparing `jaxrenderer-0.1.0/renderer/shader.py` & `jaxrenderer-0.1.1/renderer/shader.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/shaders/README.md` & `jaxrenderer-0.1.1/renderer/shaders/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/shaders/depth.py` & `jaxrenderer-0.1.1/renderer/shaders/depth.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/shaders/gouraud.py` & `jaxrenderer-0.1.1/renderer/shaders/gouraud.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/shaders/gouraud_texture.py` & `jaxrenderer-0.1.1/renderer/shaders/gouraud_texture.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/shaders/phong.py` & `jaxrenderer-0.1.1/renderer/shaders/phong.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/shaders/phong_darboux.py` & `jaxrenderer-0.1.1/renderer/shaders/phong_darboux.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/shaders/phong_reflection.py` & `jaxrenderer-0.1.1/renderer/shaders/phong_reflection.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/shaders/phong_reflection_shadow.py` & `jaxrenderer-0.1.1/renderer/shaders/phong_reflection_shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/shadow.py` & `jaxrenderer-0.1.1/renderer/shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/shapes/capsule.py` & `jaxrenderer-0.1.1/renderer/shapes/capsule.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/shapes/cube.py` & `jaxrenderer-0.1.1/renderer/shapes/cube.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/types.py` & `jaxrenderer-0.1.1/renderer/types.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/renderer/utils.py` & `jaxrenderer-0.1.1/renderer/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,17 +45,31 @@
 
     return zbuffer, canvas
 
 
 @jaxtyped
 @jax.jit
 def transpose_for_display(
-        matrix: Num[Array,
-                    "fst snd *channel"]) -> Num[Array, "snd fst *channel"]:
-    return jnp.swapaxes(matrix, 0, 1)
+    matrix: Num[Array, "fst snd *channel"],
+    flip_vertical: bool = True,
+) -> Num[Array, "snd fst *channel"]:
+    """Transpose matrix for display.
+
+    When flip_vertical is disabled, the matrix's origin ([0, 0]) is assumed to
+    be at bottom-left. Thus, the correct way to display the matrix is to using
+    tools like matplotlib is to specify `origin="lower"`.
+    To be compatible with PyTinyrenderer and most image processing programs,
+    the default behavior is to flip vertically.
+    """
+    mat = jnp.swapaxes(matrix, 0, 1)
+    assert isinstance(mat, Num[Array, "snd fst *channel"])
+    if flip_vertical:
+        mat = mat[::-1, ...]
+
+    return mat
 
 
 @jaxtyped
 def build_texture_from_PyTinyrenderer(
     texture: Union[Num[Array, "length"], Sequence[float]],
     width: int,
     height: int,
@@ -71,9 +85,12 @@
         the resulted texture still has 3 dimensions, with last dimension of
         side 1.
       - width: width of the texture.
       - height: height of the texture.
 
     Returns: A texture with shape `(width, height, channels)`.
     """
-    return jnp.reshape(texture, (width, height, -1),
-                       order="C").swapaxes(0, 1)[:, ::-1, :]
+    return jnp.reshape(
+        jnp.asarray(texture),
+        (width, height, -1),
+        order="C",
+    ).swapaxes(0, 1)[:, ::-1, :]
```

### Comparing `jaxrenderer-0.1.0/renderer/value_checker.py` & `jaxrenderer-0.1.1/renderer/value_checker.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.0/PKG-INFO` & `jaxrenderer-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxrenderer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Jax implementation of rasterizer renderer.
 Home-page: https://github.com/JoeyTeng/jaxrenderer
 License: Apache-2.0
 Author: Joey Teng
 Author-email: joey.teng.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

