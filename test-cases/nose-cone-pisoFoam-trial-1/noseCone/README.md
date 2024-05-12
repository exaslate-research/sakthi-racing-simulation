cp -r 0.orig 0
blockMesh
surfaceFeatureExtract
snappyHexMesh -overwrite
decomposePar
mpirun -np 8 potentialFoam -parallel -initialiseUBCs -writePhi
mpirun -np 8 simpleFoam -parallel