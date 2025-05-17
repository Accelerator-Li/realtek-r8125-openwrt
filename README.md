# RTL8125B OpenWrt Driver

The repository is for building the Realtek RTL8125 / RTL8125B(S)(G) driver for OpenWrt firmwares

Fork from [https://github.com/csrutil/realtek-r8125-openwrt](https://github.com/csrutil/realtek-r8125-openwrt)

[![Build Realtek r8125 driver for OpenWrt](https://github.com/Accelerator-Li/realtek-r8125-openwrt/actions/workflows/r8125.yaml/badge.svg?branch=main)](https://github.com/Accelerator-Li/realtek-r8125-openwrt/actions/workflows/r8125.yaml)

## Setup

Attention⚠️, only support official firmware. If you are compiling your own firmware, please refer to the scripts in the action.

First, download the corresponding ipk file according to your version, scp it to your device, and then run

```bash
opkg -i kmod-r8125_xxx.ipk
```

If you are using the 5.15 kernel, the r8196 driver should automatically drive your network card. If you want to force the use of the driver from this project, you can delete the r8196 driver.
