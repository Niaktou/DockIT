![DockIT logo](DockIT_logo.png)
A fully modular things

# DockIT — Modular Desktop Control System

DockIT is a customizable, 3D-printed, ESP32-powered modular control station designed to complement your keyboard and enhance your desktop experience. With a sleek neumorphic interface and hot-pluggable modules, DockIT is your personal command center.

---

## 🚀 Features

- **Modular design** with magnetic + pogo pin connection
- **Main module** with a 480x320 touchscreen (ILI9488)
- Custom operating system interface ("DockIT OS") with animated UI
- Real-time module detection and display
- **Modules include:**
  - 🎚️ Slider Module (4 analog faders)
  - 🌦️ Weather Module (location, time, weather)
  - 🎛️ Macro Keypad Module (custom shortcut buttons)
  - 🔉 Sound Knob Module (infinite rotary encoder with feedback)
  - 🔌 USB Hub / Charger Module (USB-A & USB-C)
  - 🖥️ Info Display Module (CPU temp, animated GIFs, system stats)
- Capacitive touch support (GLS1680F)
- Future Bluetooth + USB dual-mode support

---

## 🧩 Architecture

- **Main controller:** ESP32-S3 with PSRAM
- **Display:** 3.5” ILI9488 TFT LCD, SPI or 8-bit parallel
- **Touchscreen:** Capacitive, I2C
- **Module detection:** I2C EEPROM + ID mapping
- **Modular connection:** Pogo pins + neodymium magnets

---

## 🖥️ User Interface

- Custom UI using **LVGL**
- Neumorphic design
- Modular interface adapts dynamically as modules are connected
- Smooth transitions and boot animation (DockIT logo)

---

## 🔧 Hardware

| Component        | Reference                  |
|------------------|----------------------------|
| Microcontroller  | ESP32-S3                   |
| Screen           | 3.5" ILI9488 TFT LCD       |
| Touch Controller | GLS1680F (I2C)             |
| EEPROM per module| AT24C256                   |
| Slider Faders    | DJM B10KX2 (80mm max)      |
| Rotary Encoder   | EC11 / Magnetic (no detents)|
| Motor Driver (optional)| TB6612FNG or L293D   |
| Pogo Pins        | 8–10 pins per module       |

---

## 🧪 Status

- [~] Hardware prototyping (main module + slider)
- [~] UI mockups and boot animation
- [ ] Full modular hot-plug detection
- [ ] Bluetooth/USB HID implementation
- [~] Final 3D-printed case design

---

## 🛠️ Installation (coming soon)

> 🚧 In progress: will include wiring diagrams, LVGL configuration, and firmware installation

---

## 📁 Directory Structure
