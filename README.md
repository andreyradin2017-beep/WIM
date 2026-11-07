# WIM (WoW Instant Messenger)

WoW 3.3.5a (WotLK) addon that turns whispers and other chat into separate IM-style message windows.

This repository is based on WIM v3 and includes local compatibility/fixes for running on the Sirus private server client (`## Interface: 30300`).

## Features

- Separate message window for each whisper/chat target.
- Window tabs, history browser, filters, and emoticons.
- Minimap icon, options UI, slash commands, URL handling.
- Bundled libraries (`LibStub`, `Astrolabe`, `LibSharedMedia-3.0`, etc.).
- Saved settings and history through WoW SavedVariables.

## Installation

1. Copy the whole `Wim` folder to:

   ```
   World of Warcraft/Interface/AddOns/Wim
   ```

   The folder name must stay `Wim`.
2. Restart the game or run `/reload`.
3. Enable the addon in the AddOns menu if needed.

## Usage

- `/wim` or `/wim help` — show available slash commands.
- `/wim options` — open settings.
- `/wim history` — open the history viewer.
- `/wim rl` — reload the UI.

## Requirements

- WoW client 3.3.5a / Interface 30300.
- No separate library installation is required; dependencies are bundled in `Libs/`.

## Notes

- Settings and history are stored in SavedVariables (`WIM3_Data`, `WIM3_History`, etc.).
- If WIM does not open windows, check that it is enabled for the current character in `AddOns.txt` and inspect `Logs/FrameXML.log`.
- The `Wim-main` nested copy was removed from this tree; the addon root itself is the active version.