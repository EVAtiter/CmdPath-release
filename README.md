[English](README.md) | [日本語](README.ja.md)

# CmdPath

A macOS menu-bar utility that shows the folder hierarchy menu when you **⌘ (Command)-click** the title (folder name)
of a Finder window.

In the Finder on macOS 27.2, ⌘-clicking the title no longer shows the hierarchy menu. CmdPath brings this back and shows
**the Finder's own hierarchy menu** as it is.

---

## Download

Download the latest version from [Releases](https://github.com/EVAtiter/CmdPath-release/releases/latest).

1. Unzip `CmdPath-x.x.x.zip` and move `CmdPath.app` to the Applications folder
2. When you open it, CmdPath explains that it needs Accessibility permission. Click Continue, then Open System Settings,
   and turn on CmdPath in **System Settings → Privacy & Security → Accessibility**
3. CmdPath starts working when the Finder is in front

You can also install it with Homebrew.

```bash
brew install --cask EVAtiter/tap/cmdpath
```

If Homebrew 7 or later reports an "untrusted tap", trust cmdpath first with the command below, then install again.

```bash
brew trust --cask evatiter/tap/cmdpath
```

---

## How to use

In a Finder window, ⌘-click the folder name in the title (or the folder icon to its left).
A menu appears with the current folder and the folders above it. Choose the one you want to go to.

- Also works on the title of a Finder window in the background (while the Finder is in front)
- Works regardless of tabs, window size, and how the toolbar is shown
- The cursor does not move

---

## Features

- **Hierarchy menu with ⌘-click** — Shows the Finder's own menu as it is (CmdPath does not draw its own menu)
- **Turn on / off** — From the menu bar
- **Open at Login**
- **Hide the menu bar icon** — CmdPath keeps working while the icon is hidden. To show it again, open CmdPath again
- **Japanese / English** — Shown in English when the system language is not Japanese (since 1.1.0)

---

## Notes

- CmdPath works only while the Finder is in front. It changes only a left-click with ⌘ alone held down that lands on a
  Finder window title. Normal clicks, right-clicks, and other apps are not affected
- If you ⌘-click right after moving the cursor onto the title (within about 0.3 seconds), nothing happens. Click again
- ⌘-dragging on the title shows the menu instead
- If you turn off Accessibility permission while CmdPath is running, clicks are not accepted for about 10 seconds
  (they come back on their own). Quit CmdPath before turning off the permission
- Not yet tested with external displays or with displays that use different scaling

---

## Privacy

CmdPath does not use the network. It does not record what you do or store personal information. It does not modify the
Finder, inject code, or use private APIs.

---

## Requirements

macOS 14 Sonoma or later (tested on macOS 27.2) / Apple Silicon (arm64) only / Notarized by Apple

---

Copyright © 2026 EVA Titer. All rights reserved.
