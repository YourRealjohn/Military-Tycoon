# REDz Library V2
*RedzLibV2 English Version*

## ðŸ“¦ Load the Library
```lua
loadstring(game:HttpGet(("https://raw.githubusercontent.com/Seven7-lua/RedzLibs/refs/heads/main/src/RedzlibV2/source.lua")))()
```

## ðŸªŸ Create the Main Window
```lua
MakeWindow({
  Hub = {
    Title = "REDz HUB",
    Animation = "by : redz9999"
  },
  Key = {
    KeySystem = false, -- Put true if you want to activate the key system false if not
    Title = "Key System",
    Description = "",
    KeyLink = "",
    Keys = {"1234"},
    Notifi = {
      Notifications = true,
      CorrectKey = "Running the Script...",
      Incorrectkey = "The key is incorrect",
      CopyKeyLink = "Copied to Clipboard"
    }
  }
})
```

```lua
--[[
Hub: Window configuration
  Title: <string> HUB title
  Animation: <string> Animation text
Key: Key system configuration
  KeySystem: <boolean> Enable or disable key system
  Title: <string> Key system title
  Description: <string> Key system description
  KeyLink: <string> URL to get the key
  Keys: <table> List of valid keys
  Notifi: Key system notifications
    Notifications: <boolean> Enable notifications
    CorrectKey: <string> Message on correct key
    Incorrectkey: <string> Message on wrong key
    CopyKeyLink: <string> Message when link is copied
]]
```

## âž– Minimize Button
```lua
MinimizeButton({
  Image = "",
  Size = {40, 40},
  Color = Color3.fromRGB(10, 10, 10),
  Corner = true,
  Stroke = false,
  StrokeColor = Color3.fromRGB(255, 0, 0)
})
```

```lua
--[[
Image: <string> URL or asset ID for the image
Size: <table> Button size {width, height}
Color: <Color3> Background color
Corner: <boolean> Round corners
Stroke: <boolean> Add border
StrokeColor: <Color3> Border color
]]
```

## ðŸ—‚ï¸ Create a Tab
```lua
local Main = MakeTab({Name = "Main"})
```

## ðŸ”” Create a Notification
```lua
MakeNotifi({
  Title = "REDz HUB",
  Text = "Test Notification",
  Time = 5
})
```

## ðŸ“„ Create a Section
```lua
local section = AddSection(Main, {"Test"})
```

## ðŸ“ Update Section Text
```lua
SetSection(section, "Hello")
```

## ðŸ”˜ Create a Button
```lua
AddButton(Main, {
  Name = "Test Button",
  Callback = function()
    -- your function
  end
})
```

## âœ… Create a Toggle
```lua
local Toggle = AddToggle(Main, {
  Name = "Test Toggle",
  Default = false,
  Callback = function(Value)
    -- your function
  end
})
```

## ðŸ”„ Update Toggle
```lua
UpdateToggle(Toggle, true)
```

## ðŸŽšï¸ Create a Slider
```lua
local Slider = AddSlider(Main, {
  Name = "Test Slider",
  MinValue = 10,
  MaxValue = 100,
  Default = 25,
  Increase = 1,
  Callback = function(Value)
    -- your function
  end
})
```

## ðŸ”„ Update Slider
```lua
UpdateSlider(Slider, 50)
```

## âŒ¨ï¸ Create a Keybind
```lua
AddKeybind(Main, {
  Name = "Test Keybind",
  KeyCode = "E",
  Default = false,
  Callback = function(Value)
    -- your function
  end
})
```

## ðŸ“ Create a TextBox
```lua
AddTextBox(Main, {
  Name = "Test TextBox",
  Default = "Hello",
  PlaceholderText = "Type here...",
  ClearText = true,
  Callback = function(Value)
    -- your function
  end
})
```

## â¬‡ï¸ Create a Dropdown
```lua
local Dropdown = AddDropdown(Main, {
  Name = "Test Dropdown",
  Options = {"1", "2", "3"},
  Default = "2",
  Callback = function(Value)
    -- your function
  end
})
```

## ðŸ”„ Update Dropdown
```lua
UpdateDropdown(Dropdown, {"One", "Two", "Three"})
```

## ðŸŽ¨ Create a Color Picker
```lua
AddColorPicker(Main, {
  Name = "Test Color Picker",
  Default = Color3.fromRGB(255, 255, 0),
  Callback = function(Value)
    -- your function
  end
})
```

## ðŸ·ï¸ Create a Text Label
```lua
local Label = AddTextLabel(Main, "AutoFarm")
```

## ðŸ”„ Update Label Text
```lua
SetLabel(Label, "Running")
```

## ðŸ“œ Create a Paragraph
```lua
local Paragraph = AddParagraph(Main, {"Paragraph Title", "This is a paragraph description."})
```

## ðŸ”„ Update Paragraph
```lua
SetParagraph(Paragraph, {"New Title", "Updated description."})
```

## ðŸ–¼ï¸ Create an Image
```lua
local Image = AddImageLabel(Main, {
  Name = "Cool Image",
  Image = "rbxassetid://"
})
```

## ðŸ”„ Update Image
```lua
SetImage(Image, "rbxassetid://4155801252")
```

## ðŸ’£ Destroy the Script
```lua
DestroyScript()
```

## ðŸ“± Mobile Toggle (Floating)
```lua
local MobileToggle = AddMobileToggle({
  Name = "Mobile Toggle",
  Visible = true,
  Callback = function(Value)
    -- your function
  end
})

MobileToggle.Visible = true -- or false
```
