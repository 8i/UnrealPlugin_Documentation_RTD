============================================================
Troubleshooting
============================================================

## Pat holograms are not casting any shadows.
------------------------------------------------------------

Please be sure to set the lighting in the scene to stationary or moveable. Pat meshes are dynamic instances that will not recieve lighting when using static lights.

## Remote PAT manifests are not playing.

Please ensure that the manifests are properly hosted.

## Local PAT manifest are playing in the editor but not my built executable.

Please ensure that Local assests are being properly packaged during the build step. Ensure that *Additional Non-Asset Directories To Copy* are being set correctly.
