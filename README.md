# Realtek Wireless Driver for Linux
v4.3.14_13455.20150212_BTCOEX20150128-51

## Supported chipsets
* RTL8192C
* RTL8192D
* RTL8723A
* RTL8188E
* RTL8812A (AC1200)
* RTL8821A (AC1200)
* RTL8192E
* RTL8723B

## How-To (general)

1. Select your chipset and platform in `Makefile`. For example:
  * Change ```CONFIG_RTL8821A = n``` to ```CONFIG_RTL8821A = y```
  * Change ```CONFIG_PLATFORM_I386_PC = n``` to ``` CONFIG_PLATFORM_I386_PC = y```
2. Uninstall the old driver if needed: `sudo modprobe -r [chipset_name]`, where `[chipset_name]` is `8821au` for instance.
3. `make`
4. `sudo make install`
5. `sudo modprobe [chipset_name]`

## Release notes

```
v4.3.14_13455.20150212_BTCOEX20150128-51
Realtek release:
1. This driver can support 8811AU and 8821AU
2. Support BT coexist
3. Support Adaptivity
4. Support efuse and mac address can read from file
5. Support Sniffer feature
6. Support Linux kernel 3.16.0
7. Fix some 802.11 logo issue
8. Fix WPS issue
```


