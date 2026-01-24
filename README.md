# GOMove UI for TrinityCore 3.3.5a

An updated GOMove UI for TrinityCore 3.3.5a. Originally created by [rochet2](https://github.com/Rochet2/TrinityCore/tree/gomove_3.3.5/src/server/scripts/Custom/GOMove).

## Features

### Core Features
- **Position Controls**: Move objects in any direction using compass-style buttons (N, S, E, W, NE, NW, SE, SW)
- **Vertical Movement**: Up/Down buttons for Z-axis movement
- **Snap Controls**: X, Y, Z, O buttons to snap object position/orientation to player position
- **Info Button**: Display detailed information about selected gameobjects
- **Pitch/Roll/Turn Sliders**: Full rotation control with mousewheel support for fine-tuning

### New Features
- **Scale Control**: Slider to resize gameobjects (10% to 500%)
- **Copy/Paste**: Copy selected object to clipboard and paste new instances at your location
- **Grid Snap**: Toggle grid snapping for precise object alignment
- **Tooltips**: Descriptive tooltips for all buttons explaining their function
- **Keyboard Shortcuts**: Optional keyboard shortcuts (Delete, Insert, Ctrl+P)
- **Additional Slash Commands**: Extended command list for power users

## Slash Commands

| Command | Description |
|---------|-------------|
| `/gomove` | Toggle the main UI window |
| `/gomove help` | Show all available commands |
| `/gomove reset` | Reset all frame positions to defaults |
| `/gomove resetsliders` | Reset all sliders to default values |
| `/gomove copy` | Copy selected object to clipboard |
| `/gomove paste` | Paste object from clipboard |
| `/gomove grid` | Toggle grid snap on/off |
| `/gomove gridsize <n>` | Set grid snap size |
| `/gomove scale` | Show current scale value |
| `/gomove selectall` | Select all objects in the selection list |
| `/gomove clearselection` | Clear current selection |
| `/gomove invertselection` | Invert current selection |
| `/gomove keybinds` | Enable/disable keyboard shortcuts |
| `/gomove clearundo` | Clear undo history |

## Keyboard Shortcuts (when enabled)

| Key | Action |
|-----|--------|
| `Delete` | Delete selected objects |
| `Insert` | Select nearest object |
| `Ctrl+P` | Paste copied object |

## Installation

1. Place the `GOMove` folder in `<WoW Installation Folder>\Interface\Addons`
2. Place the `GOMove.cpp`, `GOMoveScripts.cpp`, and `GOMove.h` files in `<Trinity Installation Folder>\src\server\scripts\Custom\GOMove` folder
3. Update your `custom_script_loader.cpp` file to reference the new custom script
4. Build your Trinity server with CMake
5. Build your Trinity Visual Studio solution
6. Login and type `/gomove` to open the UI (should be open by default)

## UI Sections

1. **Position** - Compass-style directional movement controls
2. **Rotation** - Pitch, Roll, and Turn sliders for full rotation control
3. **Scale** - Object scaling with slider and quick buttons
4. **Tools** - Select, Snap, Delete, Ground, Floor, Go To, Respawn, Copy, Paste, Info, Grid
5. **Spawn** - Spawn new objects by entry ID
6. **Lists** - Access Favourites and Selections lists

## Credits

- Original GOMove by [Rochet2](http://rochet2.github.io/)
- Original concept by Mordred
- Port as AC-Module and rework by Tralenor
- Objscale integration partly from Magnus
