# yocto_templateconf/ggc/rcar-gen3

This layer provides the configuration to use AWS Greengrass on the R-Car.

## Dependencies

This layer depends on:

* URI: git://git.yoctoproject.org/poky
  * branch: dunfell
  * revision: 6ebb33bdaccaeadff0c85aab27acf35723df00d8

* URI: git://github.com/renesas-rcar/meta-renesas
  * layers; meta-rcar-gen3
  * branch: dunfell
  * revision: 0fe77668f5d9a31a5d10449988c3d8fb8dc475c5

* URI: git://git.openembedded.org/meta-openembedded
  * layers: meta-oe, meta-networking, meta-python, meta-filesystems
  * branch: dunfell
  * revision: c38d2a74f762a792046f3d3c377827b08aade513

* URI: git://git.yoctoproject.org/meta-virtualization
  * branch: dunfell
  * revision: 92cd3467502bd27b98a76862ca6525ce425a8479

* URI: git://git.yoctoproject.org/meta-java
  * branch: dunfell
  * revision: 62d6c0653ad69e14c21db2d4482e578400116a1b

* URI: git://github.com/aws/meta-aws
  * branch: dunfell
  * revision: 09a9e8845e1c0685d279a5fec12dc2764e67675c

* URI: git://github.com/tkomagata/meta-docker
  * layers; meta-rcar-gen3
  * branch: dunfell
  * revision: 1ca1b5caf6f373dcc49db82dce50f4d8ab9f25cd

## Patches

Please submit any to the the maintainer:

Maintainer: Tomohiro Komagata <tomohiro.komagata.aj at gmail.com>

## Quick Start

1. MACHINE={h3ulcb or m3ulcb}
2. TEMPLATECONF=$PWD/yocto_templateconf/ggc/rcar-gen3/${MACHINE}/bsp/ \
   source poky/oe-init-build-env rcar-build
3. bitbake core-image-minimal
4. Prepare a SD card and set the u-boot environment variables. Please refer the [R-Car page on eLinux Wiki](https://elinux.org/R-Car/Boards/Yocto-Gen3/v5.5.0#Running_Yocto_images).
4. Boot your R-Car Starter Kit.

## Supported Boards/Machines

- Renesas Electronics Corporation. R-Car Starter Kit premier(H3ULCB) (R8A7795)
- Renesas Electronics Corporation. R-Car Starter Kit pro(M3ULCB) (R8A7796)
