# hipBLAS-common
Common files shared by hipBLAS and hipBLASLt

## Build Instructions

There are 2 ways to build the hipblas-common package:

### rmake script

Simply run the rmake script:

`./rmake --install`

### Calling cmake and make directly

```
mkdir build
cd build
cmake ..
make package install
```
