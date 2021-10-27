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
 - AppleALC修改过Controller.Plist(TigerLake PCH cAVs 43c8 ID Patch->IOServceStartPatch)建议别更新后期维护会跟进
 - Wi-Fi 蓝牙 (没放驱动)
 - SMBIOS MacPro 7,1
 - 其他问题欢迎反馈
 # AppleALC
 - 针对 B560 有输出设备播放音视频进度条不动的修改版 AppleALC主要针对device-id 43C8 和 F0C8 实时跟进版本(使用时有问题欢迎反馈😛)
