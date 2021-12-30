# The Z370m-ITX OpenCore Profile

## Working hardware

- CPU: i3-8100
- MainBoard: ASRock Z370m-ITX
- GPU Card: RX580

## Working version

- OpenCore 0.6.7
- macOS 10.15.7

# Working features

- iGPU HDMI and DP
- Broadcom Bluetooth

## Not Working features

- Broadcom Wi-Fi
- Airdrop

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
