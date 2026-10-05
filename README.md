# Sekiro: Shadows Die Twice - Custom Cheat Engine Table

A robust, feature-rich Cheat Engine table (`.CT`) specifically configured for the single-player game *Sekiro: Shadows Die Twice*. This table provides a versatile range of modifications, from financial and progression enhancements to advanced physics, movement, and defensive controls.

---

## 🚀 Core Features

### 💰 Economy & Inventory Controls
* **Infinite Money / Credits**: Freezes or forces your current money balance. (Default: `9999` / Hex `270F`).
* **Specific Infinite Item Usage**: Prevents items from decreasing, but *only* activates on the specific item you currently use (does not blindly overwrite everything to 20 at once).
* **Double Enemy Loot**: Instantly doubles the dropped reward quantities whenever you harvest loot from defeated enemies.
* **Freeze Inventory & Equipment**: Automatically forces and freezes all item counts in your active equipment slots and inventory tabs straight to `#10`.

### 📈 Skill Points & Progression
* **Instant Skill Points**: A standalone script that safely forces rapid progression without sharing overlapping opcodes. Defeating an enemy will instantly fill your progression bar.
* **Skill Points Multiplier (SP M.P)**: Multiplies incoming experience/skill points. (Default value: `1500`).

### ⚔️ Combat & Stealth Mechanics
* **Stealth Mode (Undetected by Enemies)**: Complete ghost visibility tracking. Enemies and cameras lose the ability to detect you entirely. 
  * 🎛️ **Hotkey:** `~` (Tilde key) toggles this option on and off.
* **God Mode**: Complete protection from incoming vitality damage.
* **God Mode + Infinite Resurrection**: Keeps you alive and ensures resurrection targets are frozen to safe maximums.
  * 🎛️ **Hotkey:** `F1` (Press only when a fatal strike lands to safely cycle states).
* **1-Hit Kill**: Dynamically scales enemy vitality damage downward, forcing target health pools directly to `1` or lower on impact.
* **Damage Multiplier (D M.P)**: amplifies your natural physical output. (Default offset value: `80`).
* **Boss Long-Fight Mode (1 HP Challenge)**: Forces your offensive strikes to deal exactly `1 HP` of real damage to boss encounters, intentionally dragging out fights for practicing deflection pacing.

### 🛡️ Deflection & Parry Automation
* **Auto Parry / Deflect Attack**: Automates defensive logic to perfectly step into windows or execute counter-deflections precisely as strikes hit.
  * 🎛️ **Hotkey:** Numpad `9` toggles status tracking.
* **Aggensive Strike-Parry**: Forces clean guard-breaking parameters and active frames to execute defensive parries while you are mid-animation attacking an enemy.
* **Poison Guard-Break**: Slowly strips down structural posture while actively administering poison downscaling directly to all nearby hostile targets (Default value: `#66`).

### 🌍 Physics, Flight & Movement Modifiers
* **Speed Multiplier**: Increases overall engine velocity mechanics cleanly. 
  * 🎛️ **Hotkey:** `F2` toggles overall speed (Includes integrated activation audio cues).
* **Super Jump Modifiers**: Two independent tiers (`Level 1` and `Level 2`) to heavily boost vertical leap physics.
* **Jump to Fly (Float Mode)**: Freezes vertical launch coordinates. When you jump, you float indefinitely in place. Perfect for exploration.
* **Teleport Jump**: Launches you heavily forward into your current directional orientation as you jump. 
  * 🎛️ **Hotkey:** `F3` toggles this system (Note: Grappling hooks are disabled while active).
* **Walk in Air / Flight Mode**: Completely freezes your Y-Axis velocity grids allowing you to freely maneuver through the environment.
  * 🎛️ **Hotkey:** `F4` to freeze/unfreeze coordinates mid-air.
* **Superman Jump Mode**: Extreme acceleration curve calculations applied strictly to running trajectory vectors.
  * 🎛️ **Hotkey:** `F5` triggers flight pacing vectors.

---

## ⚙️ Customization Guidelines

Several scripts feature explicit external pointers that you can manually fine-tune by double-clicking the raw variable value row inside Cheat Engine:

1. **Custom Wealth Allocations:** Open up the main structure script header for the *Infinite Money* entry to manually modify the default `270F` allocation hex limits to your preferred balance.
2. **Adjusting Skill Points Curve:** Double-click the green entry reading `1500` under the **SP M.P** sub-tree and scale it up to values like `3000` or `5000` to maximize leveling speed.
3. **Adjusting Damage Scales:** Double-click the green entry reading `80` under the **D M.P** sub-tree to scale it up to `100`, `200`, or beyond for hyper-customized damage output.
4. **Binding Your Own Hotkeys:** To re-map any script to a different key, right-click the desired script row in Cheat Engine, select **Set/Change Hotkeys**, or use the keyboard shortcut `Ctrl + H`.

---

## ⚠️ Safe Usage & Save Game Security

Because *Sekiro* is an offline single-player experience, running these scripts poses **no ban risks** via external anti-cheat servers. However, to guarantee your local save file does not become corrupted from data freezes:

* Avoid force-saving or triggering automated Sculptor's Idol checkpoints while actively running hyper-extended environmental float hacks or coordinate freezes like *Walk in Air* or *Jump to Fly*.
* Back up your directory save folder (`%APPDATA%\Sekiro\`) regularly before performing heavy memory value overwrites.

---

## ⚖️ Terms & Disclaimer
This framework is distributed strictly for **personal offline use, behavioral analysis, and gameplay modification research**. All code adjustments, pointer structures, and offset maps have been developed independently. All original copyrights, trademark configurations, and engine code files belong exclusively to FromSoftware and Activision.
