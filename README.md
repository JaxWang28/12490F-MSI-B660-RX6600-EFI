# 基本信息

* macOS 13.2.1
* opencore 0.9.0

* `config.plist`中的三码已经删除，请自行添加。



# 硬件信息

| 硬件 | 型号                                                         |
| ---- | ------------------------------------------------------------ |
| 主板 | 微星 [MAG B660M](https://www.msi.com/Motherboard/MAG-B660M-MORTAR-DDR4) |
| CPU  | i5-12490f                                                    |
| 显卡 | ASUS [RX6600](https://www.asus.com/hk/motherboards-components/graphics-cards/dual/dual-rx6600-8g/) |
| SSD  | [WD_BLACK SN770 NVMe™ SSD](https://www.westerndigital.com/zh-cn/products/internal-drives/wd-black-sn770-nvme-ssd#WDS250G3X0E) |
| RAM  | GLOWAY 光威天策系列DDR4 3200MHz                              |
| 网卡 | [FENVI-T919](https://cn.fenvi.com/product_detail_27.html)    |



# 完善度

| 功能     | 完善程度 |
| -------- | -------- |
| wifi     | 正常     |
| 隔空投送 | 正常     |
| 蓝牙     | 正常     |
|          |          |





# Kexts 版本

| Kexts               | Version |
| ------------------- | ------- |
| Lilu                | 1.6.4   |
| VirtualSMC          | 1.3.1   |
| SMCProcessor        | 1.3.0   |
| SMCSuperIO          | 1.3.0   |
| AppleALC            | 1.8.0   |
| CPUFriend           | 1.2.6   |
| LucyRTL8125Ethernet | 1.1.0   |
| WhateverGreen       | 1.6.4   |
| RadeonSensor        | 0.3.3   |
| SMCRadeonGPU        | 0.3.3   |
| USBToolBox          | 1.1.1   |
| RestrictEvents      | 1.0.9   |



# 已知问题

* 自己生成的`CPUFriendData`不能实现睿频。




# 填过的坑

* 启动项中多了 EFI boot，原因是boot文件夹下缺少两个隐藏文件 0.8.9 开始
* ~~对于免驱显卡且设置正确机型，whateverGreen是不需要的~~
* it is encouraged to use WhateverGreen.
* i5-12490f 是没有大小核的，但是不勾选 `ProvideCurrentCpuInfo` 不能进入系统。原因是 kernel 中的 patch 中的 `_cpuid_set_info` 与其是配套使用的，需要同时弃用。
