--inpontates
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()

--Windows
local Window = Library.CreateLib("pikachu hub", "GrapeTheme")

--tabs 
local Tab = Window:NewTab("Início")

Section:NewButton("versão BETA", "BETA", function()
    print("Clicked")
end)

local Tab = Window:NewTab("TabName")

Section:NewButton("BETA", "BETA", function()
    print("Clicked")
end)

local Tab = Window:NewTab("TabName")

--setigs
local Section = Tab:NewSection("Início")

--tongless
Section:NewToggle("velocidade", "ToggleInfo", function(state)
    if state then
        print("Toggle On")
    else
        print("Toggle Off")
    end
end)

--slades
Section:NewSlider("PIkachu hub", "pika pika", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

--
