# Description

Creates [OCI compliant](https://github.com/opencontainers/image-spec) Alpine Linux container image.

# Usage

## Normal

    alpine-make-oci [options] [ -- [config_flags] ]

## Rootless

    alpine-make-oci unshare [options] [ -- [config_flags] ]

## Options

    -h, --help                      Show this message then exit.
    -k, --keep                      Keep image in the local repository.
    -n, --name=<name>               Generated image name.
    -o, --output=<path>             Save a compressed OCI bundle at the specified location.

## Config Flags

Arguments to pass to buildah-config; see [buildah-config(1)](https://github.com/containers/buildah/blob/master/docs/buildah-config.md).

# Installation

## [Arch User Repositiory](https://aur.archlinux.org/)

    yay -S alpine-make-oci

## From Source

### Install dependencies

* [Buildah](https://github.com/containers/buildah) ***(run-time)***

* [alpine-make-rootfs](https://github.com/alpinelinux/alpine-make-rootfs) ***(run-time)***

* [meson](https://github.com/mesonbuild/meson) ***(build)***

### Install the script

    meson build
    sudo ninja -C build install
