<div align="center">

<img width="1774" height="887" alt="Flux Theme Enabler" src="https://github.com/user-attachments/assets/8bad13e2-2730-4274-84aa-3a0e58d32500" />

<img src="https://img.shields.io/badge/FluxThemeEnabler-v3.2-blueviolet?style=for-the-badge&logo=android" alt="FluxThemeEnabler"/>
<br/>
<img src="https://img.shields.io/badge/RealmeUI%207%20%7C%20ColorOS16-Supported-brightgreen?style=for-the-badge"/>
<img src="https://img.shields.io/badge/OxygenOS16-Supported-orange?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Root-Magisk%20%7C%20KernelSU%20%7C%20APatch-red?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Telegram-colorosmodules-blue?style=for-the-badge&logo=telegram"/>

# ✨ Flux_Theme_Enabler

### Enable O+ Flux Theme 2.0 wallpapers, resources & effects on RUI7 / COS16 / OOS16

Made with ♥ by **[Ayan (@imnotaino)](https://t.me/imnotaino)**  
Updates & Support → **[t.me/colorosmodules](https://t.me/colorosmodules)**

</div>

---

# 📖 What is this?

**Flux_Theme_Enabler** is a specialized Magisk / KernelSU / APatch module designed to fully enable the new **O+ Flux Theme 2.0** experience on:

- Realme UI 7
- ColorOS 16
- OxygenOS 16 (separate branch)

A lot of ports and unofficial builds either:
- fail to load Flux wallpapers
- lose wallpaper access permissions
- break wallpaper parsing
- revert theme mounts after boot
- partially register OPLUS resources

This module fixes the entire chain properly using:
- system-less bind mounts
- permission correction
- SELinux context patching
- late-boot remount protection
- Flux resource registration

without modifying `/system`.

The result:
- fully working Flux wallpapers
- stable theme mounting
- proper wallpaper rendering
- fixed wallpaper crashes
- premium O+ visual experience

---

# ✨ Features

| Feature | Description |
|---|---|
| 🌌 **Flux Theme 2.0 Enabled** | Unlocks O+ Flux resources & wallpapers |
| 🖼️ **Wallpaper Permission Fix** | Fixes wallpaper loading & access crashes |
| 🔒 **SELinux Context Repair** | Applies proper readable system contexts |
| 🔁 **Late-Boot Mount Protection** | Prevents ColorOS remount override issue |
| ⚡ **Stylized Flash Installer** | Premium slow-print flashing sequence |
| 🛡️ **System-less Overlay** | No direct partition modification |
| 📱 **OPlus Optimized** | Built specifically for COS16/OOS16/RUI7 |

---

# 🛠️ Wallpaper Permission Bug Fixed

One of the biggest issues with Flux ports is broken wallpaper access.

Normally, bind mounting directly from:

```bash
/data/adb/modules/
```

causes:
- permission denied errors
- wallpaper loading failures
- inaccessible resources
- theme crashes

especially inside:
- Wallpaper app
- Theme Store
- SystemUI resource parser

---

## 📸 Flash Preview

```text
╔══════════════════════════════════════╗
║            O+ Flux Theme             ║
║          Wallpaper Enabler           ║
╚══════════════════════════════════════╝

  Developer : Ayan (@imnotaino)
  Channel   : t.me/colorosmodules

  Flash Time : 2026-05-18 09:47:36

──────────────────────────────────────
          ★  Device  Info  ★
──────────────────────────────────────
  Device  : realme Narzo 60x
  Codename: ossi
  Android : 16  (SDK 36)
  Build   : RMX3782_16.0.0.xxx
  Kernel  : 5.15.x
  Battery : 84%
──────────────────────────────────────

  ► Initialising environment...
  ► Verifying root access...
  ► Verifying OS compatibility...
  ► Extracting wallpaper resources...
  ► Patching Wallpaper configuration...
  ► Registering OPLUS Flux theme...
  ► Mounting decoupling wallpaper...
  ► Optimizing theme database...
  ► Cleaning temporary files...

══════════════════════════════════════
    ✓ O+ Flux Theme Enabler Ready!
══════════════════════════════════════

  ➤  t.me/colorosmodules

  Made with ♥ by Ayan (@imnotaino)
```

---

# 📦 File Structure & Components

| File | Purpose |
|---|---|
| `module.prop` | Module metadata & credits |
| `post-fs-data.sh` | Early boot mount & permission handler |
| `service.sh` | Late-boot remount protection |
| `customize.sh` | Premium flashing sequence |

---

# ⚙️ What the module patches

The module safely overlays:
- Flux wallpapers
- OPLUS theme resources
- Wallpaper parser configs
- Mount points

without modifying:
- `/system`
- `/vendor`
- `/odm`

Everything remains:
- reversible
- removable
- system-less


---

# 🚀 Installation

1. Download latest `Flux_Theme_Enabler.zip`
2. Open:
   - Magisk
   - KernelSU
   - APatch
3. Go to **Modules**
4. Select **Install from storage**
5. Flash the ZIP
6. Reboot device

After reboot:
- Flux resources mount automatically
- Wallpaper access is restored
- Theme remains persistent across boot

---

# ❓ FAQ

## Q: Will this work on Android 15?

Partially.

The module is mainly optimized for Android 16 branches.

---

## Q: Does this replace stock wallpapers?

No.

It only overlays and enables Flux resources.

---

## Q: Why was wallpaper crashing before?

Because Android system apps couldn't properly access bind-mounted resources due to permission and SELinux restrictions.

---

## Q: Why is `service.sh` needed?

Because ColorOS remounts `/my_product` during late boot and destroys early mounts.

Without late-boot protection the theme disappears after boot.

---

## Q: Is this safe to uninstall?

Yes.

Disable/remove the module and reboot.

Everything reverts automatically.

---

# 📢 Telegram Channel

For updates, support, and future ColorOS modules:

### 👉 https://t.me/colorosmodules

---

# 👤 Credits

| Role | Name |
|---|---|
| Developer | Ayan (@imnotaino) |
| Target OS | RUI7 / COS16 / OOS16-Separate branch |
| Theme | O+ Flux Theme 2.0 |

---

<div align="center">

### Made with ♥ by Ayan (@imnotaino)

t.me/colorosmodules

</div>
