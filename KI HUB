local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("KI HUB", "Synapse")
--------------------------------------------------
local Tab = Window:NewTab("Main")
--------------------------------------------------
local Section = Tab:NewSection("infinite yield")
Section:NewButton("infinite yield", "infinite yield", function()
    loadstring(game:HttpGet(('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'),true))()
end)
--------------------------------------------------
local Section = Tab:NewSection("arsenal")
Section:NewButton("arsenal", "arsenal", function()
    loadstring(game:HttpGet(('https://pastebin.com/raw/kvpwyQRT')))()
end)
--------------------------------------------------
local Section = Tab:NewSection("speed")
Section:NewSlider("speed", "you speed", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)
--------------------------------------------------
local Tab = Window:NewTab("Player")
--------------------------------------------------
local Section = Tab:NewSection("player")
players = {}
 
for i,v in pairs(game:GetService("Players"):GetChildren()) do
   table.insert(players,v.Name)
end
 
Section:NewDropdown("Select Player", " ", players, function(abc)
    Select = abc
end)
 
 
Section:NewButton("Refresh", " ", function()
    table.clear(players)
for i,v in pairs(game:GetService("Players"):GetChildren()) do
   table.insert(players,v.Name)
end
end)
 
Section:NewButton("Teleport", " ", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[Select].Character.HumanoidRootPart.CFrame
end)
