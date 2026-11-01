# Waybar & Scripts

## Configuration Structure

Waybar is configured as an external client bar via `spitfire.autostart()`:

```lua
"waybar -c ~/.config/spitfire/waybar/config.jsonc -s ~/.config/spitfire/waybar/style.css"

Key Components

config.jsonc: Defines modules (workspaces, clock, weather, network, etc.)
style.css: Implements the Gold & Navy theme with sheer transparency
powermenu.sh: Rofi-based power menu script in rofi/ directory
spitfire.rasi: Rofi styling matching Waybar's color palette

Workspace Module
The workspace module uses ext-workspace-v1 protocol to display all 12 workspaces dynamically. Active workspace is highlighted with gold (#d4b483), inactive with navy (#414868).
