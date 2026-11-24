# Sway profiles

From `~/dotfiles`, install the shared packages and one machine profile with GNU Stow.

```sh
stow sway waybar scripts foot fuzzel mako swaylock laptop
~/.local/bin/machine-init
```

On the dual-monitor desktop, replace `laptop` with `desktop`. To switch an existing installation, unstow the old profile first, for example with `stow -D laptop`. Choose Sway at login (Sway (NVIDIA) on the NVIDIA desktop).

The laptop uses the top bar. The desktop profile owns its bottom bar, wallpaper, monitor layout, and keyboard swap. Local monitor and input overrides go in `~/.config/machine/sway.conf`.

Both profiles read bindings from `sway/.config/sway/config`. Super+I opens the shortcut sheet, Super+D opens the launcher, and Super+Escape opens the power menu.
