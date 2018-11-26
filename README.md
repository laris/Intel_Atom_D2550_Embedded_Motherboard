# Intel Atom D2550 Motherboard

## Hardware PCBA review
### CPU - [D2550 Intel SPEC]( https://ark.intel.com/products/65470/Intel-Atom-Processor-D2550-1M-Cache-1-86-GHz-)
|Feature|Spec|Note|
|----|----|----|
|Product Collection|Intel® Atom™ Processor D Series|
Code Name|Cedarview
Launch Date|Q1'12
Cores|2
Threads|4
Processor Base Frequency|1.86 GHz
TDP|10W
Max Memory Size|4GB
Memory Types|DDR3 800/1066
Max # of Memory Channels|1
Max # of PCI Express Lanes|4
Turbo Boost|No
Hyper-Threading|Yes
Virtualization (VT-x)|No
Virtualization for Directed I/O (VT-d)|No
Intel 64|Yes
### HeatSink and Fan
* Active or passive heatsink
* 12v fan
### Memory DIMM
* DIMM Type: DDR3 
* Freqency: 1333/1066/800 MHz
* Module size: 1/2/4 GB
### Storage connection
* Standard SATA port
* Mini-PCIE SATA port
* SATA power connector
* 
### Network
* RTL8111E 
### Power supply
* DC 12v 5.5mm x 2.5mm Coaxial power connector
    * SPEC [Coaxial Power connector](https://en.wikipedia.org/wiki/Coaxial_power_connector)
    * Male: Receptacle/Jack/Socket/DC插头座 5.5x2.5mm
    ![](img/DC12v-Jack-physical.png)
    ![](img/DC12v-Jack-spec.png)
    * Female: Plug 
    ![](img/DC12v-plug-physical.jpg)
* ATX 20 x PIN 
    * SPEC: [20/24-pin ATX12V 2.x power supply connector + CPU P4 ](https://en.wikipedia.org/wiki/Power_supply_unit_(computer)#Wiring_diagrams)
    ![](img/ATX_24P_SPEC.png)
    ![](img/ATX_PINOUT_24P_4P.png)
* ATX 12v 2 x 4
### Peripherals 
* IT87 [IT8786E-I Datasheet](ds_it87_rs232/IT8786E.pdf)
* Serial/RS232 [MF243/MAX3243E](ds_it87_rs232/RS232_max3243e.pdf)
* LPT port
* USB 2.0
* USB 3.0

## Hack BIOS to enable 64-bit x86_64 OS support
### BIOS
### Check MSR config
* Refer post
![D2550 64-bit and VTx No](img/D2550_VTX_NO.jpg)
### IDA reverse engineering 
### Phonix packaging 
### Program/Flash BIOS

## OS
### Grub black screen issue
### Linux black screen issue
### OpenWRT x86_64 installation 
### Synology DSM

## TE7075M
* PCBA: TE7075M

## M7072
* System Spec/Manual: [TBE-M7072](TopStar-M7072-SPEC.md)
* PCBA image
![M7072-USB3-1](img/M7072_IMG_3025_small.jpg)
[M7072-USB3-1_Large](img/M7072_IMG_3025.jpg)
![M7072-USB3-2](img/M7072_IMG_3026_small.jpg)
[M7072-USB3-2_Large](img/M7072_IMG_3026.jpg)
* BIOS: SD-M7072-J


