# Static Firmware Analysis

After saving the flash memory we are able to extract the file structure using the following command.

`binwalk -e KasaPTZFirmware.bin`

We then see files that support a wide variety of functionality.

## OpenWRT-Based Linux
- openwrt_version
- openwrt_release
- procd
- ubus, uci, netifd
- uClibc 1.0.31

## Realtek Wi-Fi
- rtl8188fu
- 8188fu.ko
- wirelessd

## Proprietary Components
- ucloud
- p2pd
- libtpcom.so
- libtpsocket.so
- libucloud.so
- cloud_mod
- cloud_upgrade
- cloud_reconnect

## Camera-Specific Functionality
- is_cal
- set_imageCtrl_dayNight
- firm_mac
- nvrammanager
- device_info
- hardware.txt

## Update/Recovery Infrastructure
- auto_upgrade
- update_firmware
- upgrade_prepare
- upgrade_recovery
- recover-manager
- prefetchfirm
- sysupgrade

## TLS Material
- uhttpd.crt
- uhttpd.key
- tp-link-CA.pem
- tpracloudca.pem

