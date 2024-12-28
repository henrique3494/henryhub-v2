local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()

local Window = Library.CreateLib("henryhub v2", "DarkTheme")

--tabs
local Tab = Window:NewTab("bloxfruits")


--labs
Section:NewLabel("script")

--botōes
Section:NewButton("autofarm", "autofarmar levels", function()
    https://github.com/WarzMvp/blox-fruits-script.git
end)

--Toggles
Section:NewToggle("velocidade", "ToggleInfo", function(state)
    if state then
        print("rapido on")
    else
        print("rapido Off")
    end
end)

--sliders
Section:NewSlider("SliderText", "SliderInfo", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

