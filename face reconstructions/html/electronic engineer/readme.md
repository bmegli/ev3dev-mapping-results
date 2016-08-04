Anonymous electronic engineer from National Centre for Nuclear Research (Poland)

This is not me.

See the [result](http://htmlpreview.github.io/?https://github.com/bmegli/ev3dev-mapping-results/blob/master/face%20reconstructions/html/electronic%20engineer/electronic_engineer.html) here.

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
10. Export mesh to ply with vertices, normals and faces

## aopt

aopt -i mesh.ply -N mesh.html


