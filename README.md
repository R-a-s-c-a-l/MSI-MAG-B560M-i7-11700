# MSI-MAG-B560M-i7-11700

|            |                                                           |
| --------   | --------------------------------------------------------- |
| Mobo       | MSI-MAG-B560-MORTAR                                       |
| CPU        | Intel(R) Core(TM) i7-11700                                |
| GPU        | AMD Radeon RX 570.                                        |
| Network    | Realtek PCIe 2.5Gb Ethernet (RTL8125)                     |                                                                           
| Disk       | SN750                                                     |
| Bootloader | OpenCore 0.7.5 Release                                    |

# 状态
 - Type-C USB2.3 Gen2x2 没测 
 - 第一次安装为了方便定制USB建议安装11.2 之后再OTA升级 否则请关闭`XhciPortLimit`
 - AppleALC修改过Controller.Plist(TigerLake PCH cAVs 43c8 ID Patch->IOServceStartPatch)
 - Wi-Fi 蓝牙 (没放驱动)
 - SMBIOS MacPro 7,1
 - 其他问题欢迎反馈
 # AppleALC
 - 针对 B560 有输出设备播放音视频进度条不动的修改版 AppleALC主要针对device-id 43C8 和 F0C8 (使用时有问题欢迎反馈😛)
 - 方法 2 无需使用Modified AppleALC 或者 FakePCIID 可尝试 注入 `device-id D07A0000 并搭配原版AppleALC Release 1.6.7或更高版本` 同时IceLake-LP 或者 Z490 H470 W480 Q470 等平台如果出现核显的核显数字音频(DP HDMI)无法使用也可尝试此方法 推荐！(如果无效请开 issues 报告实际情况)

## 鸣谢
- [Mieze](https://github.com/Mieze) 提供 [LucyRTL8125Ethernet](https://github.com/Mieze/LucyRTL8125Ethernet).
- [Acidanthera](https://github.com/acidanthera) 提供 [AppleALC](https://github.com/acidanthera/AppleALC), [RestrictEvents](https://github.com/acidanthera/RestrictEvents), [Lilu](https://github.com/acidanthera/Lilu), [OcBinaryData](https://github.com/acidanthera/OcBinaryData), [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg), [VirtualSMC](https://github.com/acidanthera/VirtualSMC) ,[WhateverGreen](https://github.com/acidanthera/WhateverGreen)

