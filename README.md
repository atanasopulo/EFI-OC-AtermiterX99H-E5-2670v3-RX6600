# Sonoma on Atermiter X79 + E5-2620v2 + AMD RX6600 | OpenCore

## I made publicly available my configuration, so people struggling like I was can at least get closer to a solution.

### Check this post on Reddit, for which I made this repository:

#### https://www.reddit.com/r/hackintosh/comments/17eteyc/sonoma_on_atermiter_x99d4_e52670v3_amd_rx6600/

### The hardwae this is made for:

- CPU: Xeon E5-2670 v3 | 12 cores 24 threads | 2.3GHz turbo 3.1GHz.
- Motherboard: Atermiter X99H.
- GPU: Sapphire PULSE | AMD RX6600 8GB.
- RAM: 64GB 2133 MHz ECC DDR4 (4x16GB).
- Ethernet Card: Realtek RTL8111.
- Internal Audio: ALC897.
- BT Card: CSR 4.0 Bluetooth USB dongle (Qualcomm/Cambridge Silicon Radio CSR8510).
- NVME: ADATA XPG Spectrix S20G 1Tb

### I made two different EFI configurations as described below:

- [EFI VirtualSMC](https://github.com/VivaPeron/EFI-OC-AtermiterX99H-E5-2670v3-RX6600/tree/main/EFI%20VirtualSMC): This one is very stable and safe to use to boot into the Monterey right after it's been installed.
- [EFI FakeSMC3](https://github.com/VivaPeron/EFI-OC-AtermiterX99H-E5-2670v3-RX6600/tree/main/EFI%20FakeSMC3): This one replaces VirtualSMC with FakeSMC3, which in my case has better support for hardware sensors.

Both includes the kexts and OpenCore entries for the bluetooth dongle. Please check the reddit post for further info on that particular bluetooth setup.


You can test them if want. But, please, take into consideration that if your CPU, motherboard, or GPU, are different, then it might not work if you don't adapt it.
The SMBIOS info like serials, UUID, etc are safe. But please change them as someone else might be using them already.