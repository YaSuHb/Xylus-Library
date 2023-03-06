# Xylus Library 
# The parent of the library
If you do not add this, Your GUI wont work.

```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/YaSuHb/Xylus-Library/main/XylusMain"))()
```

# Creating the window

```lua
Window = Library.Main("Text","LeftShift") -- change leftshift to the button that you want to use to hide the gui
```

# Creating tabs

```lua
local Tab = Window.NewTab("Text")
```

# Creating sections

```lua
local Section = Tab.NewSection("Text")
```

# Adding buttons

```lua
local Button = Section.NewButton("Text",function()
  --put your code here
end)
```

# Adding Toggles

```lua
local EnabledToggle = Section.NewToggle("Enabled Toggle",function(bool)
-- put your code here
end,true) -- true = enable

local DisabledToggle = Section.NewToggle("Disabled Toggle",function(bool)
-- put your code here
end,false) -- false = disabled
```

# Adding sliders

```lua
local SliderPrecise = section.NewSlider("Slider precise",0,100,true,function(value)

end,25)
local SliderNotPrecise = section.NewSlider("Slider not precise",0,100,false,function(value)

end,75)
```
