# OPENCORE-i5-8400-Gigabyte-B360M-Aorus-Gaming3

## Specs
```
Processor : Intel Core i5-8400 (Coffee Lake) 

Motherboard : Gigabyte B360M Aorus Gaming 3

Ram: 16GB 2666mhz

SSD : Zotac 120GB, Crucial MX500 500GB

Hard Drive: Seagate 2TB Hard Drive

Internal Graphics : Intel UHD Graphics 630 2048 MB

External Grapics : Gigabyte GTX 1050 ti (Disabled in MacOs 11 Big Sur)

WIFI & Bluetooth : Intel AC 9560

Ethernet : Intel I219V7 PCI Express Gigabit- Ethernet
```

## Software
- OpenCore 0.9.3 (Supported up to Ventura)
- macOS Big Sur 11.2

## BIOS Setting
### Disable
```
* Fast Boot
* Secure Boot
* Serial/COM Port
* VT-d
* Intel Platform Trust

```
### Enable
```
* Above 4G decoding
* Hyper-Threading
* EHCI/XHCI Hand-off
* DVMT Pre-Allocated(iGPU Memory): 64MB
* SATA Mode: AHCI
```
## Change Serial,MLB,SMUUID

At first download GenSMBIOS tool from [here.](https://github.com/corpnewt/GenSMBIOS)

Then extract it & Open-> GenSMBIOS.command

#### 1. Select option :3

#### 2. type: iMac19,1

#### 3. Copy the Serial, Board Serial & SmUUID

#### 4. Open EFI->OC->config.plist then Replace it with your generated SMBIOS
```
Serial -> SystemSerialNumber
Board Serila -> MLB
SmUUID ->SystemUUID
```
