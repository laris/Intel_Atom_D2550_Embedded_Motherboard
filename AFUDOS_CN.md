AFUDOSU.EXE  %1  /P  /B  /N  /K  /R /FDT /MER /OPR

- /O		Save current ROM image to file     
- /S  		Display current system's ROMID    
- /D		Verification test of given ROM File without flashing BIOS.

- /P  		Program Main BIOS                                         
- /B  		Program Boot Block                                        
- /N  		Program NVRAM                 
- /K  		Program all non-critical blocks.

- /R  		Preserve ALL SMBIOS structure during programming          


- /X  		Don't Check ROM ID                                        
- /REBOOT  	Reboot after programming.                                 
- /SHUTDOWN  	Shutdown after programming.  




http://blog.sina.com.cn/s/blog_813e14e70100wdby.html

超微主板BIOS 升级工具AFUDOS 命令参数的含义？ (2011-07-21 12:09:53)
标签： 杂谈	分类： 主板产品
Q:超微主板BIOS 升级工具 AFUDOS  命令参数的念义？ 如，/P /B /N /C /R /REBOOT /X

 

A:/P Program main bios image             （刷BIOS主程序块）
 /B Program Boot Block                  （刷新BOOT块）
 /N Program NVRAM                       （刷新NVRAM)
 /C Destroy CMOS after update BIOS done  (刷新BIOS后清除CMOS数据)
  /REBOOT Reboot after update BIOS done   (升级完后)

 /X Do not check ROM ID                   (不检查ROM ID号)    

  /R Preserve all SMBIOS structures during NVRAM  programming    (NVROM 中保留SMBIOS结构)


http://blog.chinaunix.net/uid-21354120-id-3198033.html

AFUDOS AMI BIOS DOS下刷写参数
 分类： IT业界2012-05-05 22:35:34
命令行模式的用法和示例（AFUDOS 和 AFUWIN）：
注意：许多选项是高级的，使用不当可能会损害您的系统。

+---------------------------------------------------------------------------+
|                   AMI Firmware Update Utility  Ver.4.xx                   |
|      Copyright (C)2007 American Megatrends Inc. All Rights Reserved.      |
+---------------------------------------------------------------------------+
| 用法: AFUWIN [选项 1] [选项 2]...                            |
|           或                                                              |
|        AFUWIN <输入或输出文件名> <命令>                                   |
|           或                                                              |
|        AFUWIN <命令>                                                      |
| ------------------------------------------------------------------------- |
| 命令:                                                                     |
|         /O - 保存当前 BIOS 到文件                                         |
|         /U - 显示 ROM 文件的 ROMID                                        |
|        /Ln - 参考选项: /Ln                                                |
|         /M - 参考选项: /M                                                 |
|       /MAI - 显示系统 ROM 和 ROM 文件的 MA 信息                           |
|     /HOLE: - 根据给出的名称更新具体的保留区 ROMHole                       |
|              NewRomHole1.BIN /HOLE:RomH1                                  |
|  /HOLEOUT: - 根据给出的名称保存具体的保留区 ROMHole                       |
|              NewRomHole1.BIN /HOLE:RomH1                                  |
|         /D - 不刷写 BIOS 情况下，验证测试给出的 ROM 文件                  |
|        /EC - 刷写嵌入式控制器 EC 固件 BIOS（参考 OFBD 说明）              |
|       /NCB - 刷写非关键块 NCB 区域（参考 OFBD 说明）                      |
|    /NCBOUT - 根据给出的名称输出 NCB 数据                                  |
| 选项:                                                                     |
|         /P - 刷写 BIOS 主程序映像                                         |
|         /B - 刷写引导块 BootBlock                                         |
|         /N - 刷写非易失随机访问存储器 NVRAM                               |
|         /C - 清除 CMOS 校验和                                             |
|         /E - 刷写嵌入式控制器 EC 块                                       |
|         /K - 刷写所有非关键块 NCB                                         |
|        /Kn - 仅刷写第n个非关键块 NCB（n=0-7）                             |
|         /Q - 静默执行                                                     |
|    /REBOOT - 刷写后重新启动                                               |
|         /X - 强制刷写，不检查 ROM ID                                      |
|         /S - 显示当前系统的 ROMID                                         |
|        /Ln - 加载 CMOS 默认值: （n=0-3）                                  |
|              L0: 加载当前优化值 Load current optimal                      |
|              L1: 加载当前安全值 Load current failsafe                     |
|              L2: 从 ROM 文件加载优化值                                    |
|              L3: 从 ROM 文件加载安全值                                    |
|         /M - 更新引导块 Bootblock MAC 地址（若存在）                      |
|              示例: /M1234ABCD 将更新 MAC 为 1234ABCD                      |
|         /R - 在 NVRAM 刷写时保留所有 SMBIOS 结构                          |
|      /ECUF - 发现新版本时更新嵌入式控制器 EC BIOS                         |
|  /SHUTDOWN - 刷写后关机           