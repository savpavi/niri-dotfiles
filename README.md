# niri-dotfiles (archived)

An early snapshot (September 2026) of my [Niri](https://github.com/YaLTeR/niri) configuration for Fedora: outputs, workspaces, window rules and keybindings in a single `config.kdl`.

This repository is no longer updated. The maintained Niri config, together with the rest of my desktop, lives in [savpavi/dotfiles](https://github.com/savpavi/dotfiles) under `config/niri/`.

## Notes

- Outputs are set for `DP-1` (2560×1440 @ ~180 Hz) and `DP-3` (1920×1080 @ ~120 Hz); adapt names and modes for your machine.
- It calls Noctalia, Ghostty, Dolphin, `hyprpolkitagent`, cliphist, Solaar, wpctl and playerctl; their own configs are not included.
- `Mod+W` launches a personal Looking Glass script for a Windows VM that is not part of this repo; remove or change that bind.

Validate before logging in:

```bash
niri validate --config ~/.config/niri/config.kdl
```
