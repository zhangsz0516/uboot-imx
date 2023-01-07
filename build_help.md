## imx6q board for topeet

`$ ./mk.sh mrproper`
`$ ./mk.sh mx6q_topeet_defconfig`
`$ ./mk.sh -j4`

## download to SD card

`sudo dd if=u-boot-dtb.imx of=/dev/sdc bs=512 seek=2 && sync`

- `/dev/sdc` is the sd card device


## u-boot start info

```c
U-Boot 2022.04-gdad04f4713 (Jan 07 2023 - 19:51:31 +0800)

CPU:   i.MX6Q rev1.3 996 MHz (running at 792 MHz)
CPU:   Extended Commercial temperature grade (-20C to 105C) at 33C
Reset cause: POR
Model: i.MX6 Quad Topeet Smart Device Board
DRAM:  2 GiB
Core:  80 devices, 19 uclasses, devicetree: separate
MMC:   FSL_SDHC: 1, FSL_SDHC: 2, FSL_SDHC: 3
Loading Environment from MMC... OK
No panel detected: default to Hannstar-XGA
Display: Hannstar-XGA (1024x768)
In:    serial
Out:   serial
Err:   serial
SEC0:  RNG instantiated
switch to partitions #0, OK
mmc1 is current device
flash target is MMC:1
Net:   Could not get PHY for FEC0: addr 1
Could not get PHY for FEC0: addr 1
No ethernet found.

Fastboot: Normal
Normal Boot
Hit any key to stop autoboot:  0

```


