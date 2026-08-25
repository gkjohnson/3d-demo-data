GLB models courtesy of NASA / JPL-Caltech.

**Source**

https://mars.nasa.gov/resources/25042/mars-perseverance-rover-3d-model/

https://mars.nasa.gov/resources/25043/mars-ingenuity-helicopter-3d-model/

https://mars.nasa.gov/resources/24883/spirit-and-opportunity-rover-3d-model/

https://science.nasa.gov/resource/insight-lander-3d-model/

https://science.nasa.gov/resource/juno-3d-model/

`InSight.glb` and `Juno.glb` are optimized with:

```
gltf-transform optimize <input> <output> \
	--flatten false --join false --instance false --simplify false \
	--compress draco --texture-compress webp --texture-size 2048
```
