# Sulfate Lib - Alpha Docs

# Starting the library

```lua
local SulfateLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/Grayy12/SulfateLib-alpha/main/Sulfate.lua?token=GHSAT0AAAAAABXMGZCWGQ4MUMC3WOQHY5VCYXSRJ5A",true))()
```


# Creating a Window

```lua
local window = SulfateLib:Window()
```

# Creating a Tab

```lua
local MainTab = window:CreateTab({
	name = "MainTab",
	description = "This is the main tab description",
})

--[[
name = <string> - The name of the Window
description = <string> - A Description for the Window
]]--
```

# Creating a Section

```lua
MainTab:CreateSection({
	name = "Button Section",
})

--[[
name = <string> - The Name of the Section
--]]
```

# Creating a Button

```lua
MainTab:CreateButton({
	name = "Button",
	callback = function()
		print("Clicked button")
	end,
})

--[[
name = <string> - The Name of the Button
callback = <function> - The Function of the Button
]]--
```

# Creating a Toggle

```lua
MainTab:CreateToggle({
	name = "Toggle",
	default = false,
	callback = function(value)
		print(value)
	end,
})

--[[
name = <string> - The Name of the Toggle
default = <bool> - The default value of the Toggle
callback = <function> - The Function of the Toggle
]]--
```

# Creating a Slider

```lua
MainTab:CreateSlider({
	name = "slider",
	minvalue = 0,
	default = 0,
	maxvalue = 100,
	callback = function(value)
		print(value)
	end,
})

--[[
name = <string> - The Name of the Toggle.
minvalue = <number> - The Minimum value of the Slider.
default = <number> - The default value of the Slider.
maxvalue = <number> - The Maximum value of the Slider.
callback = <function> - The Function of the Toggle.
]]--
```

# Creating a Notification

```lua
SulfateLib:CreateNotification({
	title = "Test",
	content = "Test content",
	time = 5,
})

--[[
title = <string> - The Title of the Notification.
content = <string> - The Content of the Notification.
time = <number> - The Amount of time the Notification is on screen.
]]--
```
