fastSHT is a very fast toolkit for doing spherical harmonic transforms on a large number of spherical maps. It converts massive SHT operations to a BLAS level 3 problem and uses the highly optimized matrix multiplication toolkit to accelerate the computation. GPU acceleration is supported and can be very effective. Core code is written in fortran but a Python wrapper is provided and recommended.


# Dependencies

Fortran compiler: `ifort` is recommanded for the CPU version; `nvfortran` is required for the GPU version

Intel MKL library

[`f90wrap`](https://github.com/jameskermode/f90wrap)

`Python3`, `numpy`, `CMake`


# (Recommended) Download and compile with the docker image that is compatable with both CPU and GPU version

```
docker pull rectaflex/intel_nvidia_sdk
```

# Compilation

```
./compile.sh # for the CPU version
```

```
./compile.sh -DGPU=on # for the GPU version
```

# Examples and Testing
General tests and comparisons with Healpy is in `scripts/test_all.py`.

Notebook that demonstrates the basic interfaces is in  `scripts/demo.ipynb`.


# Citing fastSHT

...
