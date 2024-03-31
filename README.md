## **ASUS-P8B75-M LX  hackintosh Sonoma**
## **本机配置**

| CPU | E3-1230V2 |
| --- | --- |
| 主板 | 华硕P8B75-M LX  |
| 内存 | 两条深圳产杂牌内存（8+8=16GB） |
| 主硬盘 | 东芝TR150（240G，SATA固态） |
| 核心显卡 | 无 |
| 独立显卡 | RX580 8G 2304SP 撼讯|
| 有线网卡 | Realtek8111千兆内置卡 |
| 无线网卡 |  AX210  |
| 声卡 | 威盛VIA VT1708S  |

![](https://github.com/littlestar202/P8B75-M-lx-E3-1230V2-Sonoma-opencore/blob/main/picture/9E110D5EDCCAC9A6783BD80F481C3BE3.png)
![](https://github.com/littlestar202/P8B75-M-lx-E3-1230V2-Sonoma-opencore/blob/main/picture/0D587B1204F5F85C4AD575915009056B.png)
![](https://github.com/littlestar202/P8B75-M-lx-E3-1230V2-Sonoma-opencore/blob/main/picture/7C42A266A5CF5250ECB4C2D05C6E51B9.png)
## BIOS 配置

请在高级模式（advanced mode）下配置

### **高级页面**
处理器设置-开启超线程、Intel虚拟技术

南桥-关闭intel快速启动、intel智能连接
 
 **SATA** 设置 
****SATA**** 模式选择： ****AHCI**** 

北桥-内存重寻址功能（above 4g）：开启

USB设置-intel xhci 模式：开启

高级电源管理（APM）：全部关闭

### **启动页面**

快速启动：关闭

CSM：关闭（如果显卡BIOS不支持UEFI则无法关闭）

## **目前工作情况**
测试在Sonoma14.4.1正常运行

##  声卡还不够完善 这种声卡挺头大的 只能万能驱动 
目前只测试了机箱后面主板上的插孔 前置机箱未测试
