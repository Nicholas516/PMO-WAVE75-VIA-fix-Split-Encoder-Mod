# ⌨️ PMO Wave75: VIA Fix & Split Encoder Mod

This repository provides corrected `.json` definition files for the **PMO Wave75** mechanical keyboard. It is specifically designed to resolve common validation errors in the VIA web configurator and add support for custom hardware modifications.

## 🛠 Resolved Errors

When loading original manufacturer draft definitions, users often encounter the following schema validation failures which this project fixes:

- **`JSON Object: should have required property 'lighting'`**: Fixed by injecting the missing `qmk_rgblight` property.
    
- **`JSON Object: should NOT have additional properties`**: Resolved by stripping non-standard top-level blocks like `keycodes` and `customKeycodes` that VIA's parser rejects.
    

## ✨ Features

- **Split Encoder Support**: Modified matrix and keymap definitions to recognize and map a split encoder hardware mod.
    
- **Translated Interface**: English translations for original Chinese system functions and RGB menus.
    
- **VIA V2 Compatibility**: Optimized for the "Use V2 definitions (deprecated)" workflow in modern VIA clients.
    

## 🚀 Quick Start

1. **Download** the `Wave75_Split_Encoder_Fixed.json` from this repo.
    
2. Open the [VIA Web App](https://usevia.app/).
    
3. Navigate to the **Settings** tab and enable **Show Design tab**.
    
4. In the **Design** tab, toggle **Use V2 definitions (deprecated)** to **ON**.
    
5. Drag and drop the fixed `.json` file and connect your Wave75.
    

---
