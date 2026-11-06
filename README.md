<!--
  ChromeOS Brunch Builds
  Prebuilt images and release notes for the community.
-->

<div align="center">

# ChromeOS Brunch Builds

**Prebuilt ChromeOS images for compatible x86_64 PCs**

[![Builds](https://img.shields.io/badge/Builds-Prebuilt-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white)](https://github.com/HexaGhost-09/chromeos-brunch-builds/releases)
[![Platform](https://img.shields.io/badge/Platform-x86__64-0A66C2?style=for-the-badge&logo=intel&logoColor=white)](#hardware-and-recovery-selection)
[![Framework](https://img.shields.io/badge/Framework-Brunch-34A853?style=for-the-badge)](https://github.com/sebanc/brunch)
[![License](https://img.shields.io/badge/License-See%20third--party%20licenses-lightgrey?style=for-the-badge)](#credits-and-licenses)

[**⬇️ Download latest build**](https://github.com/HexaGhost-09/chromeos-brunch-builds/releases/latest)
· [All releases](https://github.com/HexaGhost-09/chromeos-brunch-builds/releases)
· [Report an issue](https://github.com/HexaGhost-09/chromeos-brunch-builds/issues)

</div>

---

## 📌 About

This repository provides **prebuilt ChromeOS images created with the Brunch framework**. The aim is to make testing and installing ChromeOS easier for users who do not want to build an image manually.

Builds are distributed through **GitHub Releases**. Each release should include its ChromeOS version, Brunch version, recovery target, image format, build date, and any known issues.

> **Important:** These are unofficial community builds. They are not produced, endorsed, or supported by Google or the ChromeOS team.

## ⬇️ Downloads

| What you need | Link |
|---|---|
| Latest available build | [Download latest release](https://github.com/HexaGhost-09/chromeos-brunch-builds/releases/latest) |
| All available builds | [Browse releases](https://github.com/HexaGhost-09/chromeos-brunch-builds/releases) |
| Build instructions / source | [Brunch framework](https://github.com/sebanc/brunch) |

If no release is available yet, check back later. Build files will be attached to individual GitHub Releases rather than committed to the repository.

### Choosing a build

1. Identify your processor model and generation.
2. Check the recovery-target reference below.
3. Open the release notes and choose the matching build.
4. Read the release-specific installation instructions before writing the image to a drive.

**Do not choose a build based on processor generation alone.** Wi-Fi, graphics, storage, firmware, and other device-specific hardware can affect compatibility.

## 🧩 Hardware and recovery selection

The following table records the recovery-target mapping used as a reference for this build collection. It is a **target-selection guide, not a guarantee that every processor in a row is supported**.

### Intel processors

| Processor generation | Recovery codename |
|:--|:--|
| 3rd generation or older | `samus` |
| 4th and 5th generation | `leona` |
| 6th to 9th generation | `shyvana` |
| 10th generation | `jinlon` |
| 11th generation and newer | `voxel`* |

### AMD processors

| Processor family | Recovery codename |
|:--|:--|
| AMD Ryzen | `gumboz` |

\* **Version note:** Recovery targets can change between ChromeOS and Brunch releases. Current upstream Brunch documentation lists newer targets for some Intel generations (including `kanix` for 14th-generation/Core Ultra systems). Always check the [official Brunch README](https://github.com/sebanc/brunch#readme) and the notes attached to the specific build before downloading.

### General hardware considerations

- Use a compatible **64-bit (x86_64)** system with UEFI support.
- Brunch compatibility depends on the CPU, integrated graphics, firmware, kernel, and individual device components.
- Dedicated graphics, ARM processors, virtual machines, and older CPUs may be unsupported depending on the Brunch version.
- Wi-Fi, Bluetooth, audio, camera, microphone, touchpad, touchscreen, and suspend may not work on every device.

Check the upstream [Brunch hardware documentation](https://github.com/sebanc/brunch/wiki/Hardware-Support) before installing.

## 💻 Installation

Installation steps and supported image formats may differ between releases. **Follow the instructions in the release you downloaded.**

Before installing:

1. Back up important files.
2. Confirm that the image matches your hardware and recovery target.
3. Read all release notes and known issues.
4. Verify the downloaded archive or image checksum when one is provided.
5. Use a suitable image-writing tool only after confirming the target drive.

⚠️ **Warning:** Installing or using an unofficial ChromeOS image can cause data loss, including loss of data on other partitions. Do not install it on a device containing important data unless you have a verified backup and understand the risks.

## 📦 Release information

Each published release should provide:

| Detail | Description |
|---|---|
| ChromeOS version | Version of the ChromeOS recovery image used |
| Brunch version | Brunch framework release used |
| Recovery target | Intel / AMD codename |
| Image format | Exact format of the uploaded image |
| Build date | Date the image was generated |
| File checksum | SHA-256 hash, when available |
| Known issues | Hardware limitations or problems found during testing |

Large image files are hosted as **release assets**. They are not stored in the Git repository itself.

## ⚠️ Disclaimer

- This project is independent and is not affiliated with, endorsed by, or supported by Google.
- ChromeOS and related Google components remain the property of their respective owners.
- Brunch is a third-party framework. Review its documentation, license, and warnings before use.
- Hardware compatibility is not guaranteed. A build that works on one PC may fail on another, even with a similar processor.
- You are responsible for checking applicable licenses and distribution permissions before downloading, using, or redistributing any build.
- Use at your own risk. Keep backups of important data.

## 🙏 Credits and licenses

- [Brunch framework](https://github.com/sebanc/brunch) — the framework used to create generic ChromeOS images.
- [ChromeOS recovery images](https://chromeos.google.com/) — ChromeOS source images.
- All trademarks and product names belong to their respective owners.

---

<div align="center">

**Made for the community.**

[⬇️ Releases](https://github.com/HexaGhost-09/chromeos-brunch-builds/releases) · [🐛 Issues](https://github.com/HexaGhost-09/chromeos-brunch-builds/issues)

</div>
