This is CSI like scene with my dead body lying on the floor, scanned by robot programmed for path repeating.
This is almost raw result as seen in ev3dev-mapping-ui.

See the result [here](http://htmlpreview.github.io/?https://github.com/bmegli/ev3dev-mapping-results/blob/master/point%20clouds/html/crime%20scene/crime_scene.html)

Note that this scene, as opposed to html examples in face reconstructions, will not work if downloaded and opened locally.

Inline x3d needs something to serve it (Apache, etc.). 

The pipeline was the following:

## ev3dev-mapping-ui

1. Gather data with ev3dev-mapping-ui
2. Export point cloud to ply file format

## MeshLab

1. Import ply point cloud to MeshLab
2. Per Vertex Color Function (white colour for all)
3. Export mesh to x3d with only verices and colour data
4. Manually add viewpoint to x3d file (see crime_scene.x3d)
8. Add inline x3d to minimalistic html file (see crime_scene.html)



