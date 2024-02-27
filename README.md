TWRP configuration for Samsung Galaxy A10s (a10s)
================================================================
 
Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Octa-core 2.0 GHz Cortex-A53
Chipset | Mediatek MT6762 Helio P22
GPU     | 650MHz PowerVR GE8320
Memory  | 2/3 GB
Shipped Android Version | 9 Pie with OneUI Core 1.0
Storage | 32 GB
MicroSD | Up to 256 GB
Battery | 3900 mAh (non-removable)
Dimensions | 156.9 x 75.8 x 7.8 mm (6.18 x 2.98 x 0.31 in)
Display | 720 x 1520 pixels, 6.2" PLS LCD, 19:9 ratio (~271 PPI density)
Rear Camera  | 13.0 MP + 2 MP, LED flash
Front Camera | 8.0 MP
Release Month | August 2019

Blocking checks
- [x] Correct screen/recovery size
- [x] Working Touch, screen
- [x] Backup to internal/microSD
- [x] Restore from internal/microSD
- [x] reboot to system
- [x] ADB

Medium checks
- [ ] update.zip sideload
- [ ] UI colors (red/blue inversions)
- [x] Screen goes off and on
- [x] F2FS/EXT4 Support, exFAT/NTFS where supported
- [x] all important partitions listed in mount/backup lists
- [x] backup/restore to/from external (USB-OTG) storage (not supported by the device)
- [x] backup/restore to/from adb (https://gerrit.omnirom.org/#/c/15943/)
- [ ] decrypt /data
- [x] Correct date

Minor checks
- [ ] MTP export
- [x] reboot to download
- [x] reboot to recovery
- [x] poweroff
- [x] battery level
- [x] temperature
- [x] encrypted backups
- [x] input devices via USB (USB-OTG) - keyboard, mouse and disks (not supported by the device)
- [x] USB mass storage export
- [x] set brightness
- [x] vibrate
- [x] screenshot
- [x] partition SD card

# How-to compile it:
```
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_a10s-eng
make recoveryimage

```

```
#
# Copyright (C) 2024 The Android Open Source Project
# Copyright (C) 2024 The TWRP Open Source Project
#
# SPDX-License-Identifier: Apache-2.0
#
```
