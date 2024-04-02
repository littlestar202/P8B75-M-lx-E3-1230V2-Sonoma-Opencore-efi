## **ASUS-P8B75-M LX  hackintosh Sonoma**
## **本机配置**

| CPU | E3-1230V2 |
| --- | --- |
| 主板 | 华硕P8B75-M LX  |
| 内存 | 两条杂牌内存（8+8=16GB） |
| 主硬盘 | 东芝TR150（240G，SATA固态） |
| 核心显卡 | 无 |
| 独立显卡 | RX580 8G 2304SP 撼讯|
| 有线网卡 | Realtek8111千兆内置卡 |
| 无线网卡 | AX210 (博通的网卡应该也能驱动) |
| 声卡 | 威盛VIA VT1708S  |

# **截图**

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
测试在Sonoma14.4.1正常运行 请修改三码后使用

##  声卡还不够完善 这种声卡挺头大的 只能万能声卡驱动 
目前只测试了机箱后面主板上的插孔 前置机箱未测试

## 注意⚠️！！！
需要把OC/kext中的万能声卡驱动VoodooHDA.kext复制到S/E下重建缓存才能驱动

## **差不多配置的主机 声卡是ALC系列请删除万能声卡VoodooHDA.kext和AppleHDADisabler.kext 改用AppleALC.kext自行搜索后注入声卡ID 配置文件也别忘了改**

# 开机紫屏请下载   **紫屏注入EDID.zip** 详细操作请查看紫屏帮助.txt

# 出现开机第二屏死机 或者进系统死机的请把启动参数添加-amd_no_dgpu_accel
然后使用OCLP装完驱动后再去掉-amd_no_dgpu_accel即可正常
