# TWRP device trees for WIKO T3 (W-V770) - 4GB RAM - 128GB ROM
# MTK Helio P35 - mt6765
## Specs => https://ru.wikomobile.com/m3410-wiko-t3
Component Type | Details
-------:|:-------------------------
Display: 6.6 in, IPS, 720 x 1600 pixels, 24 bit
OS| Android 11 - Soc: MediaTek Helio P35 - Platform: mt6765
RAM| 4 GB, 
Storage| 128 GB - USB: 2.0, USB Type-C - Memory cards: microSD, microSDHC, microSDXC
Battery| 5000 mAh, Li-Polymer
Bluetooth| 5.0 - Positioning: GPS, A-GPS, GLONASS, BeiDou, Galileo
SIM card| Nano-SIM - Wi-Fi: a, b, g, n, ac, Wi-Fi Hotspot, Wi-Fi Direct, Wi-Fi Display

### Blocking checks

- [ ] Correct screen/recovery size
- [ ] Working Touch, screen
- [ ] Backup to internal/microSD
- [ ] Restore from internal/microSD
- [ ] reboot to system
- [ ] ADB

### Medium checks

- [ ] update.zip sideload
- [ ] UI colors (red/blue inversions)
- [ ] Screen goes off and on
- [ ] F2FS/EXT4 Support, exFAT/NTFS where supported
- [ ] all important partitions listed in mount/backup lists
- [ ] backup/restore to/from external (USB-OTG) storage (not supported by the device) (not tested)
- [ ] [backup/restore to/from adb](https://gerrit.omnirom.org/#/c/15943/)
- [ ] decrypt /data
- [ ] Correct date

### Minor checks

- [ ] MTP export
- [ ] reboot to bootloader
- [ ] reboot to recovery
- [ ] poweroff
- [ ] battery level
- [ ] temperature
- [ ] encrypted backups (no option, need to test)
- [ ] input devices via USB (USB-OTG) - keyboard, mouse and disks (not supported by the device) (not tested)
- [ ] USB mass storage export (not tested)
- [ ] set brightness
- [ ] vibrate (Doesn't work, WIP)
- [ ] screenshot
- [ ] partition SD card

## Building

```bash
source build/envsetup.sh
lunch twrp_Armor_8-eng
mka bootimage
```

