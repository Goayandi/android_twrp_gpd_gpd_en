GPD XD Plus
===============
```
By : Goayandi
```
![GPD XD Plus](https://www.zapals.com/media/catalog/product/cache/1/image/ae5fcc3175343e35bab9cec427611d29/g/p/gpd_xd_plus_5-inch_android7.0_game_tablet_with_bluetooth_4gb_ram_32gbrom_zp3020820510005_1_.jpg)

The XD Plus (codename _"gpd_en"_) is a portable gaming device from GPD.

This is a Minimal Device Tree for building TWRP for GPD XD Plus (Codename: gpd_en). I used TWRP by multirom and TWRP for Asus Zenpad 3S 10 from rakomancha to finally build a working tree for GPD XD Plus.

Basic        | Spec Sheet
------------:|:------------------------
CPU          | Cortex-A72 & Cortex-A53 | Hexa-Core | MT8176
GPU          | PowerVR GX6250
Memory       | 4GB RAM
Shipped Android Version | 7.0
Storage      | 32GB
Battery      | 6000 mAh Li-Po
Display      | 5,0
Rear Camera  | none
Front Camera | none


This branch is for building TWRP.

### Thanks to:
 * Team M.A.D
 * rakomancha

### To build: 
```

$ repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

To initialize a shallow clone, which will save even more space, use a command like this:

$ repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

After that sync your sources:

$ repo sync

Build your recovery:

$ source build/envsetup.sh

& lunch gpd_en-eng

make clean && make recoveryimage
```
