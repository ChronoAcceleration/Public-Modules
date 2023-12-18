# Public Modules

Welcome to the Public Modules repository! This repository contains a collection of Roblox module scripts developed by me. The first module available is the Glitcher module, designed for introducing glitch effects in your Roblox game.

## Glitcher Module

### Overview

The Glitcher module provides a simple and customizable way to add glitch effects to your Roblox game. It includes functions for manipulating sounds, displaying UI elements, and creating glitch effects on demand.

### Usage

#### Creating a Glitcher Object

To use the Glitcher module, create a new Glitcher object by calling the `Glitcher.new(Player)` function, where `Player` is the player to whom the glitch effects will be applied.

```lua
local Glitcher = require(game.ServerScriptService:WaitForChild("GlitcherModule"))

local player = game.Players.LocalPlayer
local glitcherInstance = Glitcher.new(player)
```

#### Triggering Glitch Effects

Once you have a Glitcher object, you can trigger glitch effects by calling the `Glitcher:Glitch()` method.

```lua
glitcherInstance:Glitch()
```

This will play glitch sounds, display UI elements, and create glitch effects.

#### Removing Glitcher Object

To remove the Glitcher UI and clean up resources, call the `Glitcher:Remove()` method.

```lua
glitcherInstance:Remove()
```

### Example

```lua
-- Example usage of the Glitcher module
local Glitcher = require(game.ServerScriptService:WaitForChild("GlitcherModule"))

local player = game.Players.LocalPlayer
local glitcherInstance = Glitcher.new(player)

-- Trigger glitch effects
glitcherInstance:Glitch()

-- Wait for a while...

-- Remove Glitcher UI
glitcherInstance:Remove()
```

### Note

Make sure to include the Glitcher UI (`GlitcherUI`) within your game's GUI for the module to work correctly.

Feel free to explore and customize the Glitcher module to suit your game's aesthetic and requirements. If you encounter any issues or have suggestions, please feel free to [report them](https://github.com/your-repository/issues).

Happy glitching!
