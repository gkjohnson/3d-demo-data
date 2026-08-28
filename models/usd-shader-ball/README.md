Converted model from the USD working group assets project.

**Source**

https://github.com/usd-wg/assets/tree/main/full_assets/StandardShaderBall

This work is licensed under a Creative Commons Attribution 4.0 International Licence.

**Files**

- `usd-shaderball-ball.glb`, `usd-shaderball-scene.glb` - converted from the original v1.0 asset.
- `standard-shader-ball.glb` - converted from the v1.1 asset via headless Blender:
  - ACEScg EXR textures converted to sRGB PNG, then compressed to webp. Geometry draco-compressed.
  - Subdivision surfaces applied at level 2.
  - Lights removed - they are expected to be recreated in code from the USD layer values.
  - Camera included, using the v1.1 conventions (50mm focal length, 20.955mm aperture).
  - The `sss_bars` texture is manually assigned since the asset's UsdPreviewSurface omits it.
