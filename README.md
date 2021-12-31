# OpenCore-Z370m-ITX

> The OpenCore config for ASRock Z370m ITX

## Working hardware

- CPU: i3-8100
- MainBoard: ASRock Z370m-ITX
- GPU Card: RX580

## Working version

- OpenCore 0.6.7
- macOS 10.15.7

# Working features

- iGPU HDMI and DP
- AMD GPU DP
  - (10 Bit Color-Depth)
- Broadcom Bluetooth

## Not Working features

- AMD GPU HDMI
- Broadcom Wi-Fi
- AirDrop

## Keypoint config

BIOS

```shell
# Chipset

Wi-Fi       Disable
```

config.plist

```shell
# DevicesProperties >
# PciRoot(0x0)/Pci(0x2,0x0)
# i3-8100
AAPL,ig-platform-id     07009B3E


# PlatformInfo > Generic
# macOS 10.15+
System Product Name     iMac19,1
# macOS 10.13+
System Product Name     iMac18,3


# UEFI > APFS
MinDate -1      MinVersion  -1
```

## Thanks to

- The [OpenCore](https://github.com/acidanthera/OpenCorePkg) Project and its team

- The [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html) # Desktop Coffee Lake
