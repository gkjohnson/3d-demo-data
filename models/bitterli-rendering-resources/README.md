# Bitterli Rendering Resources

Scenes from [Benedikt Bitterli's rendering resources](https://benedikt-bitterli.me/resources/).

Each file is optimized with the following, which keeps the scene graph and geometry intact while compressing meshes with Draco and textures as WebP:

```
gltf-transform optimize <input> <output> \
	--flatten false --join false --instance false --simplify false \
	--compress draco --texture-compress webp
```

Every scene includes the camera it was authored with. Area lights are converted to emissive geometry, and environment map lighting is not carried over.

| File | Scene | Author | License |
| --- | --- | --- | --- |
| bedroom.glb | Bedroom | SlykDrako | CC0 |
| breakfast-room.glb | The Breakfast Room | Wig42 | CC BY 3.0 |
| coffee-maker.glb | Coffee Maker | cekuhnen | CC BY 3.0 |
| contemporary-bathroom.glb | Contemporary Bathroom | Mareck | CC0 |
| country-kitchen.glb | Country Kitchen | Jay-Artist | CC BY 3.0 |
| dragon.glb | Dragon | Delatronic | CC BY 3.0 |
| grey-and-white-room.glb | The Grey & White Room | Wig42 | CC BY 3.0 |
| little-lamp.glb | Little Lamp | UP3D | CC0 |
| salle-de-bain.glb | Salle de bain | nacimus | CC BY 3.0 |
| veach-bidir-room.glb | Veach, Bidir Room | Benedikt Bitterli | CC0 |
| white-room.glb | The White Room | Jay-Artist | CC BY 3.0 |
| wooden-staircase.glb | The Wooden Staircase | Wig42 | CC BY 3.0 |
