# yocto_templateconf/ggc/rcar-gen3

This layer provides the configuration to use AWS Greengrass on the R-Car.

## Dependencies

This layer depends on:

* URI: git://git.yoctoproject.org/poky
  * branch: dunfell
  * revision: 74b22db6879b388d700f61e08cb3f239cf940d18

* URI: git://github.com/renesas-rcar/meta-renesas
  * layers; meta-rcar-gen3
  * branch: dunfell
  * revision: 13fd24957b9acc29a235ee0c7f398fd867f38b47

* URI: git://git.openembedded.org/meta-openembedded
  * layers: meta-oe, meta-networking, meta-python, meta-filesystems
  * branch: dunfell
  * revision: 814eec96c2a29172da57a425a3609f8b6fcc6afe

* URI: git://git.yoctoproject.org/meta-virtualization
  * branch: dunfell
  * revision: c4f156fa93b37b2428e09ae22dbd7f5875606f4d

* URI: git://git.yoctoproject.org/meta-java
  * branch: dunfell
  * revision: eeb136c64ecaa364d4e332d0182865dc65f2a83b

* URI: git://github.com/aws/meta-aws
  * branch: dunfell
  * revision: 9979cfa676105cb68cfadfdaeabf044d7c919319

* URI: git://github.com/tkomagata/meta-docker
  * layers; meta-rcar-gen3
  * branch: dunfell
  * revision: ed0ed36e81b65c2f6707965e8bc379cabb0c1927

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
