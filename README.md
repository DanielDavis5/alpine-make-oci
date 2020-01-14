# alpine-make-oci

## Description

Creates Alpine Linux [OCI Image](https://github.com/opencontainers/image-spec).

## Installation

```
meson build
ninja -C build install
```

## Help

    ./alpine-make-oci --help

## Run without root

    ./alpine-make-oci unshare [options] <destination> [ -- [flags] ]

## Flags

Arguments to be forwarded to [buildah-config](https://github.com/containers/buildah/blob/master/docs/buildah-config.md).
