根据启动时显示Logo分辨率的不同，有两种BIOS文件可供选择：4:3及16:9。两文件夹下同名文件除了Logo分辨率不同外没有任何区别。一般来说CSM启动倾向于使用4:3分辨率显示Logo，UEFI启动倾向于使用16:9显示Logo。但是如果你使用核显，那么即使是UEFI启动仍然可能使用4:3比例。  
由于符号“:”不能作为文件名，使用符号“x”代替。  
如果你刷入了了4x3下BIOS文件启动时Logo偏长，请改用16x9下同名BIOS文件；如果你刷入了了16x9下BIOS文件启动时Logo偏扁，请改用4x3下同名BIOS文件。

bios.bin:  
由官方BIOS版本F5d修改而来，更改版本号为F6，更改编译时间为2022/12/9 8:30  
此BIOS仅限GIGABYTE B250M-EVO主板配合Coffee Lake（8/9代）cpu使用，包含以下微码：U0步进：906EA（F0）、B0步进：906EB（F0）、P0步进：906EC（F0）、R0步进：906ED（F4）  
使用6/7代CPU禁止使用这些BIOS，刷入会导致不开机  
使用非B0步进Coffee Lake CPU需要配合针脚屏蔽贴  
ME版本已降级至此主板配合Coffee Lake cpu最新可用版本11.7.0.1261，TPM2.0功能正常，支持Windows BitLocker自动解锁  
已做pcie总线修复、SKU修复、acpi表修复、8+线程cpu初始化修复、DSSP未定义修复、12/16线程cpu支持，me启动校验移除  
核显VBIOS版本更新至1062 GOP版本更新至9.0.1112 GOP VBT版本更新至228 有线网卡BIOS驱动版本更新至2.0.59  
SYSTEM FAN风扇接口更新温度来源为VRMOS管温度传感器  
将10+核cpu核心数使用十六进制显示改为使用十进制显示  
默认解锁CFG LOCK，强制显示CSM Support开关选项  
解锁CPU温度墙开关选项（在CPU超频进阶设置内，默认为开启），关闭VRMOS温度墙，请注意VRMOS管温度  
移除Q-FLASH对BIOS文件的校验  
Q-FLASH增加NTFS分区支持  
启动Logo更改为苹果Logo  
修复部分中文翻译错误问题  
修复部分BIOS错误  
不能配合笔记本/至强转针U使用

bios-safe.bin:  
在bios.bin文件更新的基础上：  
回锁VRMOS温度墙的安全版本
