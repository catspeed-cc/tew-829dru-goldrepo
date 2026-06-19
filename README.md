# tew-829dru

Everything known about the TEW-829DRU before I half bricked it attempting to add OpenWRT support for this device.

### DISCLAIMER: This Device Tree Source (DTS) file was extracted from a router running firmware based on OpenWrt 15.05 (Chaos Calmer), which is licensed under the GNU General Public License version 2 (GPLv2).  As a derivative work of GPL-licensed software, the DTS file itself is covered by the GPLv2, granting the right to share and modify this source code; consequently, the hardware configuration described herein cannot be claimed as exclusive intellectual property by the manufacturer to restrict its distribution. 

This repository contains only the DTS source code to facilitate community assistance in unbricking the device; no proprietary binary blobs, compiled firmware, or executable images are included to ensure full compliance with intellectual property concerns and to avoid any potential license violations associated with binary redistribution.

- TRENDnet main website can be accessed here: https://www.trendnet.com/home
- TRENDnet "provides their GPL source code" here: https://www.trendnet.com/support/gpl-source-codes.asp
- TRENDnet support system is here: https://www.trendnet.com/support/
- TRENDnet contact is here: https://www.trendnet.com/company/contact-us.asp

### UNOFFICIAL PUBLIC GPL SOURCE MIRROR
I have taken the liberty to set up a GPL source mirror, as I have the express right to redistribute GPL software under GPLv2 license. This mirror will contain various manufacturers' GPLv2 source for devices if provided via website such as - TRENDnet, TP-Link (soon)

I am doing so for a few reasons:
- I intend to port as many EOL devices as possible
- I want the source before TRENDnet starts deleting old EOL routers that have been EOL for over 3 years
- I can provide others free valuable archival services of TRENDnet GPL source code
- I intend to cross reference with CVE disclosures for specific hardware/software versions in future (useable in porting)

**MIRROR URLs:**
- Main mirror page - https://gpl-mirror.catspeed.cc/
- Main mirror directory - https://gpl-mirror.catspeed.cc/mirror/
- TRENDnet GPLv2 CCS mirror - https://gpl-mirror.catspeed.cc/mirror/trendnet/

**NOTE:** The archiver will run once weekly on Sunday at 0000 - it only downloads corrupted or missing files - based on SHA1 hashes. As the script is rate limiting itself to prevent damage to their infrastructure, it may take over night to complete. Should TRENDnet have issue with this and outright block my download attempts, that would be a GPL violation in my opinion. Rate limits I will accept to a degree, I understand the circumstances, hence why the script already rate limits itself.

