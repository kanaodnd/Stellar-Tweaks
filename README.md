<div align="center">
  <img src="https://github.com/kanaodnd/kanaokturu/raw/main/a740af124b50737a86e4c4782ed9c4c7.jpg" alt="Stellar Banner" width="100%" style="border-radius: 8px;">
  
  <br>

  <h1>✨ Stellar Tweaks</h1>
  <i>A another kernel scheduler for Balancing you need, feel a harmony melody. Stellar Stellar~</i>
  
  <br><br>

  <a href="https://github.com/kanaodnd/Stellar-Tweaks/releases">
    <img src="https://img.shields.io/github/v/release/kanaodnd/Stellar-Tweaks?style=flat-square&color=7050ff&label=Release" alt="Release">
  </a>
  &nbsp;
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/License-Apache_2.0-blue?style=flat-square&color=007bff" alt="License">
  </a>
  &nbsp;
  <a href="https://t.me/hosshi_prjkt">
    <img src="https://img.shields.io/badge/Telegram-Channel-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Channel">
  </a>
  &nbsp;
  <a href="https://t.me/hosshi_chat">
    <img src="https://img.shields.io/badge/Telegram-Group-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Group">
  </a>

</div>

---

## What "Stellar" about?

**Stellar Tweaks** is a sophisticated scheduler designed to harmonize device performance and efficiency. Built with a **Rust**, it operates silently in the background to manage system resources dynamically. Unlike static scripts, Stellar adapts to your usage patterns in real-time, offering a balance between raw power and battery longevity across various SoC platforms (Snapdragon, MediaTek, Exynos, Unisoc).

## Main Features

Stellar provides granular control over system parameters through its active daemon and modern WebUI interface.

### Core Capabilities
* **Kernel Tweaking Universal:** Adaptive parameter adjustments compatible with a wide range of kernels and Android versions.
* **CPU/GPU Clocking:** Dynamic frequency management to prevent throttling and ensure stability.
* **Specific Device System Constant:** Optimized property values tailored for system responsiveness.
* **DVFS Custom Rule:** Userspace-controlled Dynamic Voltage and Frequency Scaling for precise thermal and performance management.
* **I/O Scheduler Custom:** Tuned I/O priorities to reduce latency during heavy workloads.
* **Governor Custom:** Optimization of CPU governor parameters for efficient step-scaling.

### Basic AI Driven 3 Profiler
Stellar utilizes an intelligent engine to switch between three distinct modes based on real-time context:

1.  **GAMING**
    * Engages a deterministic performance envelope. Prioritizes consistent GPU/CPU throughput, enforces thread-priority policies, and manages thermal headroom to eliminate performance volatility.
2.  **POWERSAVER**
    * Implements aggressive non-critical process suspension and fine-grained clock gating. Maximizes battery longevity by enforcing strict QoS (Quality of Service) tiers on background subsystems.
3.  **BALANCE**
    * Utilizes a predictive, on-demand scaling architecture. Operates at a minimal power floor, then performs instantaneous, workload-aware frequency and core allocation to meet demand spikes without hysteresis.
---

## UI Preview

**Experience the Next-Gen Interface.**
Powered by **Material You (MD3)** technology, the Stellar WebUI offers a sleek, adaptive, and modern control panel. Designed for clarity and aesthetics, it makes complex system tuning intuitive and visually stunning.

### Root Environment
<div align="center">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/root/Screenshot_20260125_184447_WebUI%20X.jpg" width="30%" alt="Root Dashboard" style="border-radius: 6px; margin: 3px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/root/Screenshot_20260125_184139_WebUI%20X.jpg" width="30%" alt="Root Settings" style="border-radius: 6px; margin: 3px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/root/Screenshot_20260125_184120_WebUI%20X.jpg" width="30%" alt="Root Profiling" style="border-radius: 6px; margin: 3px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/root/Screenshot_20260125_184106_WebUI%20X.jpg" width="30%" alt="Root Tools" style="border-radius: 6px; margin: 3px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/root/Screenshot_20260125_184058_WebUI%20X.jpg" width="30%" alt="Root About" style="border-radius: 6px; margin: 3px;">
</div>

<br>

### Non-Root Environment
<div align="center">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/nonroot/Screenshot_20260124_091656_AxManager.jpg" width="30%" alt="NonRoot Dashboard" style="border-radius: 6px; margin: 3px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/nonroot/Screenshot_20260124_091649_AxManager.jpg" width="30%" alt="NonRoot Settings" style="border-radius: 6px; margin: 3px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/nonroot/Screenshot_20260124_091706_AxManager.jpg" width="30%" alt="NonRoot Tools" style="border-radius: 6px; margin: 3px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/nonroot/Screenshot_20260124_091726_AxManager.jpg" width="30%" alt="NonRoot Profiling" style="border-radius: 6px; margin: 3px;">
  <img src="https://github.com/kanaodnd/Stellar-Tweaks/raw/main/screenshot/nonroot/Screenshot_20260124_091719_AxManager.jpg" width="30%" alt="NonRoot About" style="border-radius: 6px; margin: 3px;">
</div>

---

## Supported Environments

Stellar Tweaks is designed to be versatile, supporting both Rooted and Non-Rooted environments with varying degrees of control.

| Environment | Supported Managers | Capability Level |
| :--- | :--- | :--- |
| **Root** | • KernelSU (Recommended)<br>• Magisk<br>• APatch | **Full Control**<br>(Direct Kernel access, DVFS, I/O, Governors, Bypass Charging) |
| **Non-Root** | • Axeron Manager | **Regular Optimization**<br>(AI Engine, Device Configuration, System Properties) |

---

## Installation

1.  **Download** the latest release from the [Releases Page](https://github.com/kanaodnd/Stellar-Tweaks/releases).
2.  **Install** via your preferred manager:
    * *Rooted/Unrooted User:* Flash the `.zip` file in Manager app.
3.  **Reboot (For Rooted Only)** your device to initialize the daemon.
4.  **Access** the dashboard via Manager interface to configure your preference.

---

## Community & Support

* **Bug Reports:** Please submit issues via [GitHub Issues](https://github.com/kanaodnd/Stellar-Tweaks/issues).
* **Discussion:** Join our Telegram group for support and feature requests.

<div align="center">

**If this project has been helpful to you, consider giving it a star ⭐**

<p align="center">
  <code>✦ "From me, to you, years from now." ✦</code>
</p>

</div>
