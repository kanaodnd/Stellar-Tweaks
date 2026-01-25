# ✨ Stellar Tweaks 
*A another kernel scheduler for Balancing you need, feel a harmony melody. Stellar Stellar~*

<div align="center">
  <img src="https://github.com/kanaodnd/kanaokturu/raw/main/a740af124b50737a86e4c4782ed9c4c7.jpg" alt="Stellar Banner" width="100%" style="border-radius: 8px;">
  <br><br>

  <a href="https://github.com/kanaodnd/Stellar-Tweaks/releases">
    <img src="https://img.shields.io/github/v/release/kanaodnd/Stellar-Tweaks?style=for-the-badge&color=7050ff&labelColor=1a1b26&logo=github&logoColor=white" alt="Latest Release">
  </a>
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/LICENSE-APACHE--2.0-blue?style=for-the-badge&color=007bff&labelColor=1a1b26&logo=apache&logoColor=white" alt="License">
  </a>
  <img src="https://img.shields.io/badge/WRITTEN_IN-RUST-orange?style=for-the-badge&color=ff7f50&labelColor=1a1b26&logo=rust&logoColor=white" alt="Written in Rust">

  <br>

  <a href="https://t.me/hosshi_prjkt">
    <img src="https://img.shields.io/badge/TELEGRAM-CHANNEL-26A5E4?style=for-the-badge&color=26A5E4&labelColor=1a1b26&logo=telegram&logoColor=white" alt="Channel">
  </a>
  <a href="https://t.me/hosshi_chat">
    <img src="https://img.shields.io/badge/TELEGRAM-GROUP-26A5E4?style=for-the-badge&color=26A5E4&labelColor=1a1b26&logo=telegram&logoColor=white" alt="Group">
  </a>
</div>

---

## Overview

**Stellar Tweaks** is a sophisticated scheduler designed to harmonize device performance and efficiency. Built with a **Rust daemon**, it operates silently in the background to manage system resources dynamically. Unlike static scripts, Stellar adapts to your usage patterns in real-time, offering a balance between raw power and battery longevity across various SoC platforms (Snapdragon, MediaTek, Exynos, Unisoc).

## Key Features

Stellar provides granular control over system parameters through its active daemon and modern WebUI interface.

### Core Capabilities
* **Kernel Tweaking Universal:** Adaptive parameter adjustments compatible with a wide range of kernels and Android versions.
* **CPU/GPU Clocking:** Dynamic frequency management to prevent throttling and ensure stability.
* **Specific Device System Constant:** Optimized property values tailored for system responsiveness.
* **DVFS Custom Rule:** Userspace-controlled Dynamic Voltage and Frequency Scaling for precise thermal and performance management.
* **I/O Scheduler Custom:** Tuned I/O priorities to reduce latency during heavy workloads.
* **Governor Custom:** Optimization of CPU governor parameters for efficient step-scaling.

### AI Driven 3 Profiler
Stellar utilizes an intelligent engine to switch between three distinct modes based on real-time context:

1.  **GAMING**
    * Prioritizes sustained performance, stabilizes FPS, and minimizes jitter for competitive gameplay.
2.  **POWERSAVER**
    * Maximizes battery life by aggressively limiting background activities and clock speeds during inactivity.
3.  **BALANCE**
    * The optimal middle ground for daily usage, scaling performance up instantaneously only when necessary.

---

## UI Preview

Experience a modern and intuitive control panel designed for ease of use.

### Root Environment
<div align="center">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/root/Screenshot_20260125_184447_WebUI%20X.jpg" width="45%" alt="Root Dashboard" style="border-radius: 8px; margin: 5px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/root/Screenshot_20260125_184139_WebUI%20X.jpg" width="45%" alt="Root Settings" style="border-radius: 8px; margin: 5px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/root/Screenshot_20260125_184120_WebUI%20X.jpg" width="45%" alt="Root Profiling" style="border-radius: 8px; margin: 5px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/root/Screenshot_20260125_184106_WebUI%20X.jpg" width="45%" alt="Root Tools" style="border-radius: 8px; margin: 5px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/root/Screenshot_20260125_184058_WebUI%20X.jpg" width="45%" alt="Root About" style="border-radius: 8px; margin: 5px;">
</div>

<br>

### Non-Root Environment (Axeron)
<div align="center">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/nonroot/Screenshot_20260124_091656_AxManager.jpg" width="45%" alt="NonRoot Dashboard" style="border-radius: 8px; margin: 5px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/nonroot/Screenshot_20260124_091649_AxManager.jpg" width="45%" alt="NonRoot Settings" style="border-radius: 8px; margin: 5px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/nonroot/Screenshot_20260124_091706_AxManager.jpg" width="45%" alt="NonRoot Tools" style="border-radius: 8px; margin: 5px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/nonroot/Screenshot_20260124_091726_AxManager.jpg" width="45%" alt="NonRoot Profiling" style="border-radius: 8px; margin: 5px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/nonroot/Screenshot_20260124_091719_AxManager.jpg" width="45%" alt="NonRoot About" style="border-radius: 8px; margin: 5px;">
</div>

---

## Supported Environments

Stellar Tweaks is designed to be versatile, supporting both Rooted and Non-Rooted environments with varying degrees of control.

| Environment | Supported Managers | Capability Level |
| :--- | :--- | :--- |
| **Root** | • KernelSU (Recommended)<br>• Magisk<br>• APatch | **Full Control**<br>(Direct Kernel access, DVFS, I/O, Governors, Bypass Charging) |
| **Non-Root** | • Axeron Manager | **User-space Optimization**<br>(AI Engine, UI Customization, System Properties) |

---

## Installation

1.  **Download** the latest release from the [Releases Page](https://github.com/kanaodnd/Stellar-Tweaks/releases).
2.  **Install** via your preferred manager:
    * *Root Users:* Flash the `.zip` file in Magisk/KSU/APatch app.
    * *Non-Root Users:* Import the module into Axeron Manager.
3.  **Reboot** your device to initialize the daemon.
4.  **Access** the dashboard via the WebUI or manager interface to configure your profiles.

---

## Community & Support

* **Bug Reports:** Please submit issues via [GitHub Issues](https://github.com/kanaodnd/Stellar-Tweaks/issues).
* **Discussion:** Join our Telegram group for support and feature requests.

<div align="center">
  <p>If you find this project useful, consider supporting the development.</p>
  <a href="https://github.com/kanaodnd/DonateMePls">
    <img src="https://img.shields.io/badge/SUPPORT-DONATE-FF4D4D?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=1a1b26" alt="Donate">
  </a>
</div>
