# EFI for Hackintosh on ASUS ROG Z390-I Gaming / AMD RX 580 GPU / 1820A Wifi

Everything is working on Catalina with both Clover and OpenCore
- You need to generate your own UUID/Serial #will add how soon#
- The opencore EFI works with Big Sur, including WIFI/Bluetooth. But not continuity.

## Hardware

- COUGAR QBX Black Mini-ITX Ultra-Compact Pro Gaming Case
- ASUS ROG Z390-I Gaming
- Inter Core i7-9700K
- Radeon Shapphie Pulse RX 580
- Dell VW3T3 WLAN DW 1820A Wifi (onboard replacement)
- 2 x Crucial Ballistix Sport LT 3000 MHz DDR4 DRAM 8GB
- Samsung 970 EVO NVMe M.2 SSD 1TB / Samsung 850 EVO NAND SSD 500G / Crucial MX300 280GB
- Corsaire SF 450 / SFX to ATX Power supply adapter
- CPU Fan - NH-U9S - Only one that can cool down that CPU in that small case
- Case Fan - NF-A9
- 3 Dell Monitor (2DP + DVI) + HDMI to TV

<details>
<summary>COUGAR QBX Case Photos</summary>

![Tiny case](images/emptycase/IMG_5383.JPG "Tiny case")
![Tiny case](images/emptycase/IMG_5384.JPG "Tiny case")
![Tiny case](images/emptycase/IMG_5385.JPG "Tiny case")
![Front USB](images/emptycase/IMG_5386.JPG "Tiny case")
![Left side](images/emptycase/IMG_5393.JPG "Left side")
![SSD Access left side](images/emptycase/IMG_5394.JPG "SSD Access left side")
![Inside access left side](images/emptycase/IMG_5395.JPG "Inside access left side")
![Inside](images/emptycase/IMG_5396.JPG "Inside")
![Original fan](images/emptycase/IMG_5397.JPG "Original fan")
![SSD Panel](images/emptycase/IMG_5402.JPG "SSD Panel")
![HDD/SSD mount](images/emptycase/IMG_5403.JPG "HDD/SSD mount")
![Right side / cable management](images/emptycase/IMG_5407.JPG "Right side / cable management")
![Right side / other SSD mount](images/emptycase/IMG_5408.JPG "Right side / other SSD mount")
![SSD or Front optique drive mount](images/emptycase/IMG_5409.JPG "SSD or Front optique drive mount")
![SSD or Front optique drive mount](images/emptycase/IMG_5412.JPG "SSD or Front optique drive mount")
![Sliding top panel - Optique drive access](images/emptycase/IMG_5413.JPG "Sliding top panel - Optique drive access")
![PSU and adapter](images/emptycase/IMG_5425.JPG "PSU and adapter")
![SFX to ATX Power supply](images/emptycase/IMG_5427.JPG "SFX to ATX Power supply")

</details>

<details>
<summary>Build Photos</summary>

![Open COUGAR QBX with SSD side panel](images/case/Open_COUGAR_QBX.JPG "Open COUGAR QBX with SSD side panel")
![CPU Fan NH-U9S](images/case/Packed.JPG "Massive CPU Fan NH-U9S")
![SSD Panel in place](images/case/SSD_Panel.JPG "SSD Panel in place")
![Front](images/case/Hackintosh.JPG)
![Back 2DP + DVI + HDMI to DV](images/case/Back_Case.JPG "Back 2DP + DVI + HDMI to DV")
![Overall view](images/case/Side_Case.JPG)

</details>

<details>
<summary>Dell VW3T3 WLAN DW 1820A Wifi onboard replacement</summary>

![1820A WIFI/BT card](images/1820a/IMG_5481.jpg)
![Need to remove the cpu cooler](images/1820a/IMG_5490.JPG)
![Top right is the original WIFI](images/1820a/IMG_5491.JPG)
![WIFI removed](images/1820a/IMG_5492.JPG)
![Original wifi card](images/1820a/IMG_5494.JPG "Original wifi card")
![Reconnected WIFI antenna](images/1820a/IMG_5497.JPG "1820A WIFI")

</details>

## What works

All of Continuity

<details>
<summary>Service detail</summary>

- Handoff
- iMessage
- Continuity Camera
- Universal Clipboard
- Instant Hotspot
- Air Drop
- iPhone Cellular Calls
- Auto Unlock
- Apple Pay

</details>

- Sleep (fans and RGB LEDs included)
- Power Nap (sleep with background operations such as Time Machine)
- Wake
- Audio (select internal speakers)
- Ethernet - Bluetooth - WiFi
- All USB and USB 3.1 ports - Port mapping for the case
- Nightshift (no kexts required)

## USBMap

My case has 2 front USB 3.1 Gen 1 and I'm not using usb c.
With the 15 ports limit, here what I chose:

| Ports | Type | Description |
| --- | --- | --- |
| HS03 | USB 2 Standard-A connector | Rear USB 3.1 Gen 2 (red) |
| HS04 | USB 2 Standard-A connector | Rear USB 3.1 Gen 2 (red) |
| HS06 | USB 2 Standard-A connector | Rear USB 2.0 (black) |
| HS07 | USB 2 Standard-A connector | Rear USB 3.1 Gen 1 (blue) |
| HS08 | USB 2 Standard-A connector | Rear USB 3.1 Gen 1 (blue) |
| HS09 | USB 2 Standard-A connector | Front USB 3.1 Gen 1 |
| HS10 | USB 2 Standard-A connector | Front USB 3.1 Gen 1 |
| HS13 | Internal connector | Aura Motherboard |
| HS14 | Internal connector | Bluetooth/Wifi - DELL DW1820 (BCM4350) 802.11ac |
| SS03 | USB 3 Standard-A connector | Rear USB 3.1 Gen 2 (red) |
| SS04 | USB 3 Standard-A connector | Rear USB 3.1 Gen 2 (red) |
| SS07 | USB 3 Standard-A connector | Rear USB 3.1 Gen 1 (blue) |
| SS08 | USB 3 Standard-A connector | Rear USB 3.1 Gen 1 (blue) |
| SS09 | USB 3 Standard-A connector | Front USB 3.1 Gen 1 |
| SS10 | USB 3 Standard-A connector | Front USB 3.1 Gen 1 |

