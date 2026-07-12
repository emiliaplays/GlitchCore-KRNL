# GlitchCore-KRNL

> Custom Linux kernel for Samsung Exynos 9820 / 9825 devices

<p align="center">

![Linux](https://img.shields.io/badge/Linux-4.14.356-blue?style=for-the-badge)
![Android](https://img.shields.io/badge/Android-15-green?style=for-the-badge)
![KernelSU](https://img.shields.io/badge/KernelSU-Legacy-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-GPL--2.0-orange?style=for-the-badge)

</p>

Built and maintained by **GlitchByEmilia**

---

# About

GlitchCore-KRNL is a custom Linux **4.14.356** kernel for Samsung Galaxy S10 and Galaxy Note10 devices powered by the Exynos 9820 / 9825 platform.

The project is built completely from source with a focus on:

- Stability
- Performance
- Battery life
- Long-term maintainability
- Daily-driver reliability

Every public release is tested on real hardware before publication.

---

# Features

- Linux **4.14.356**
- Android 15 / One UI 7 compatible
- Built with Android Clang 20
- Built completely from source
- Custom GlitchCore branding
- AnyKernel3 flashable ZIP
- KernelSU-Next Legacy support
- Manual hook implementation
- Optimized VFS cache behavior
- Optimized for Exynos 9820 / 9825
- Boot-tested releases
- Stable daily-driver kernel

---

# Current Release

## GlitchCore-KRNL v1.2

| Feature | Status |
|---------|--------|
| Boot | ✅ |
| Daily Driver | ✅ |
| One UI 7 | ✅ |
| KernelSU Legacy | ✅ |
| VFS Cache Optimization | ✅ |
| Stability | ✅ |
| Battery Life | ✅ |
| Performance | ✅ |

---

# KernelSU

GlitchCore-KRNL includes built-in support for:

**KernelSU-Next Legacy v3.2.0**

Current status

```text
KernelSU Version
----------------
v3.2.0-legacy

Hook Mode
---------
Manual

Driver
------
Built-In

Status
------
Working
```

The recommended Manager APK is included with every GitHub release and inside this repository.

```text
extras/
└── KernelSU-Next/
    └── KernelSU_Next_v3.2.0_33129-release.apk
```

For best compatibility always use the bundled Manager.

If KernelSU Manager reports:

```
Non-GKI Kernel
```

after flashing, simply reinstall the bundled KernelSU Manager APK.

The kernel already contains the correct KernelSU Legacy driver.

---

# Supported Devices

| Device | Codename |
|---------|----------|
| Galaxy S10e | beyond0lte |
| Galaxy S10 | beyond1lte |
| Galaxy S10+ | beyond2lte |
| Galaxy S10 5G | beyondx |
| Galaxy Note10 | d1 |
| Galaxy Note10+ | d2s |
| Galaxy Note10+ 5G | d2x |

---

# Flashing

Flash the generated AnyKernel3 ZIP using **TWRP Recovery**.

Recommended before flashing:

- Backup your Boot partition
- Backup important files
- Keep a copy of your previous kernel
- Know how to recover using TWRP or Odin

---

# Building

Clone the repository:

```bash
git clone https://github.com/emiliaplays/GlitchCore-KRNL.git
cd GlitchCore-KRNL
```

Example build:

```bash
./build.sh --model d2s --ksu y
```

Supported models

```text
beyond0lte
beyond1lte
beyond2lte
beyondx

d1
d1xks
d2s
d2x
d2xks
```

---

# Roadmap

## GlitchCore-KRNL v1.2 OC

Currently under development.

Planned improvements

- Scheduler tuning
- CPU performance tuning
- GPU governor tuning
- Memory management improvements
- Devfreq tuning
- Additional performance profiles
- Source cleanup
- Further battery optimizations

Experimental features

- GPU overclock
- CPU overclock
- Thermal profiles
- Dynamic performance modes

---

# Disclaimer

```text
/*
 * Your warranty is now void.
 *
 * I am NOT responsible for:
 *
 * • Bricked devices
 * • Bootloops
 * • Lost data
 * • Dead SD cards
 * • Hardware damage
 * • Overheating
 * • Missed alarms
 * • Any damage caused by flashing this kernel
 *
 * You alone are responsible for anything that happens
 * to your device.
 *
 * Always make a backup before flashing.
 */
```

---

# Credits

Huge thanks to everyone whose work made this project possible.

- Ravindu644
- ExtremeKernel
- KernelSU-Next
- OpenELA
- Samsung Open Source Release Center
- Android Open Source Project (AOSP)
- Linux Kernel Community

Without these projects this kernel would not exist.

---

# License

GlitchCore-KRNL is licensed under the **GNU General Public License v2 (GPL-2.0)**.

This project is based on the Linux kernel and therefore all kernel modifications remain licensed under GPL-2.0.

See the **COPYING** file for the full license.

---

# Support

Please open a GitHub Issue if you encounter a bug.

When reporting issues include:

- Device model
- ROM version
- Kernel version
- Recovery used
- Steps to reproduce
- Kernel logs
- Recovery logs (if available)

---

# Philosophy

GlitchCore-KRNL follows a simple philosophy.

- Stability before benchmarks
- Battery before unnecessary overclocking
- Measured optimizations instead of placebo tweaks
- Clean source code
- Open-source development
- Daily-driver reliability
- Long-term support

Every public release is tested on real hardware before being published.

---

# Downloads

Official releases are available on GitHub.

Each release includes:

- AnyKernel3 flashable ZIP
- SHA-256 checksum
- Recommended KernelSU-Next Manager APK
- Release notes
- Complete changelog

---

# Contributing

Contributions are always welcome.

Feel free to:

- Open Issues
- Submit Pull Requests
- Report bugs
- Suggest new features
- Improve documentation

---

# Thank You ❤️

Thank you for using **GlitchCore-KRNL**.

If you enjoy this project, consider giving the repository a ⭐ on GitHub.

Happy flashing!

**— GlitchByEmilia**
