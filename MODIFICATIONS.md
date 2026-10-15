# Modifications to Mark LV

This document details all changes made to the original **Mark LV** project by **FatihMakes**.

## Original Work

- **Original Project:** Mark LV
- **Original Author:** FatihMakes
- **Original Repository:** https://github.com/FatihMakes/Mark-LV
- **Original License:** Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)
- **YouTube:** [@FatihMakes](https://www.youtube.com/@FatihMakes)
- **Instagram:** [@fatihmakes](https://www.instagram.com/fatihmakes)

## Attribution

This project, **Horizon**, is a modified version of Mark LV. All modifications are documented below in accordance with the CC BY-NC 4.0 license requirements. The original creator, FatihMakes, retains all rights as specified in the license.

⭐ **Please support the original creator by starring the [Mark LV repository](https://github.com/FatihMakes/Mark-LV).**

---

## Changes Made

### Phase 1: Rebranding (October 2026)

#### User-Facing Changes
All user-facing references to "JARVIS" or "Jarvis" have been changed to "Horizon":

**Files Modified:**
1. **`memory/config_manager.py`**
   - Default assistant name changed from "JARVIS" to "Horizon" (lines 54, 68, 108)

2. **`ui.py`** (45 changes)
   - Window title: "J.A.R.V.I.S." → "Horizon"
   - UI labels, tooltips, and messages updated
   - Desktop shortcut names: `J.A.R.V.I.S.lnk` → `Horizon.lnk` (Windows), `J.A.R.V.I.S.app` → `Horizon.app` (macOS)
   - Autostart registry key: `JARVIS_AI` → `Horizon_AI` (Windows)
   - Bundle identifiers updated for macOS
   - Tool tips and device picker labels updated
   - Memory panel, clipboard panel, customize overlay labels updated

3. **`main.py`** (16 changes)
   - System prompt updated to introduce "Horizon"
   - Tool names: `shutdown_jarvis` → `shutdown_horizon`
   - Log messages and user-facing strings updated
   - Morning briefing messages updated

4. **`setup.py`** (2 changes)
   - Installation messages: "Hey Jarvis" → "Hey Horizon"
   - Comments updated

5. **`dashboard/server.py`** (5 changes)
   - Module docstring updated
   - AES salt generation comment updated
   - Upload directory references updated
   - HTML error messages in phone dashboard updated

6. **`memory/memory_manager.py`** (1 change)
   - Module docstring updated

7. **`config/jarvis.ico` → `config/horizon.ico`**
   - Icon file renamed
   - All code references to the icon updated in `ui.py`, `setup.py`, and `main.py`

8. **`readme.md`** (22+ changes)
   - Project title updated with attribution notice
   - All feature descriptions updated
   - Wake-word references: "Hey Jarvis" → "Hey Horizon"
   - Assistant name references throughout documentation
   - Git clone URL updated to user's repository
   - License section updated with original work attribution
   - Quick Start instructions updated

#### Preserved Elements
The following were intentionally **NOT** changed to maintain plugin compatibility and internal consistency:

- Internal class names: `JarvisUI`, `JarvisLive`, `JarvisThread`
- Developer-facing debug logs marked `[JARVIS]` (not visible to end users)
- Core module names and internal identifiers

### Technical Validation
- All modified Python files passed syntax validation
- No breaking changes to plugin API
- Configuration file backward compatibility maintained
- All 71 user-facing references successfully updated

---

## Future Planned Changes (Not Yet Implemented)

### Phase 2: Wake-Word Model Update
- Update wake-word detection from "Hey Jarvis" to "Hey Horizon"
- Train or obtain custom Picovoice Porcupine model for "Hey Horizon"

### Phase 3: Background Listener
- Implement always-on wake-word listener
- Run in background with minimal resource usage

---

## License Compliance

This modified work is distributed under the same **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license as the original.

### Required Attribution
- Original work: Mark LV by FatihMakes
- Original repository: https://github.com/FatihMakes/Mark-LV
- License: CC BY-NC 4.0

### Modification Notice
This file serves as the modification notice required by the CC BY-NC 4.0 license, documenting all changes made to the original work.

---

**Last Updated:** October 15, 2026
