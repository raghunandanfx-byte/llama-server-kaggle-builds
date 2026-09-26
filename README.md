# llama-server Kaggle Builds

Reproducible precompiled `llama-server` binaries for Kaggle GPU runtimes.

## Current target

- llama.cpp: `b11146`
- OS ABI: Ubuntu 22.04 / glibc 2.35
- CUDA toolkit: 12.8.1
- GPU target: `sm_75` (Tesla T4)
- Flash Attention: enabled
- FA K/V quant combinations: **all supported combinations**
- VMM: disabled for Kaggle compatibility
- NCCL: disabled
- Binary RPATH: `$ORIGIN`

Successful builds are published as GitHub Release assets with a SHA-256 checksum.

## Release naming

`b11146-kaggle-sm75-fa-all`

## Package naming

`llama-server-b11146-ubuntu22.04-glibc2.35-cuda12.8-sm75-fa-all.tar.gz`

The package contains `llama-server` and the local llama.cpp shared libraries it requires. It does not bundle glibc, libstdc++, or CUDA runtime libraries supplied by Kaggle.
