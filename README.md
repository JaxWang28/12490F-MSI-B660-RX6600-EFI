* CPU i5-12490f
* GPU rx6600
* 主板 msi-b660m
* 固态 wd-770
* 网卡 FENVi-T919



* macOS 13.2.2
* Opencore 0.9.0



* ~~对于免驱显卡且设置正确机型，whateverGreen是不需要的。~~

* 启动项中多了 EFI boot，原因是boot文件夹下缺少两个隐藏文件 0.8.9 开始

* it is encouraged to use WhateverGreen.

* 虽然i5 12490f没有大小核，ProvideCurrentCpuInfo 也是必须的。



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





