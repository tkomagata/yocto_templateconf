# yocto_templateconf/rz-vlp/rzg-vlp

This layer provides the configuration to use AWS Greengrass on the RZ/G.

## Dependencies

This layer depends on:

* URI: git://git.yoctoproject.org/poky
  * branch: dunfell
  * revision: bba323389749ec3e306509f8fb12649f031be152

* URI: git://git.yoctoproject.org/meta-gplv2
  * branch: dunfell
  * revision: 60b251c25ba87e946a0ca4cdc8d17b1cb09292ac

* URI: https://github.com/renesas-rz/meta-renesas
  * branch: dunfell
  * revision: 4aa5c708036f2e6408a8af673fe15e51247378f6

* URI: git://git.openembedded.org/meta-openembedded
  * layers: meta-oe, meta-python, meta-multimedia, meta-filesystems, meta-networking
  * branch: dunfell
  * revision: ec978232732edbdd875ac367b5a9c04b881f2e19

* URI: git://git.yoctoproject.org/meta-virtualization
  * branch: dunfell
  * revision: "c5f61e547b90aa8058cf816f00902afed9c96f72

* URI: git://git.yoctoproject.org/meta-java
  * branch: dunfell
  * revision: eeb136c64ecaa364d4e332d0182865dc65f2a83b

* URI: https://github.com/aws/meta-qt5
  * branch: dunfell
  * revision: c1b0c9f546289b1592d7a895640de103723a0305

* URI: https://github.com/aws/meta-aws
  * branch: dunfell
  * revision: a64c32254c3731e9b3c40231bd60d2b21efa0488

## Patches

Please submit any to the the maintainer:

Maintainer: Tomohiro Komagata <tomohiro.komagata.aj at gmail.com>

## Quick Start

1. MACHINE={h3ulcb or m3ulcb}
2. TEMPLATECONF=$PWD/yocto_templateconf/ggc/rz-vlp/rzg-vlp/ \
   source poky/oe-init-build-env rz-build
3. bitbake core-image-minimal

## Supported Boards/Machines

- Renesas Electronics Corporation. Renesas RZ/G2L Evaluation Board Kit
