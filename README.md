CloudCompare_OSGV
============

This is a modified fork of CloudCompare that adds a proof-of-concept implementation of Osteon Scan Gauge Validation
(OSGV). The validation process is exposed via the new command-line function `-OSGV` which will perform the validation
between the first two loaded CAD (stl) models and write results to a `.tmp` folder. To demonstrate, it is invoked like 
so:

```shell
CloudCompare.exe -o /path/to/upperjaw.stl -o /path/to/lowerjaw.stl -OSGV -ROT_AXIS 1
```

*Note: The `-ROT_AXIS` option is optional and defaults to `1` (Y-axis).*

If successful, the comparison results, and a difference point cloud will be saved to a `.tmp` folder in the working 
directory. The results will be placed in separate folders inside `.tmp` with a unique name based on the scan filenames.

See the original [README.md](README_original.md) for more information.
