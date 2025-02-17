--1
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()

--windows
local Window = Library.CreateLib("2", "Ocean")

--tabs
local Tab = Window:NewTab("3")

Section:NewLabel("4")


--começo

Section:NewButton("5", "teste do script", function()
    print("IBlanksYT")
end)


--toggles usavel
Section:NewToggle("velocidade", "ToggleInfo", function(state)
    if state then
        print("rapido On")
    else
        print("rapido Off")
    end
end)

--sloders
Section:NewSlider("SliderText", "SliderInfo", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)
