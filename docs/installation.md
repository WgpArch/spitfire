# Installation Guide

## Prerequisites

Ensure you have the following packages installed:

```bash
sudo pacman -S waybar swaybg nm-applet swaync grim libnotify rofi lxterminal
Available via the AUR
trizen -S paru -S yay -S spitfire

Manual installation 
git clone https://github.com/dani-77/spitfire.git
cd spitfire
sudo make install

This specific repository
1 Clone the Repository
git clone git@github.com:WgpArch/spitfire.git ~/dotfiles/spitfire

2 Deploy Configuration
cp -r ~/dotfiles/spitfire/configs/spitfire ~/.config/spitfire

3 Verify Directory Structure
Your ~/.config/spitfire/ should contain:
config.lua (main compositor config)
rofi/ (launcher & powermenu scripts/styles)
waybar/ (bar config & CSS)
screenshots/ (auto-captured images)

4 Launch
Select "spitfire" from your display manager session menu or run spitfire from a TTY.

Troubleshooting

No Waybar? Ensure paths in config.lua autostart match your actual file locations.
Screenshot Fails? Verify ~/Pictures/Screenshots/spitfire/ exists and is writable.
Workspace Limit? Confirm spitfire.workspace.max = 12 is set in config.lua.
