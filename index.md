---
title: HanziKey Support
---

# HanziKey Support

HanziKey is a pop-up Mandarin dictionary for macOS. Translate Chinese
text in any app via hotkey, region OCR, or live capture — fully on
your Mac.

## Get in touch

Email **mikespearman.e@gmail.com**

Please include:

- Your macOS version (Apple menu → About This Mac)
- The HanziKey version (HanziKey menu bar → Settings → bottom of window)
- A brief description of what you were trying to do

I read every message.

## Common questions

### The translation popup doesn't appear when I press ⌘⇧Y

HanziKey needs Accessibility permission to read your selected text.

1. Open **System Settings → Privacy & Security → Accessibility**
2. Toggle HanziKey on (use the **+** button to add it if it's not listed)
3. Quit and relaunch HanziKey

If the toggle is already on but the hotkey still doesn't work, remove
HanziKey from the list, then re-add it and re-grant permission. macOS
sometimes caches a stale entry from a previous version of the app.

### The screen capture features (⌘⇧O / ⌘⇧L) don't work

These need Screen Recording permission.

1. Open **System Settings → Privacy & Security → Screen Recording**
2. Toggle HanziKey on
3. **Quit and relaunch HanziKey** — macOS doesn't apply the new permission
   to a running app

### A translation looks wrong or a definition is missing

HanziKey uses [CC-CEDICT](https://cc-cedict.org/) for dictionary data, which
is a community-maintained dataset. Occasionally entries have gaps or
unusual definitions. Email me the word and I'll either flag it for the
CC-CEDICT maintainers or note the limitation in a future update.

### The hotkey conflicts with another app

You can rebind any HanziKey hotkey from the menu bar icon → Settings →
Hotkeys section. Click the current shortcut and press the new combination.

### Where is my saved data stored?

HanziKey doesn't sync to any servers and doesn't create accounts. App
preferences are stored locally in macOS's standard UserDefaults
(`~/Library/Containers/com.michaelspearman.hanzikey/`). To reset to
defaults, delete that folder while the app is quit.

## Requirements

- macOS 15.0 (Sequoia) or later
- Accessibility permission (used only when you press the selection hotkey)
- Screen Recording permission (used only when you press an OCR hotkey)

## Privacy

See the [privacy policy](privacy.html) for details on data handling.

Short version: nothing leaves your Mac. No accounts, no servers, no
analytics.
