Anonymous medical physicist from National Centre for Nuclear Research (Poland)

This is not me. 

This file has to be opened from software supporting u3d (e.g. Acrobat Reader)

The pipeline was the following:

## ev3dev-mapping-ui

1. Gather data with ev3dev-mapping-ui
2. Export point cloud to ply file format

## MeshLab

1. Import ply point cloud to MeshLab
2. Select region of interest
3. Invert selection
4. Delete selected vertices
5. Conditional vertex selection with y < 0.01
6. Delete selected vertices
7. Compute normals for point sets
8. Surface Reconstruction: Poisson
9. Transform: Move, Translate, Center (check all)
10. Export mesh to u3d (this results in u3d and tex file)

## Latex

pdflatex on result tex file

