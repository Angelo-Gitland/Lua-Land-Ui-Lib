# 🏝️ Lua-Land-Ui-Library

🏝️ Lua Land Ui Library - A roblox ui library that help you to build an script immediately and easier. it was build since April 21, 2026 developed By LLH Lua Land.

# ❓ Why use Lua Land Ui Library

Using Lua Land Ui Library is better because it is the faster ui library that you can build your own scripts without building your custom gui. It also has an icon dictions and Themes dictions that you can use without rbxassetid only name of the icon.

<img width="1920" height="1280" alt="InShot_20260905_134022082" src="https://github.com/user-attachments/assets/ce1e6c54-0a17-4073-8a79-b456ee1089e6" />


# ✨ What are the ui elements

Lua Land Ui Library has a complete and good ui elements, the following are:

- TextButton
- Textbox
- TextLabel
- Slider
- Toogles
- Checkbox
- Dropdown
- Search Bar

Those are the list of ui elements in Lua Land Ui Library that you can create

# ⚡ Installation

**Booting Up The Library:**

```lua
local lib = loadstring(game:HttpGet("https://raw.githubusercontent.com/Angelo-Gitland/Lua-Land-Ui-Library/refs/heads/main/Lua%20Land%20Ui"))()
```

**Setting-Up the windows:**

```lua
local Window = Library:CreateWindow({
	Title = "Lua Land Ui Library",
	Subtitle = "Developed By LLH Lua Land",
	TitleIcon = "zap", -- -- Find available icons here: Dictions-Icons.md
	Theme = "Default", -- -- Find available themes here: Dictions-Themes.md
	Keybind = Enum.KeyCode.RightControl, -- Keybind for toggle
```

**Setting-Up Intro:**

```lua
Intro = {
		Title    = "Lua Land Ui Library",
		Subtitle = "Developed By LLH Lua Land",
		Icon     = "home",
	},
})
```

**Setting-Up Key system Window:**

```lua
	KeySystem = {
		Title = "Lua Land Key System",
		Subtitle = "Enter key to continue!",
		TitleIcon = "key-round", -- Find available icons here: Dictions-Icons.md
		Theme = "Fire", -- Find available themes here: Dictions-Themes.md
		Key = "LuaLandUiNew!",
		Placeholder = "Enter your key...",
		GetLink = "https://discord.gg/Zame2JAGDr",
		NotifTitle = "Lua Land Key System",
		NotifIcon = "clipboard-check",
		NotifDesc = "The key link was copied to your clipboard!",
		Script = function()
			loadstring(game:HttpGet("https://obfuscatorhub.vercel.app/api/JpDNqmfp"))() -- Script that will load if key is correct
		end,
	},
})
```

**Creating a Tab:**

```lua
local HomeTab = Window:CreateTab({
	Name      = "Home",
	Icon      = "house",
	SearchBar = false, -- Set to true if you want this tab with Search Bar
})
```

**Creating a Section:**

```lua
HomeTab:CreateSection("Welcome to Lua Land Ui Library!")
```

**Creating a TextLabel:**

```lua
HomeTab:CreateLabel("Developed By LLH Lua Land")
```

**Creating a Textbox:**

```lua
HomeTab:CreateTextbox({
	Title = "Textbox",
	Placeholder = "Type or input a text here!",
	Limit = 20, -- The limit of textbox text inputting.
	ClearOnFocus = false,
}, function(text, enterPressed)
	StatusLabel.Text = "Status: textbox = " .. tostring(text)
	print("[Lua Land] Textbox:", text, "Enter:", enterPressed)
end)
```

**Creating a TextButton:**

```lua
HomeTab:CreateButton("Join Discord", function()
   print("Link: https://discord.gg/EmxDAmasj6")
end)
```

**Creating a Slider:**

```lua
HomeTab:CreateSlider", 0, 500, function(Value)
     print("Slide it!")
end)
```

**Creating a Toogle:**

```lua
HomeTab:CreateToogle("Fly", function(Value)
    print("Logic Here!")
end)
```

**Creating a CheckBox:**

```lua
HomeTab:CreateCheckbox("Enable Floating", function(Value)
   print("Logic Here!")
end)
```

**Creating a Dropdown:**

```lua
HomeTab:CreateDropdown({
	Label   = "Choose type",
	Options = {"Team Color", "Health Color", "Static Color", "Rainbow"},
	Default = "Team Color",
}, function(Value)
	print("ESP Color Mode:", Value)
end)
```

📜 NOTE: This is just an example!

# 🎭 Icons Dictions List

**Open This File to see the full icons list [HERE](Dictions-Icons.md)**

In this file you can see the available icons in Lua Land Ui Library.

# 🤩 Themes Dictions List

**Open This File to see the full themes list [HERE](Dictions-Themes.md)**

In this file you can see the available themes that you can display and design for your script in Lua Land Ui Library.
