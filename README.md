local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Tutorial", "BloodTheme")

---Tabs
local Tab = Window:NewTab("Buff")
local Section = Tab:NewSection("Buff")

----Buttons
Section:NewButton("Keyboard", "ButtonInfo", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/advxzivhsjjdhxhsidifvsh/mobkeyboard/main/main.txt", true))()
end)
Section:NewSlider("WalkSpeed", "MakeYouGoFaster", 200, 16, function(s) -- 200 (MaxValue) | 16 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)
