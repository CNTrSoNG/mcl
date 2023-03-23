[![Build Status](https://github.com/herumi/mcl/actions/workflows/main.yml/badge.svg)](https://github.com/herumi/mcl/actions/workflows/main.yml)

# Build with cmake (without WASI)

* Only static libs are built.
* No printf. 

```
cmake .. -DMCL_USE_GMP=OFF -DMCL_USE_ASM=OFF -DMCL_STATIC_LIB=ON -DCMAKE_TOOLCHAIN_FILE="$WASI_SDK_ROOT/share/cmake/wasi-sdk.cmake" -DWASI_SDK_PREFIX=$WASI_SDK_ROOT -DCMAKE_BUILD_TYPE=Release -LA
```
