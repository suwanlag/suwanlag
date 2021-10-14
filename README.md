local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("ScriptHub", "LightTheme")

local Tab = Window:NewTab("Bloxfruit")
local Section = Tab:NewSection("SHELL X HUB Script")

Section:NewButton("Get", "ButtonInfo", function()
    loadstring(game:HttpGet("https://whitelistshellxhub.000webhostapp.com/script.lua"))()
end)

local Section = Tab:NewSection("XenonHub Script")

Section:NewButton("Get", "ButtonInfo", function()
    _G.Fast_Attack = true -- true / fasle [Full Screen Required]
    _G.Keys = "FE0N2-YKA3E-AG96M"
    _G.Color = Color3.fromRGB(235, 64, 52)
    loadstring(game:HttpGet("https://raw.githubusercontent.com/Xenon-Trash/Loader/main/Loader.lua"))();
end)

local Section = Tab:NewSection("Evillhub Script")

Section:NewButton("get", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/Natthawat69/EvilHub-FREE/main/Script.lua"))()
end)

local Section = Tab:NewSection("STRIKE HUB")

Section:NewButton("get", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/StormSKz12/StirkeHub1/main/Gameincluded"))()
end)

local Section = Tab:NewSection("CenterHub")

Section:NewButton("get", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/Achitsak/CENTER-HUB/main/Blox%20Fruits"))()
end)

local Tab = Window:NewTab("Kinlegacy")
local Section = Tab:NewSection("XenonHub")

Section:NewButton("get", "ButtonInfo", function()
    _G.Keys = "JUC4H-TVJZ5-ZIPXC"
_G.Color = Color3.fromRGB(235, 64, 52)
loadstring(game:HttpGet("https://raw.githubusercontent.com/Xenon-Trash/Loader/main/Loader.lua"))();
end)

local Section = Tab:NewSection("HyperXScript")

Section:NewButton("get", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/DookDekDEE/ALLFREE/main/hyperx.lua"))()
end)

local Tab = Window:NewTab("Arsenal")
local Section = Tab:NewSection("ArsenalScript")

Section:NewButton("get", "ButtonInfo", function()
    loadstring(game:HttpGet(('https://pastebin.com/raw/kvpwyQRT')))()
end)

local Section = Tab:NewSection("DarkHub")


Section:NewButton("get", "ButtonInfo", function()
    loadstring(game:HttpGet(('https://raw.githubusercontent.com/RandomAdamYT/DarkHub/master/Init'), true))()
end)
