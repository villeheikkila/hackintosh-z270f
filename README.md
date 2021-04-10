## Hardware

| Component        | Model                        |
| ---------------- | ---------------------------- |
| Motherboard      | Asus ROG Strix Z270F         |
| CPU              | Intel i7-7700K               |
| Memory           | Kingston HyperX 32GB 2666Mhz |
| Storage          | Samsung EVO 960 512GB NVMe   |
| GPU              | PowerColor Radeon RX 5700 XT |
| WLAN & Bluetooth | Fenvi T919 BCM94360CD        |

## Software

| Component | Model  |
| --------- | ------ |
| OpenCore  | 0.6.8  |
| macOS     | 11.2.3 |

## How to get started

Read the [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/). Set the MLB, ROM, SystemSerialNumber and SystemUUID as instructed.

## Status

Currently everything else works except for the unlock with Apple Watch stalls on login even though it works elsewhere. There are also some issues with DRM in Big Sur. Partial fix that can be used is to run

`defaults write com.apple.AppleGVA gvaForceAMDKE -boolean no`

in the terminal to force the use of the discrete GPU's decoder. This however breaks screen recording.
