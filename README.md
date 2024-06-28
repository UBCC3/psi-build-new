About psi4-feedstock
====================

This is a modification of the [Psi4 feedstock for Conda](https://github.com/conda-forge/psi4-feedstock/) that makes it
build a copy of this repository. It is unable to complete the post-build tests, but it manages to build an output file
in `build_artifacts/broken`. The test issues are due to Git version mismatches, which are not trivial to fix without
reworking how this Git repo works... In the mean time, this is "good enough" for generating a package for the compute
cluster.

To build, run...
```sh
python3 build-locally.py
```

And it should crash only in the testing stage ;)
