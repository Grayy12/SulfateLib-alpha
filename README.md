# Sulfate Lib - Alpha Docs

# Starting the library

```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/Grayy12/SulfateLib-alpha/main/Sulfate.lua?token=GHSAT0AAAAAABXMGZCWGQ4MUMC3WOQHY5VCYXSRJ5A",true))()
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
	name = "Click",
	callback = function()
		print("Clicked button")
	end,
})

--[[
name = <string> - The Name of the Button
callback = <function> - The Function of the Button
```
