---
title: HanziKey Support
---

# HanziKey Support

HanziKey is a pop-up Mandarin dictionary for macOS. Look up Chinese
in any app via selection hotkey, drag-region translate, or
cursor-driven hover dictionary. Fully on your Mac.

The three hotkeys, at a glance:

- **⌘⇧Y: Show Translation Popup for Selected Text.** Select text in
  any app and press this for a breakdown popup.
- **⌘⇧O: Translate Region.** Drag-select a rectangle on screen and
  see a full translation plus per-word breakdown.
- **⌘⇧I: Translate Source.** Open the unified reading panel; pick
  a source (region, screen, or window) and hover words for
  definitions, or toggle to Passage view for the full translation.

There's also an optional fourth hotkey, **Convert Numbered Pinyin to
Tone Marks**, that turns `ni3 hao3` into `nǐ hǎo` in any editable
text field. It's disabled by default; enable and bind it from the
menu bar icon → Settings → Hotkeys if you want it.

## Common questions

### The translation popup doesn't appear when I press ⌘⇧Y

HanziKey needs Accessibility permission to read your selected text.

1. Open **System Settings → Privacy & Security → Accessibility**
2. Toggle HanziKey on (use the **+** button to add it if it's not listed)
3. Quit and relaunch HanziKey

If the toggle is already on but the hotkey still doesn't work, remove
HanziKey from the list, then re-add it and re-grant permission. macOS
sometimes caches a stale entry from a previous version of the app.

### The screen capture features (⌘⇧O / ⌘⇧I) don't work

These need Screen Recording permission.

1. Open **System Settings → Privacy & Security → Screen Recording**
2. Toggle HanziKey on
3. **Quit and relaunch HanziKey.** macOS doesn't apply the new permission
   to a running app.

### I downloaded from the Mac App Store but already had the DMG installed (or vice versa)

That's fine. Both builds use the same bundle identifier and the same
on-disk settings. One small wrinkle: macOS keys Accessibility and
Screen Recording permissions by the binary's signing fingerprint, and
the App Store version and DMG version sign with different certificates.
After switching, macOS will ask you to grant permissions again. Toggle
HanziKey on in both Privacy lists and quit / relaunch the app.

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
