* nose cone test case for steady state solver - simpleFoam

```sh
blockMesh
surfaceFeatureExtract
snappyHexMesh -overwrite
decomposePar
mpirun -np 4 simpleFoam -parallel
```
