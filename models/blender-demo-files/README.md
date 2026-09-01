# Blender Demo Files

Scenes converted from the official [Blender demo files](https://www.blender.org/download/demo-files/) for the three-gpu-pathtracer demos. Materials are collapsed or baked for glTF export and area lights are carried as emissive planes the demo converts back to area lights. Licensing is as stated on the Blender demo files page.

Each file is optimized with the following, which keeps the scene graph and geometry intact while compressing meshes with Draco and textures as WebP:

```
gltf-transform optimize <input> <output> \
	--simplify false --weld false --join false \
	--compress draco --texture-compress webp
```

| File | Scene | Author |
| --- | --- | --- |
| lone-monk.glb | Lone Monk | Carlo Bergonzini / Monorender |
| monster.glb | Monster Under The Bed | Metin Seven, based on 2D concept art by Blake Stevenson |

The monster is rendered with subsurface scattering in the source scene, which glTF cannot carry - the demo stands in a rough transmissive material at load time.
