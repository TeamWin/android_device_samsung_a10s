## Recovery Device Tree for the Samsung Galaxy A10s

## How-to compile it:

# Create dirs
$ mkdir tw; cd tw

# Init repo
$ repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-11

# Clone repo
$ git clone https://github.com/HayateDevTH/android_device_samsung_a10s -b android-11 device/samsung/a10s

# Sync
$ repo sync

# Run 
$ chmod +x device/samsung/a10s/mkbootimg to avoid building issues.

# Build
$ source build/envsetup.sh; export ALLOW_MISSING_DEPENDENCIES=true; lunch twrp_a10s-eng; mka recoveryimage
