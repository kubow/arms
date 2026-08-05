# Single-board computers

Use maintained external maps for discovery and OS coverage. Keep local notes only for owned, tested, or unusual boards.

## Start here

| Map | Best for | Read carefully |
|---|---|---|
| [Armbian](../../software/operating-systems/linux/armbian.md) · [board map](https://armbian.com/boards) | Board → Armbian image and support level | **Platinum**, **standard**, **community**, and **work in progress** are different promises |
| [DietPi](../../software/operating-systems/linux/dietpi.md) · [board map](https://dietpi.com/docs/hardware/) | Board → lightweight server image | DietPi support may exclude kernel, GPU, Wi-Fi, audio, and other upstream issues |
| [LibreELEC](../../software/operating-systems/linux/libreelec.md) · [board map](https://libreelec.tv/downloads/) | Board/SoC → Kodi appliance image | Media decoding and display support are SoC- and image-specific |
| [OpenWrt](../../software/operating-systems/linux/openwrt.md) · [hardware table](https://openwrt.org/toh/start) | Board/router → OpenWrt target | Check device revision, flash size, and installation method |

## Hardware maps

| Map | Best for | Limitation |
|---|---|---|
| [sbc.compare](https://sbc.compare/browse) | Filter and compare specifications, interfaces, price, and benchmarks | Third-party data; verify against the manufacturer |
| [linux-sunxi devices](https://linux-sunxi.org/Category%3ADevices) | Allwinner board identification and upstream Linux work | Allwinner only; some pages describe old kernels |
| [linux-sunxi mainlining matrix](https://linux-sunxi.org/Linux_mainlining_effort) | Allwinner SoC feature status in mainline Linux | SoC support does not guarantee every board peripheral works |

## How to use a map

1. Find the exact board and hardware revision.
2. Check support tier and last image/update date.
3. Check the SoC, bootloader, storage, Ethernet, Wi-Fi, GPU/video, and GPIO separately.
4. Confirm that recovery media and a serial-console path exist.
5. Record only the chosen/tested combination in [Compatibility](../../COMPATIBILITY.md).

An available image means “boots on this target,” not necessarily “all hardware works.”

## Local notes

- [C.H.I.P.](chip/CHIP.md)
- [Cubieboard](cubietech/Cubieboard.md)
- [Cubietruck](cubietech/Cubietruck.md)
- [Pine64](pine64/Pine64.md)
- [Raspberry Pi](raspberry-pi/README.md)

Local OS relationships: [Compatibility](../../COMPATIBILITY.md#operating-systems).
