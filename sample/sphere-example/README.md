```sh
blockMesh
surfaceFeatureExtract
snappyHexMesh -overwrite
decomposePar
mpirun -np 4 simpleFoam -parallel
```
