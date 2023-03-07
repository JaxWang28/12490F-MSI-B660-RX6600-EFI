* macOS 13.2.2
* opencore 0.9.0



| 硬件 | 型号                                                         |
| ---- | ------------------------------------------------------------ |
| 主板 | 微星 [MAG B660M](https://www.msi.com/Motherboard/MAG-B660M-MORTAR-DDR4) |
| CPU  | i5-12490f                                                    |
| 显卡 | ASUS [RX6600](https://www.asus.com/hk/motherboards-components/graphics-cards/dual/dual-rx6600-8g/) |
| SSD  | [WD_BLACK SN770 NVMe™ SSD](https://www.westerndigital.com/zh-cn/products/internal-drives/wd-black-sn770-nvme-ssd#WDS250G3X0E) |
| RAM  | GLOWAY 光威天策系列DDR4 3200MHz                              |
| 网卡 | [FENVI-T919](https://cn.fenvi.com/product_detail_27.html)    |



| 功能     | 完善程度 |
| -------- | -------- |
| wifi     | 正常     |
| 隔空投送 | 正常     |
| 蓝牙     | 正常     |
|          |          |



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



* ~~对于免驱显卡且设置正确机型，whateverGreen是不需要的。~~it is encouraged to use WhateverGreen.

* 启动项中多了 EFI boot，原因是boot文件夹下缺少两个隐藏文件 0.8.9 开始

* 虽然i5 12490f没有大小核，ProvideCurrentCpuInfo 也是必须的。

