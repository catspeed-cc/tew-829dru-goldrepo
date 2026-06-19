# TRENDnet tew-829dru goldsheet

Everything known about the TEW-829DRU before I half bricked it attempting to add OpenWRT support for this device.

## MANUFACTURER INFORMATION:
- TRENDnet main website can be accessed here: https://www.trendnet.com/home
- TRENDnet "provides their GPL source code" here: https://www.trendnet.com/support/gpl-source-codes.asp
- TRENDnet support system is here: https://www.trendnet.com/support/
- TRENDnet contact is here: https://www.trendnet.com/company/contact-us.asp
- TRENDnet TEW-829DRU https://www.trendnet.com/support/support-detail.asp?prod=100_TEW-829DRU
- FCC ID: XU8TEW829DRU [https://fccid.io/XU8TEW829DRU](https://fccid.io/XU8TEW829DRU)

## LEGAL DISCLAIMER:
This Device Tree Source (DTS) file was extracted from a router running firmware based on OpenWrt 15.05 (Chaos Calmer), which is licensed under the GNU General Public License version 2 (GPLv2).  As a derivative work of GPL-licensed software, the DTS file itself is covered by the GPLv2, granting the right to share and modify this source code; consequently, the hardware configuration described herein cannot be claimed as exclusive intellectual property by the manufacturer to restrict its distribution. 

This repository contains only the DTS source code to facilitate community assistance in unbricking the device; no proprietary binary blobs, compiled firmware, or executable images are included to ensure full compliance with intellectual property concerns and to avoid any potential license violations associated with binary redistribution.

## LICENSE:
These files were obtained from a device which runs firmware based on OpenWRT 15.05 (Chaos Chalmer) and as such are covered by the GPLv2 license. As a result I must provide a copy of the license for you (see LICENSE.md)<br />
<br />
Any additions or modifications made by myself will also be covered by the same GPLv2 license (see LICENSE.md)

## REPOSITORY FILES:
- [trendnet-tew-829dru-goldsheet.txt](https://github.com/catspeed-cc/tew-829dru/blob/master/trendnet-tew-829dru-goldsheet.txt) (current goldsheet)
- [spi-extracted.dts](https://github.com/catspeed-cc/tew-829dru/blob/master/spi-extracted.dts) (current running DTS from router SPI NOR - canonical single source of truth)
- [stock-fixed.dts](https://github.com/catspeed-cc/tew-829dru/blob/master/stock-fixed.dts)  (tew-829dru DTS from firmware image extraction - copy?)
- [trendnet_tew-829dru.dts](https://github.com/catspeed-cc/tew-829dru/blob/master/trendnet_tew-829dru.dts) (tew-829dru DTS from firmware image extraction)

## FOLLOW MY WORK ON TEW-829DRU:
You may follow my port of TEW-829DRU to OpenWRT by [visiting the repository](https://github.com/catspeed-cc/openwrt), [the DTS file](https://github.com/catspeed-cc/openwrt/blob/tew-829dru-25.12/target/linux/ipq40xx/files-6.12/arch/arm/boot/dts/qcom/qcom-ipq4019-tew-829dru.dts), [this support ticket](https://github.com/catspeed-cc/openwrt/issues/1) and [this pull request](https://github.com/catspeed-cc/openwrt/pull/5)

-----

## CATSPEED.CC COMMUNITY GPL CCS MIRROR:
I have taken the liberty to set up a GPL Complete Corresponding Source mirror, as I have the right to redistribute GPL software under GPLv2 license. This mirror will contain various manufacturers' GPLv2 Complete Corresponding Source for devices if provided via website such as - TRENDnet, TP-Link (soon)

I am doing so for a few reasons:
- I intend to port as many EOL devices as possible
- I want the source before TRENDnet starts deleting old EOL routers that have been EOL for over 3 years
- I can provide others free valuable archival services of TRENDnet GPL source code
- I intend to cross reference with CVE disclosures for specific hardware/software versions in future (useable in porting)

**MIRROR URLs:**
- Main mirror page - https://gpl-mirror.catspeed.cc/
- Main mirror directory - https://gpl-mirror.catspeed.cc/mirror/
- TRENDnet GPLv2 CCS mirror - https://gpl-mirror.catspeed.cc/mirror/trendnet/

**NOTE:** The archiver will run once weekly on Sunday at 0000 EST/EDT - it only downloads corrupted or missing files - based on SHA1 hashes. As the script is rate limiting itself to prevent damage to their infrastructure, it may take over night to complete. Should TRENDnet have issue with this and outright block my download attempts, in my opinion that would be a GPL violation. Rate limits I will accept to a degree, I understand the circumstances, hence why the script already rate limits itself.

-----

- For more information about catspeed.cc visit [https://catspeed.cc/](https://catspeed.cc/)
- For more information about OpenWRT visit [https://openwrt.org/](https://openwrt.org/)
- For more information about Software Freedom Conservancy visit [https://sfconservancy.org/](https://sfconservancy.org/)

-----

❤️ We support the work of the **Software Freedom Conservancy**, who fight to uphold GPL compliance so projects like this one remain possible.

  <a href="https://sfconservancy.org/sustainer/">
  <img src="https://sfconservancy.org/static/img/supporter-badge.png" width="194" height="90" alt="Become a Conservancy Sustainer!" border="0"/>
  </a>
