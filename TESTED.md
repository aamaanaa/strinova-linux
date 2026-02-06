### Legend

- ✅ Perfect game experience
- ⚠️ Playable 
- ❌ Does not work at all

### Hardware Table

| | Wine version | System, DE | GPU | Comment |
|-|--------------|------------|-----|---------|
| ✅ | [wine-tkg 10.5 staging ntsync](https://github.com/future-XD/wine-tkg-staging-ntsync-git) | Fedora 43, GNOME, Wayland (stock kernel) | [NITRO+ AMD Radeon™ RX 7900 XTX Vapor-X 24GB](https://www.sapphiretech.com/en/consumer/nitro-radeon-rx-7900-xtx-vaporx-24g-gddr6) | Repo author's system. Amd 9 9950X3D cpu, overclocked. GPU has byski waterblock.
| ✅ | wine 10.7 staging | Fedora 42, Hyprland, Wayland | RX 570, RX5600 GPU | 
| ⚠️ | wine-tkg 10.9 staging | Mint 22.1, Cinnamon | RTX 3070 | Missing textures, gameplay not affected |
| ✅ | kron4ek-wine-10.10-staging-tkg-amd64 | Arch Linux (Kernel 6.15.5), Hyprland 0.49.0 | RTX 3060 |
| ✅ | wine-10.11-tkg-staging-ntsync-git (10.11.r0.g3e94d124-327) | CachyOS, bspwm, Linux kernel 6.12.36-1-lts, mesa-git | AMD Radeon RX 6600 | Even with a cursed PC setup with mixed RAM modules, game data on an external NTFS SSD, the game runs without any issue.
| ✅ | wine-10.11-staging-tkg-ntsync-amd64-wow64 | Arch linux, KDE Plasma, Wayland, Zen 6.15.5 | AMD Radeon RX 480 |
| ✅ | kron4ek-wine-10.12-staging-tkg-amd64 | Manjaro, GNOME, Wayland | AMD Radeon RX 6800 xt |
| ✅ | Kron4ek-wine-10.10-staging-tkg-amd64 | Endeavor Os, KDE 6, Wayland | Nvidia RTX 3070 Mobile | 
| ✅ | kron4ek-wine-10.10-staging-tkg-amd64 | Ultramarine 42, GNOME, Wayland | RX 9060 XT 16GB | 
| ✅ | wine-10.7-staging-tk-x86_64 | Debain Unstable, Cinnamon, Xorg | Radeon VEGA 6 | Running fine with luteis. Bottles presents issues with freezing
| ✅ | kron4ek-wine-10.12-staging-tkg-amd64 | CachyOS, AwesomeWM | AMD Radeon RX 5500M
| ✅ | kron4ek-wine-10.17-staging-tkg-amd64| Arch Linux 6.17.5-lqx1, Hyprland | RTX3060 (580.95.05)
| ✅ | kron4ek-wine-10.18-staging-tkg-amd64| Fedora 43 KDE(wayland) | 1050ti/mx150 (same gpu)  | Everything works fine, but the game launches only on the second attempt. I’m running the game via Steam inside Bottles. This is the same setup I used on Windows, and I didn’t bother reinstalling the game separately for Linux without steam.Problem: after clicking Run in the launcher, the game hangs on a black screen. I have to close it, launch it again - and only then it works.This happens every time. Even if I close only the game (not the launcher), I still need to start it twiceI suspect this is related to running the game from an NTFS drive mounted via userspace FS(ntfs-3g).What’s especially odd, the game launches only when the drive is mounted by Dolphin.When I set up auto-mount with the same filesystem (ntfs-3g) or with ntfs3, the game stops launching entirely I tried to mount the disk in the home directory, at the moment when Dolphin mounts it in /run/media/{user}/{mount_point} maybe it is reason, IDK. 
| ✅ | kron4ek-wine-10.10-staging-tkg-amd64 | Ubuntu 25.04 with KDE | NVIDIA RTX 4060 |








...actually there are few more confirmed runs without provided info, feel free to [report your hardware](https://github.com/aamaanaa/strinova-linux/issues/new/choose)
