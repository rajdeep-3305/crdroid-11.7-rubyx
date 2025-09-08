# 📖 Flashing Guide for crDroid 11.7 (rubyx)

---

## 🔑 Prerequisites
- An **unlocked bootloader**
  👉 [Mi Unlock Tool](https://en.miui.com/unlock/index.html)  
- A **PC with platform tools installed (ADB + Fastboot)**  
  👉 [SDK Platform-Tools](https://developer.android.com/tools/releases/platform-tools)  
- Required files:
  - `boot.img`
  - `vbmeta.img` (only needed for first install)
  - `ROM.zip`

---

## 🛠 Flashing Recovery
1. Reboot phone into **fastboot mode**.  
2. (Optional, first install only) Flash `vbmeta.img`:
   ```bash
   fastboot flash vbmeta vbmeta.img

3. Flash the recovery image `boot.img`:

`fastboot flash boot boot.img`


4. Reboot into recovery:

`fastboot reboot recovery`


---

## 📦 ROM Installation

1. In recovery:

Go to Factory reset → Format data/factory reset.



2. Back to main menu → Apply update → Apply from ADB.


3. On PC, sideload the ROM:

`adb sideload ROM.zip`




---

## 🔧 Flashing Add-ons (Optional)

For vanilla ROMs (like crDroid), reboot recovery after ROM install:

Recovery → Advanced → Reboot to recovery

Sideload GApps or other modules:

`adb sideload gapps.zip`


You can also flash Magisk or other add-ons the same way.



---

## 🚀 First Boot

From recovery → Reboot → System

First boot may take 5–10 minutes.

Sit tight, let it finish setup… then enjoy crDroid 🎉


---
