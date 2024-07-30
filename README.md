# Neverlose Library

## Booting the Library
```lua
local NEVERLOSE = loadstring(game:HttpGet("https://raw.githubusercontent.com/3345-c-a-t-s-u-s/NEVERLOSE-UI-Nightly/main/source.lua"))()
```

## Change theme (**REQUIRED**)

```lua
NEVERLOSE:Theme("dark") -- [ dark , nightly , original ]
```

## Create Window

```lua
local Window = NEVERLOSE:AddWindow("NEVERLOSE", "TEXT HERE")
```

## Create Tab 

```lua
local MainTab = Window:AddTab('Test', 'ads')
```

## Create Section

```lua
local Example = ExampleTab:AddSection('Example', "left")
```

## Create Label 
```lua
Example:AddLabel("Label")
```

## Create Buttons

```lua
Example:AddButton("Button Example", function()
	print("Button")
end)
```

## Create Toggles

```lua
Example:AddToggle('Toggle', false, function(val)
	print("Toggle", val)
end)
```

## Create Keybind

```lua
Example:AddKeybind('Keybind', Enum.KeyCode.X, function(val)
	print('keybind', val)
end)
```

## Create Slider
```lua
Example:AddSlider('Slider', 1, 100, 50, function(val)
	print('slider', val)
end)
```

## Create Dropdown
```lua
Example:AddDropdown('Dropdown', {1, 2, 3}, 2, function(val)
	print("dropdown", val)
end)
```

# Key System

```lua
local NEVERLOSE = loadstring(game:HttpGet("https://raw.githubusercontent.com/3345-c-a-t-s-u-s/NEVERLOSE-UI-Nightly/main/source.lua"))()

local function Start(Key)
	local Window = NEVERLOSE:AddWindow("NEVERLOSE", "TEXT HERE")
end

local KeySystem = NEVERLOSE:KeySystem("Key System", "https://discord.gg/bedol-hub", function(key)
	if key=='1234' then
		return true
	end
	return false
end)

KeySystem:Callback(Start)
```
