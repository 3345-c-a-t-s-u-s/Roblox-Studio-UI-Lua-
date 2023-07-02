# Roblox Studio UI 

## Create Window
```lua
local RobloxStudioUI = loadstring(game:HttpGet("https://raw.githubusercontent.com/3345-c-a-t-s-u-s/Roblox-Studio-UI-Lua-/main/source.lua"))()

local Window = RobloxStudioUI:NewWindow("Roblox Studio UI","Role Of Player")
```
## Create Section
```lua
local Section = Window:NewSection("Scetion",Module.ImageIcon.Server,Color3.fromRGB(0, 115, 255))
```

## Create Assets
```lua
Section:NewDropdown("Dropdwon",{"1","2","3"},function(Stats)
	print(Stats)
end)

Section:NewLabel("Label")

Section:NewButton("Button",function()
	print('is click')
end)

Section:NewSlider(1,100,function(number)
	print(number)
end)

Section:NewToggle("Toggle",false,function(boolen)
	print(boolen)
end)

Section:NewKeybinds("Key",Enum.KeyCode.X,function(newkey)
	print(newkey)
end)
```

# Assets Opstion

## Dropdown
```lua
Dropdown:Set({"4","5","6"})
Dropdown:Refresh()
```

## Label
```lua
Label:Set("New Label")
```
## Button
```lua
Button:Set("New Label")
```
## Slider
```lua
Slider:Set(50) -- Number
```
## Toggle
```lua
Toggle:Set(false) -- boolen
```
## Keybind
```lua
Keybind:Set(Enum.KeyCode.J)
```
