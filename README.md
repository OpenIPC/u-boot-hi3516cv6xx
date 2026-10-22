# Retired: hi3516cv6xx is built in OpenIPC/u-boot

This repository is archived. Hi3516CV610 and Hi3516CV608 U-Boot is now built
from the same tree as every other HiSilicon and Goke SoC OpenIPC supports: the
`openipc-hisilicon` branch of
[OpenIPC/u-boot](https://github.com/OpenIPC/u-boot/tree/openipc-hisilicon)
(OpenIPC/u-boot#32), with its CI on the `openipc` branch (OpenIPC/u-boot#34).
This repository stopped publishing in #10.

The signed boot images keep their names, `boot-hi3516cv610-<ddr>-nor.bin` and
`boot-hi3516cv608-nor.bin`, in the
[OpenIPC/firmware `latest`](https://github.com/OpenIPC/firmware/releases/tag/latest)
release. They now carry the OpenIPC boot layer shared with the other SoCs,
which finds the flash layout at boot, including the split NOR image.

The upstream U-Boot documentation is in `README`; the history here stays
readable for reference.