### REPOSITORY FILES:
- [trendnet-tew-829dru-goldsheet.txt](https://github.com/catspeed-cc/tew-829dru/blob/master/trendnet-tew-829dru-goldsheet.txt) (current goldsheet)
- [spi-extracted.dts](https://github.com/catspeed-cc/tew-829dru/blob/master/spi-extracted.dts) (current running DTS from router SPI NOR - canonical single source of truth)
- [stock-fixed.dts](https://github.com/catspeed-cc/tew-829dru/blob/master/stock-fixed.dts)  (tew-829dru DTS from firmware image extraction - copy?)
- [trendnet_tew-829dru.dts](https://github.com/catspeed-cc/tew-829dru/blob/master/trendnet_tew-829dru.dts) (tew-829dru DTS from firmware image extraction)

### You may follow my port of TEW-829DRU to OpenWRT by [visiting the repository](https://github.com/catspeed-cc/openwrt), [the DTS file](https://github.com/catspeed-cc/openwrt/blob/tew-829dru-25.12/target/linux/ipq40xx/files-6.12/arch/arm/boot/dts/qcom/qcom-ipq4019-tew-829dru.dts) and [this support ticket](https://github.com/catspeed-cc/openwrt/issues/1)

### For more information about OpenWRT [visit their website](https://openwrt.org/)



#### ERASE BELOW
ical eraseblock size:    126976 bytes
UBI: smallest flash I/O unit:    2048
UBI: VID header offset:          2048 (aligned 2048)
UBI: data offset:                4096
UBI: attached mtd2 to ubi0
UBI: MTD device name:            "mtd=0"
UBI: MTD device size:            48 MiB
UBI: number of good PEBs:        384
UBI: number of bad PEBs:         0
UBI: max. allowed volumes:       128
UBI: wear-leveling threshold:    4096
UBI: number of internal volumes: 1
UBI: number of user volumes:     2
UBI: available PEBs:             185
UBI: total number of reserved PEBs: 199
UBI: number of PEBs reserved for bad PEB handling: 3
UBI: max/mean erase counter: 4/3
Read 0 bytes from volume kernel to 84000000
No size specified -> Using max size (3809280)
## Booting kernel from FIT Image at 84000000 ...
   Using 'config@ap.dk07.1-c1' configuration
   Trying 'kernel@1' kernel subimage
	 Description:  ARM OpenWrt Linux-3.14.43
	 Type:         Kernel Image
	 Compression:  gzip compressed
	 Data Start:   0x840000e4
	 Data Size:    3361261 Bytes = 3.2 MiB
	 Architecture: ARM
	 OS:           Linux
	 Load Address: 0x80208000
	 Entry Point:  0x80208000
	 Hash algo:    crc32
	 Hash value:   455baf05
	 Hash algo:    sha1
	 Hash value:   815ee16957306915e27edd00aa3f66ef979b805b
   Verifying Hash Integrity ... crc32+ sha1+ OK
## Flattened Device Tree from FIT Image at 84000000
   Using 'config@ap.dk07.1-c1' configuration
   Trying 'fdt@ap.dk07.1-c1' FDT blob subimage
	 Description:  ARM OpenWrt qcom-ipq40xx-ap.dkxx device tree blob
	 Type:         Flat Device Tree
	 Compression:  uncompressed
	 Data Start:   0x8436c2f8
	 Data Size:    37922 Bytes = 37 KiB
	 Architecture: ARM
	 Hash algo:    crc32
	 Hash value:   b448c7b5
	 Hash algo:    sha1
	 Hash value:   c2130265a9512115b7a12df0207d3b0f268068f2
   Verifying Hash Integrity ... crc32+ sha1+ OK
   Booting using the fdt blob at 0x8436c2f8
   Uncompressing Kernel Image ... OK
   Loading Device Tree to 86ff3000, end 86fff421 ... OK
eth0 MAC Address from ART: 3c:8c:f8:f3:96:b2
eth1 MAC Address from ART: 3c:8c:f8:f3:96:b4
eth2 MAC Address from ART: 3c:8c:f8:f3:96:b3
Using machid 0x8010006 from environment

Starting kernel ...


					  #####################
					  ## CALDATA PACKING ##
					  #####################

These are the board-2.json files I used (named differently)

This is only required for developers porting devices, the average user will not have to do any of this process.
This is mainly documentation for myself.

What is important here is the overall structure, and the `names` field. Copy it exactly.
The filenames are irrelevant. Yours may be different. Just rename or replace them.

qca4019-artcaldata.json
###
[
  {
	"names": ["bus=ahb,bmi-chip-id=0,bmi-board-id=28,variant=TEW-829DRU-2G"],
	"data": "cal-ahb-0-fresh.bin"
  },
  {
	"names": ["bus=ahb,bmi-chip-id=0,bmi-board-id=30,variant=TEW-829DRU-5G"],
	"data": "cal-ahb-1-fresh.bin"
  }
]
###

qca9984-artcaldata.json
###
[
	{
		"names": [
			"bus=pci,bmi-chip-id=0,bmi-board-id=1"
		],
		"data": "cal-pci-fresh.bin"
	}
]
###

The commands to run to build the bin file:
###
# CREATE BOARD-2.BIN (QCA9984)
qca-swiss-army-knife/tools/scripts/ath10k/ath10k-bdencoder -c qca9984-artcaldata.json -o qca9984-artcaldata.bin
qca-swiss-army-knife/tools/scripts/ath10k/ath10k-bdencoder -c qca9984-boardData.json -o qca9984-boardData.bin

# EXTRACT BOARD-2.BIN - INSIDE tmp/ (QCA9984)
qca-swiss-army-knife/tools/scripts/ath10k/ath10k-bdencoder -e ../../qca9984-artcaldata.bin
qca-swiss-army-knife/tools/scripts/ath10k/ath10k-bdencoder -e ../../qca9984-boardData.bin

# CREATE BOARD-2.BINS (QCA4019)
qca-swiss-army-knife/tools/scripts/ath10k/ath10k-bdencoder -c qca4019-artcaldata.json -o qca4019-artcaldata.bin
tools/qca-swiss-army-knife/tools/scripts/ath10k/ath10k-bdencoder -c qca4019-boardData.json -o qca4019-boardData.bin

# EXTRACT BOARD-2.BIN - INSIDE tmp/ (QCA4019)
qca-swiss-army-knife/tools/scripts/ath10k/ath10k-bdencoder -e ../qca4019-artcaldata.bin
qca-swiss-army-knife/tools/scripts/ath10k/ath10k-bdencoder -e ../qca4019-boardData.bin
###

You can make a tmp/ directory, enter it, and run the extraction command in order to extract it back into a board-2.json and the original bin file(s)

Should the JSON look correct (has both entries if there are two) and there are all bin files present (with different names is ok) then you completed a "round trip".

The files are ready for insertion into your dev environment and to be built into the image.
```
