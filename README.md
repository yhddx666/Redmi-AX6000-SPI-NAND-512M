# Redmi-AX6000-SPI-NAND-512MB
用于红米AX6000改512MB闪存atf_uboot以及固件云编译。

具体教程看大佬文章：https://www.right.com.cn/forum/thread-8261227-1-1.html

本人仅在固件中添加几个常用插件

固件已集成kmod-mtd-rw，运行下面命令加载后解锁分区的写入：

```bash
insmod /lib/modules/$(uname -r)/mtd-rw.ko i_want_a_brick=1
```
