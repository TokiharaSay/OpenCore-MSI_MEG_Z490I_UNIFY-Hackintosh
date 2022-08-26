<div align="center">
<img src="https://asset.msi.com/resize/image/global/product/product_3_20200507175236_5eb3da64772d8.png62405b38c58fe0f07fcef2367d8a9ba1/1024.png" width="350px">
</div>

<h1 align="center">MSI Z490i UNIFY Hackintosh</h1>
<h3 align="center">微星 Z490i UNIFY 黑苹果 OpenCore 引导配置</h3>
<br>

### Computer Spec:

| Component        | Brank                              |
| ---------------- | ---------------------------------- |
| CPU              | Intel i9 10900T ES (10C-20T)       |
| iGPU             | Intel® HD 630 Graphics             |
| DGPU             | DELL  Radeon RX 5300               |
| Lan              | Realtek PCIe 2.5GbE                |
| Audio            | Realtek ALC1220/S                  |
| Ram              | KLEVV 32 GB DDR4 3200 Mhz          |
| Wifi + Bluetooth | Intel® AX201  BCM94360Z4           |
| NVMe             | WD SN550 1T*2  INTEL S3520 120G    |
| SmBios           | iMac 19,1                          |
| BootLoader       | OpenCore 0.8.4                     |
| macOS            | Ventura 13.0 Beta6                 |

## Working & Not Working / 可用与不可用的功能

### Non-Fuctional / 不工作

| Feature | Status | Dependency | Remarks |
| --- | --- | --- | --- |
| Thunderbolt 3 Hotplug<br>雷电接口热插拔 | ⚠️ |  | Thunderbolt Driver 和认证可能不加载；雷电固件可能不识别 |

### Video and Audio / 音频与视频

| Feature | Status | Dependency | Remarks |
| --- | --- | --- | --- |
| Full Graphics Accleration (QE/CI)<br>图形硬件加速 | ✅ | `WhateverGreen.kext` | |
| Audio Playback through 3.5mm<br>通过 3.5mm 接口播放音频 | ✅ | `AppleALC.kext` | |
| Automatic Headphone Output Switching<br>当插入耳机时自动切换音频输出 | ✅ | `AppleALC.kext` | |

### Power, Charge, Sleep and Hibernation / 电源管理、充电、睡眠、休眠

| Feature | Status | Dependency | Remarks |
| --- | --- | --- | --- |
| CPU Power Management (SpeedShift)<br>CPU 电源管理 | ✅ | `SSDT-PLUG and CPUFriendDataProvider` | |
| S3 Sleep / Hibernation Mode 3<br>S3 睡眠 / Mode 3 休眠 | ✅ | `原生支持` | |
| Hibernation Mode 25<br>Mode 25 休眠 | ⚠️ | | 测试休眠之后无法正常进入macos |

### Input & Output

| Feature | Status | Dependency | Remarks |
| --- | --- | --- | --- |
| WiFi | ✅ | `AirportFixup.kext` | Suggest to switch Broadcom based card<br>推荐更换博通无线网卡 |
| Bluetooth | ✅ | `94360Z4 APPLE firmware / 白果固件网卡` | Suggest to switch Broadcom based card<br>推荐更换博通无线网卡 |
| USB 2.0, USB 3.0 | ✅ | `USBToolBox UTBMap_Brcm/UTBMap_intel` | 根据你的需求使用UTBMap_Brcm/UTBMap_intel|

## Donation / 捐赠

Donating to this project is OPTIONAL. But feel free to buy me a coffee if you appreciate my works.

捐赠本项目 **并不是必需的**。但是如果我的项目对你有所帮助，为什么不考虑一下给我买杯咖啡呢？

<img src="https://fastly.jsdelivr.net/gh/TokiharaSay/Pic/IMG_2453(20220826-080924).JPG" width="350px">

## Maintainer / 维护者

**MSI_MEG_Z490I_UNIFY** © [TokiharaSay](https://github.com/TokiharaSay), Released under the [GPL-3.0](./LICENSE) License.<br>
Authored and maintained by TokiharaSaywith help from contributors ([list](https://github.com/TokiharaSay/OpenCore-MSI_MEG_Z490I_UNIFY-Hackintosh)）.

>[Blog](https://blog.runebalot.cn/) · GitHub [@TokiharaSay](https://github.com/TokiharaSay) · Twitter [@TokiharaSay](https://twitter.com/TokiharaSay) 
