<div align="center">
  <img src="https://github.com/kanaodnd/kanaokturu/raw/main/a740af124b50737a86e4c4782ed9c4c7.jpg" alt="Stellar Banner" width="100%" style="border-radius: 8px;">
  
  <br>

  <h1>Stellar Tweaks</h1>
  <p><b>Intelligent Performance & Energy Orchestration Engine for Android</b></p>

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

## Overview

Most traditional Android optimization tools rely on static shell scripts, aggressive throttling, or continuous `dumpsys` polling loops that consume CPU resources and introduce frame volatility.

**Stellar Tweaks** is a deterministic orchestration engine engineered in **Rust** with native Android framework integration. It operates silently in userspace and kernelspace to dynamically align system resources, rendering pipelines, and hardware governors with real-time application demands across Qualcomm Snapdragon, MediaTek, Samsung Exynos, and Unisoc platforms.

> [!WARNING]
> Stellar directly orchestrates low-level kernel subsystems, CPU/GPU governors, and Dynamic Voltage and Frequency Scaling (DVFS). To prevent parameter collisions and ensure deterministic scheduling, avoid running concurrent third-party performance modules or conflicting optimizer scripts.

---

## Key Features

<details open>
<summary><b>1. Fast Energy Aware Scheduling (FEAS)</b></summary>
<br>

* **Dynamic Frame Awareness:** Monitors render thread throughput in real time, scaling hardware frequency curves to prevent frame drops during sudden rendering spikes.
* **Cluster-Aware Thread Affinity:** Directs high-priority threads (such as `RenderThread` and game engine threads) to Prime and Big CPU cores, while offloading background tasks to efficiency clusters.
* **Cooperative Idle Snapping:** Smoothly transitions hardware into low-power states during global inactivity without relying on evdev polling loops.
</details>

<details open>
<summary><b>2. Hardware & Power Orchestration</b></summary>
<br>

* **Custom GPU Governors:** Independent GPU governor configuration per profile (`Powersaving`, `Balanced`, `Gaming`) across Adreno, Mali, Devfreq, and KGSL architectures.
* **Dynamic I/O Scheduling:** Context-sensitive block I/O scheduling backed by cached hardware device mapping to eliminate storage hitching.
* **Advanced DVFS & Power Management:** Granular userspace frequency limits that balance power draw and sustained performance during heavy workloads.
* **Bypass Charging (Idle Battery State):** Allows supported hardware to draw power directly from the charger without routing current into the battery cell, significantly lowering thermal generation.
* **Fast Charging Monitoring:** Maintains stable charging throughput while respecting safety boundaries.
</details>

<details open>
<summary><b>3. Display & Visual Synchronization</b></summary>
<br>

* **Multi-Vendor Display Controller:** Integrated support for Xiaomi, Samsung, Transsion (Infinix/Tecno), BBK/Oplus, and generic AOSP display interfaces.
* **Force Refresh Rate Mode:** Overrides vendor display lockouts when standard Android display managers fail to engage high refresh rates.
* **Battery-Saver Refresh Limiter:** Automatically locks the display panel to 60Hz whenever the Android Battery Saver mode engages.
</details>

<details open>
<summary><b>4. Framework Integration & Utilities</b></summary>
<br>

* **Device Identity Spoofing:** Built-in system-level device spoofing profiles to unlock 90/120 FPS configurations in supported titles.
* **System Native Notifications:** Emits clean `<App Label> • Optimized` toast alerts natively without requiring overlay or floating window permissions.
* **Modular Component Uninstaller:** Granular cleanup subroutines allowing users to selectively remove configuration directories (`clean config`) or revert hardware tweaks (`clean tweaks`).
* **Self-Healing Boot Configuration:** Automatically detects panel refresh rates on initial startup and generates valid defaults without user intervention.
</details>

---

## Operational Profiles

Stellar automatically transitions across three standard operational profiles based on your active usage:

| Profile | Primary Use Case | System Behavior |
| :--- | :--- | :--- |
| **Gaming** | Active gameplay & heavy render workloads | Enforces consistent performance, sets gaming hardware governors, activates bypass charging, and minimizes background interruptions. |
| **Balanced** | Daily usage, social media & multitasking | Delivers smooth responsiveness for everyday tasks while maintaining balanced power consumption and cooler device operation. |
| **Powersaver** | Low battery & emergency endurance | Caps background power draw, locks the display refresh rate to 60Hz, and shifts hardware governors to maximize battery life. |

---

## Stellar Pro (Exclusive Tier)

Stellar provides an **Exclusive / Pro Tier** designed for users who want to actively support project research and continuous development.

### Concept & Decision Intelligence
The Pro tier serves as an elevated decision intelligence layer within the daemon, offering refined automated decision-making and enhanced operational control. Supporting the project directly aids in testing across real hardware devices, maintaining kernel compatibility, and driving continuous development updates.

For tier activation details and donation options, visit the [Stellar Project Support Notice](https://t.me/hosshi_prjkt/644).

---

## User Interface Preview

Powered by **Material You 3 (M3)** design principles, the Stellar WebUI provides an intuitive, dark-surface control interface. Compiled into a single-file distribution, it requires zero external downloads and functions completely offline.

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

| Environment | Supported Managers | Capability Scope |
| :--- | :--- | :--- |
| **Root** | • KernelSU<br>• Magisk<br>• APatch | **Full Hardware & Framework Access**<br>Direct kernel tweaking, FEAS scheduling, CPU/GPU governors, I/O schedulers, display overrides, bypass charging, and hardware caches. |
| **Non-Root** | • Axeron Manager | **Userspace Optimization**<br>Dynamic app profiling, system properties, userspace priority tuning, and visual dashboards. |

> [!NOTE]
> Root access grants complete control over sysfs nodes and hardware governors. On non-rooted environments via Axeron Manager, Stellar operates within userspace privilege boundaries without modifying low-level kernel nodes.

---

## Command-Line Interface

The `stellar-daemon` binary provides straightforward terminal commands:

```bash
# Start the orchestration daemon in foreground
stellar-daemon start

# Query runtime diagnostics and active operational mode
stellar-daemon stats

# Modular component cleanup
stellar-daemon clean tweaks    # Revert kernel parameters and display locks to defaults
stellar-daemon clean config    # Remove configuration and applist files
stellar-daemon clean all       # Full rollback: revert tweaks, delete configs, stop daemon
```

---

## Installation

1. **Download** the latest release package from the [Releases](https://github.com/kanaodnd/Stellar-Tweaks/releases) page.
2. **Install** via your preferred module manager:
   * **Root:** Flash the `.zip` archive in KernelSU, Magisk, or APatch.
   * **Non-Root:** Import the module through Axeron Manager.
3. **Reboot** your device (Root only) to initialize the daemon and allow automated hardware mapping.
4. **Launch** the WebUI dashboard from your manager to customize preferences.

---

## Credits & References

Acknowledgement and appreciation to the following developers whose open-source tools, technical research, and concepts served as valuable references during the development of Stellar:

* **Rem01Gaming**
* **Notzeeta**
* **HoyoSlave**
* **Zesxhia**

---

## Community & Support

* **Issue Tracking:** Submit bug reports or technical inquiries via [GitHub Issues](https://github.com/kanaodnd/Stellar-Tweaks/issues).
* **Community Channels:** Join the [Telegram Channel](https://t.me/hosshi_prjkt) and [Telegram Group](https://t.me/hosshi_chat) for announcements, discussions, and release builds.

<div align="center">

**If you find Stellar Tweaks useful, consider starring the repository.**

</div>
