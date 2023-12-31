# singleCoreGEMM_BMOpenBLAS

Benchmark of OpenBLAS for single core GEMM.

## build and run

Before running the project,
environment variables for the number of threads should be set.

``` bash
export OPENBLAS_NUM_THREADS=1
export GOTO_NUM_THREADS=1
export OMP_NUM_THREADS=1
```

### manually

Build this project using `xmake`.
Follow commands below.

``` bash
xmake
```

Run using `xmake`.
Follow commands below.

``` bash
xmake run singleCoreGEMM_BMOpenBLAS [size]
```

### automatically

Run the script `run.sh` to build and run automatically.
It will execute GEMM with sizes [8, 16, 32, 64, 128, 256, 512, 1024, 2048, 4096, 8192, 16384, 32768].

``` bash
bash run.sh
```
