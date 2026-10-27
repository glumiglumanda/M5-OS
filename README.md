# 🚀 M5-OS (for M5Stack CoreS3)

An open-source, touch-first Operating System powered by a **JavaScript Runtime (QuickJS)** and an **OTA AppStore**, running entirely from internal Flash (LittleFS).

---

## 💡 The Vision
Most M5Stack firmwares require re-flashing to change tools or apps. **M5-OS** turns the M5Stack CoreS3 into an extensible platform where apps are written in lightweight JavaScript (`.js`) and downloaded directly over Wi-Fi.

- **JS-Driven:** Millions of developers can write hardware apps without deep C++ knowledge.
- **Internal Flash Storage:** Works out-of-the-box using LittleFS (no SD card required).
- **OTA AppStore:** Browse and install community apps over Wi-Fi with a single tap.
- **Hardware Bindings:** Native JS APIs for Camera, Touchscreen, Audio, Wi-Fi, and Sensors.

---

## 🏗️ System Architecture Plan
- **Core System (C++ / ESP-IDF):** Manages boot, hardware drivers, LVGL touch UI, and LittleFS.
- **JS Engine (QuickJS):** Executes JS scripts safely without risking system crashes.
- **Bridge API:** Maps JS commands (e.g., `M5.Speaker.beep()`) to C++ hardware functions.
- **App Store Client:** Downloads JS bundles directly from GitHub/Web into local Flash.

---

## 🤝 Looking for Core Developers!
This project is in its early architectural stage. We are currently looking for **Embedded C++ Developers** to join the core team to help build:
1. QuickJS integration on ESP32-S3.
2. Initial C++ to JS hardware bindings (Touch, Display, Speaker).
3. Basic LVGL launcher layout.

If you want to help shape the core architecture, feel free to open an Issue, a Pull Request, or drop a message!
