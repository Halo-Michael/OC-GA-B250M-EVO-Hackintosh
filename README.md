# OC-GA-B250M-EVO-Hackintosh

## 系统参数
| Name | Description |
| - | - |
| CPU | Intel 7th Gen Kaby Lake Core i7 - 7700 3.60 GHz |
| 主板 | Gigabyte GA-B250M-EVO |
| 显卡 | Intel HD Graphics 630 |
| 内存 | DDR4 2400 MHz 8G x2 |
| 硬盘 | SATA SSD 240G |
| 声卡 | Realtek HD Audio ALC 887 |
| 有线网卡 | Realtek RTL8111 & ASIX AX88179 |
| 无线网卡 | BCM94360 (14E4:43A0)  |
| 蓝牙 | BCM94360 (0A5C:22BE) |
| BIOS | AMI UEFI BIOS (Version F5d) |

## macOS & OpenCore 版本
- macOS Big Sur 11.5.1
- OpenCore 0.7.2

## BIOS 设置
- Hypet-Threading Technology : 启用
- Intel Speed Shift Technology : 启用
- Fast Boot : 禁用
- OS Type : Other
- Secure Boot : 禁用
- Serial(COM) Port : 禁用
- Parallel Port : 禁用
- XHCI Hand-Off : 启用
- Port 60/64 Emulation : 禁用
- SATA Mode : AHCI
- VT-d : 禁用
  - 如果OC中将 DisableIoMapper 设置为true，那么VT-d可以启用
- DVMT Pre-Allocated Memory : 128 MB
- CFG Lock : 禁用 (需要自行使用EFI系统禁用)

## 工作的部件
- 自动变频 & 睿频（可通过Intel Power Gadget确认）
- 核显Intel HD Graphics 630 通过DVI口正常输出(可转接HDMI)
- 独立显卡已禁用，无需拔下
- 风扇控制、温度传感器 (可通过iStat确认)
- Nvme控制器、四SATA口工作正常
- 声卡Realtek ALC 887
- 苹果启动音效
- 内置千兆有线网卡Realtek RTL8111 & 外置USB3.0千兆有线网卡ASIX AX88179
- 无线网卡BCM94360 2.4GHz、5GHz、蓝牙模块
- 机箱后部4x USB3.0口 & 2x USB2.0口 & 内部USB3.0总线接前置1x USB3.0口 + 2x USB2.0口已定制好USBPort.kext
- 夜览模式
- 睡眠 & 唤醒
- 文件保险箱 （FileVault）
- 完整安全性（Full Security） & 个性化的苹果安全启动（Personalised Apple Secure Boot）
- 隔空投送（AirDrop）
- iMessage & FaceTime
