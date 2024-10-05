![OFRP](https://i.ibb.co/4WgF7pR/banner-2.png "OFRP")
# TWRP/OFRP device trees for WIKO T3 (W-V770)

## Device specifications

| Feature     | Specification
| :-----------|:-------------
| Chipset     | Mediatek MT6765 Helio P35 (12 nm)
| CPU         | Octa-core (4x2.3 GHz Cortex-A53 & 4x1.8 GHz Cortex-A53)
| GPU         | PowerVR GE8320 (680 Mhz)
| Memory      | 4 GB LPDDR3/LPDDR4x RAM
| Storage     | 128 GB (EMMC 5.1)
| SIM         | Hybrid SIM (Nano-SIM, dual stand-by)
| Battery     | Li-Ion 5000 mAh, non-removable
| Shipped OS  | Android 11.0
| Dimensions  | 165.3 x 76 x 9.2 mm (6.51 x 2.99 x 0.36 in)
| Display     | 6.6", 720x1600 pixels, IPS LCD, 60Hz
| Camera      | 48 MP (main), 5 MP (ultrawide), 2 MP (macro), 8 MP (front)
| Comms       | GSM/HSPA/LTE, Wi-Fi 802.11 b/g/n, Bluetooth 5.0 A2DP LE
| Sensors     | Fingerprint (side-mounted), accelerometer, proximity

## Device picture

![Wiko T3](https://fdn2.gsmarena.com/vv/bigpic/wiko-t3.jpg)

## Building

```bash
source build/envsetup.sh
lunch twrp_W_V770-eng
mka adbd bootimage
```

