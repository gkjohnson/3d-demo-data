# Blendswap Models

Scenes converted from [Blendswap](https://blendswap.com/) .blend files for the three-gpu-pathtracer demos. Materials are collapsed to Principled BSDF for glTF export, unsupported node graphs are baked to textures, and area lights are carried as emissive planes the demo converts back to area lights.

Each file is optimized with the following, which keeps the scene graph and geometry intact while compressing meshes with Draco and textures as WebP:

```
gltf-transform optimize <input> <output> \
	--simplify false --weld false --join false \
	--compress draco --texture-compress webp
```

| File | Scene | Author | License |
| --- | --- | --- | --- |
| sasha.glb | [Sasha Ring](https://blendswap.com/blend/29574) | saber7711 | CC BY 3.0 |
| magie-noire.glb | [Magie Noire Perfume](https://blendswap.com/blend/30512) | Bagoule | CC0 |
| stormtrooper.glb | [Stormtrooper Star Wars VII](https://blendswap.com/blend/13953) (fan art) | ScottGraham | CC BY 3.0 |
| teapot.glb | [Stelton Theo Teapot Set](https://blendswap.com/blend/22379) (fan art) | blendswapisweird | CC0 |
| dining-room.glb | [Dining room](https://blendswap.com/blend/18762) | MaTTeSr | CC BY 3.0 |
| dodge-challenger.glb | [Dodge Challenger 1970 R/T](https://blendswap.com/blend/4046) | kryptonmedia | CC0 |
| tropical.glb | [Tropical scene](https://blendswap.com/blend/29301) | ksyu3d | CC BY 3.0 |

`tropical-beach.hdr` is the tropical scene's world lighting - the [Spiaggia di Mondello](https://polyhaven.com/a/spiaggia_di_mondello) HDRI from Poly Haven (CC0) - rendered back out with the scene's rotation and strength applied.
