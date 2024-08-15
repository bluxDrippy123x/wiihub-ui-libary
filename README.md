# Create Window
```lua
local Fun = loadstring(game:HttpGet("https://raw.githubusercontent.com/insanedude59/CheetoHub/main/newlib"))() -- Cheeto hub's UI library
local a = Fun.Create('Title')
```

# Elements
```lua
local tab1 = name:Tab("Tab 1")

local section1 = tab1:Section('Section')

section1:Slider("Print",0,50,function(value)
	game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
end)

section1:Dropdown("Dropdown",{"Apple","Water","Grass"},function(val)
	print(val) -- Makes sure the script is working and it can past this line
end)

section1:Label('Label')

section1:Toggle("Toggle",function(value)
	game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
end)

section2:TextBox("Set your walkspeed", function(ammount)
	game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = ammount
end)
