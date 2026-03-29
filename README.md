# ⌨️ PMO Wave75: VIA Fix & Split Encoder Mod

This repository provides corrected `.JSON` definition files for the **PMO Wave75** mechanical keyboard. It is specifically designed to resolve common validation errors in the VIA web configurator and add support for custom hardware modifications.

## 🛠 Resolved Errors

When loading original manufacturer draft definitions, users often encounter the following schema validation failures which this project fixes:

- **`JSON Object: should have required property 'lighting'`**: Fixed by injecting the missing `qmk_rgblight` property.
    
- **`JSON Object: should NOT have additional properties`**: Resolved by stripping non-standard top-level blocks like `keycodes` and `customKeycodes` that VIA's parser rejects.
    

## ✨ Features

- **Split Encoder Support**: Modified matrix and keymap definitions to recognize and map a split encoder hardware mod.
    
- **Translated Interface**: English translations for original Chinese system functions and RGB menus.
    
- **VIA V2 Compatibility**: Optimized for the "Use V2 definitions (deprecated)" workflow in modern VIA clients.
    

## 🚀 Quick Start

1. **Before** installing the Split Encoder **make sure the 4 contact points on the mother board are gently scraped, and the clear plastic film cut away**.
2. Put the keyboard back together.
3. Install [QMK Toolbox](https://qmk.fm/toolbox).
4. Download 'WAVE75 Tri-mode RGB（QMK Firmware）.bin' from this repo.
5. Open **QMK Toolbox** and open local file 'WAVE75 Tri-mode RGB（QMK Firmware）.bin'.
6. **WHILE HOLDING ESC KEY ON KEYBOARD** plug it in your computer. QMK Toolbox should reconize the device.
7. Click **Flash**.
8. **Download** the `WAVE75【Only use in wired mode】RGB Version (V2).JSON` from this repo.
9. Open the [VIA Web App](https://usevia.app/).
10. Navigate to the **Settings** tab and enable **Show Design tab**.
11. In the **Design Tab** load the `.JSON` file.
12. Enable **Split Encoder** in the **Design** and **Configure** tab.

---
