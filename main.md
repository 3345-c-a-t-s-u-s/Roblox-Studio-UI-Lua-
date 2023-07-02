# Roblox Studio UI - Make your onwer Script Hub

## Request 
```lua
local RobloxStudioUI = loadstring(game:HttpGet("https://raw.githubusercontent.com/3345-c-a-t-s-u-s/Roblox-Studio-UI-Lua-/main/source.lua"))()
```
## Create Window
```lua
local Window = RobloxStudioUI:NewWindow("Roblox Studio UI","Role Of Player")
```
## Create Section
```lua
local Section = Window:NewSection("Section - Name",RobloxStudioUI.ImageIcon.Client,Color3.fromRGB(25, 255, 79))

--[[
1) Name - String
2) Image - RbxId or Image in Library
3) Color Of Image - Color3
]]
```

## Create Label
```lua
Section:NewLabel("Label - UI")

---- Changing the value

local Label = Section:NewLabel("Label - UI")

Label:Set("New Label - UI")

```
## Create Button
```lua
Section:NewButton("Button - UI",function()

---- Changing the value

local Button = Section:NewButton("Button - UI",function()
	
end)

Button:Set("New Label")
```
## Create Slider
```lua
Section:NewSlider(1,50,function(Value)

---- Changing the value

local Slider = Section:NewSlider(0,50,function(Value)
	
end)

Slider:Set(25)
```
## Create Toggle
```lua
Section:NewToggle("Toggle - UI",false,function(Boolen)

---- Changing the value

local Toggle = Section:NewToggle("Toggle - UI",false,function(Boolen)
	
end)

Toggle:Set(true)
```
## Create Dropdown
```lua
Section:NewDropdown("Dropdown - UI",{"1","2","3"},function(String)

---- Changing the value

local Dropdown = Section:NewDropdown("Dropdown - UI",{"1","2","3"},function(String)
	
end)

Dropdown:Set({"4","5","6"})
Dropdown:Refresh()	
```
## Create Keybinds
```lua
Section:NewKeybinds("Keybinds - UI",Enum.KeyCode.X,function(Key)
	
end)

---- Changing the value

local Keybinds = Section:NewKeybinds("Keyinds - UI",Enum.KeyCode.X,function(Key)
	
end)

Keybinds:Set(Enum.KeyCode.E)
```
