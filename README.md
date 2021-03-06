# OC-GA-B250M-EVO-Hackintosh

## 系统参数
| Name | Description |
| - | - |
| CPU | Intel 9th Gen Coffee Lake Core i5 - 9600K 3.70 GHz |
| 主板 | Gigabyte GA-B250M-EVO |
| 显卡 | Intel UHD Graphics 630 |
| 内存 | DDR4 2666 MHz 8G x2 |
| 硬盘 | SATA SSD 240G |
| 声卡 | Realtek HD Audio ALC 887 |
| 有线网卡 | Realtek RTL8168G |
| 无线网卡 | BCM4360 (14E4:43A0)  |
| 蓝牙 | BCM4360 (0A5C:22BE) |
| BIOS | AMI UEFI BIOS (Version F5d modified) |

## macOS & OpenCore 版本
- macOS Big Sur 11.6.5 / Monterey 12.4
- OpenCore 0.8.0

## BIOS 设置
- Hyper-Threading Technology : 启用
- Intel Speed Shift Technology : 启用
- Fast Boot : 禁用
- Windows 8/10 Features : Other OS
- Secure Boot : 禁用
- Serial Port : 禁用
- XHCI Hand-Off : 启用
- Port 60/64 Emulation : 启用
- SATA Mode : AHCI
- VT-d : 禁用
  - 如果OC中将 DisableIoMapper 设置为true，那么VT-d可以启用
- DVMT Pre-Allocated Memory : 32 MB
- CFG Lock : 禁用
- CSM Support : 禁用

## 工作的部件
- 自动变频 & 睿频（可通过Intel Power Gadget确认）
- 核显Intel UHD Graphics 630 通过DVI口正常输出（可转接HDMI）
- 核显H264 HEVC硬件解码正常工作（可通过VideoProc确认）
- 独立显卡已禁用，无需拔下
- 风扇控制、温度传感器 (可通过iStat确认)
- Nvme控制器、四SATA口工作正常
- 声卡Realtek ALC 887
- 苹果启动音效
- 内置千兆有线网卡Realtek RTL8168G
- 无线网卡BCM94360 2.4GHz、5GHz
- 蓝牙模块（仅在Monterey以下工作）
- 机箱后部4x USB3.0口 & 2x USB2.0口 & 内部USB3.0总线接前置1x USB3.0口 + 2x USB2.0口已定制好USBPort.kext
- 夜览模式
- 睡眠 & 唤醒
- 文件保险箱 （FileVault）
- 完整安全性（Full Security） & 个性化的苹果安全启动（Personalised Apple Secure Boot）
- 隔空投送（AirDrop）
- 隔空播放接收器（AirPlay to Mac）
- iMessage & FaceTime
