## build

```shell
./mk.sh mx6q_topeet_defconfig
./mk.sh -j8
./mk.sh menuconfig
./mk.sh savedefconfig
cp defconfig configs/mx6q_topeet_defconfig
```

## download

- `sudo dd if=u-boot-dtb.imx of=/dev/sdc bs=512 seek=2 && sync`

