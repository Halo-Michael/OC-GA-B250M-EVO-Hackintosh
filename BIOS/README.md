bios.bin:  
此BIOS仅限GIGABYTE B250M-EVO主板配合Coffee Lake（8/9代）cpu使用，包含以下微码：U0步进：906EA（EC）、B0步进：906EB（EC）、P0步进：906EC（EC）、R0步进：906ED（EC）  
使用Coffee Lake cpu需要配合针脚屏蔽贴  
ME版本已降级至此主板配合Coffee Lake cpu最新可用版本11.7.0.1261，TPM2.0功能正常，支持Windows BitLocker自动解锁  
已做pcie总线修复、SKU修复、acpi表修复、8+线程cpu初始化修复、12/16线程cpu支持  
核显VBIOS版本更新至1062 GOP版本更新至9.0.1112 GOP VBT版本更新至228 有线网卡BIOS驱动版本更新至2.0.57  
将10+核cpu核心数使用十六进制显示改为使用十进制显示  
默认解锁CFG LOCK，添加CSM Support开关选项  
解锁温度墙，请注意VRMOS管温度  
移除Q-FLASH对BIOS文件的校验  
启动Logo更改为苹果Logo，默认分辨率1920x1080  
修复部分中文翻译错误问题  
不能配合笔记本/至强转针U使用

bios2.bin:  
在bios.bin文件更新的基础上：  
更新微码版本至：U0步进：906EA（F0）、B0步进：906EB（EC）、P0步进：906EC（F0）、R0步进：906ED（F0）  
SYSTEM FAN风扇接口更新温度来源为VRMOS管温度传感器  
注：未更新bios修改日期

bios3.bin:  
在bios2.bin文件更新的基础上：  
更新微码版本至：U0步进：906EA（F0）、B0步进：906EB（F0）、P0步进：906EC（F0）、R0步进：906ED（F0）  
注：未更新bios修改日期
