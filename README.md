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

## Features

**Works**

- ADB
- Booting (Tested on Android 9 and Android 11)
- Brightness adjust
- **Decryption** (Stock Rom & Custom Rom & GSI is also supported!)
- MTP
- Vibration

**Not Works**
- ADB Sideload

## How To Compile

# Create dirs
```
mkdir twrp; cd twrp
```

## Init repo
```
repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-11
```

## Clone repo
```
git clone https://github.com/HayateDevTH/android_device_samsung_a10s -b android-11 device/samsung/a10s
```
## Sync
```
repo sync
```

## Run This Command For Fix Permission denied
```
chmod +x device/samsung/a10s/mkbootimg
```

## Build
```
source build/envsetup.sh; export ALLOW_MISSING_DEPENDENCIES=true; lunch twrp_a10s-eng; mka recoveryimage
```
