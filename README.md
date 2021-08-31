CloudCompare_OSGV
============

This is a modified fork of CloudCompare that adds a proof-of-concept implementation of Osteon Scan Gauge Validation
(OSGV). The validation process is exposed via the new command-line function `-OSGV` which will perform the validation
between the first two loaded CAD (stl) models and write results to the given output folder. To demonstrate, it is invoked like so:

```shell
CloudCompare.exe -o /path/to/upperjaw.stl -o /path/to/lowerjaw.stl -OSGV /path/to/output
```

If successful, the output folder will contain a PLY mesh with the lowerjaw model and ICP registered upperjaw model combined.
The upperjaw model will have a different color map applied to it.

See the original [README.md](README_original.md) for more information.
