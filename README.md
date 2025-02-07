local function MBUQEV_fake_script() -- Main.DraggableScript 
	local script = Instance.new('LocalScript', Main)
 
	local UIS = game:GetService('UserInputService')
	local frame = script.Parent
	local dragToggle = nil
	local dragSpeed = 0.25
	local dragStart = nil
	local startPos = nil
 
	local function updateInput(input)
		local delta = input.Position - dragStart
		local position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X,
			startPos.Y.Scale, startPos.Y.Offset + delta.Y)
		game:GetService('TweenService'):Create(frame, TweenInfo.new(dragSpeed), {Position = position}):Play()
	end
 
	frame.InputBegan:Connect(function(input)
		if (input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch) then 
			dragToggle = true
			dragStart = input.Position
			startPos = frame.Position
			input.Changed:Connect(function()
				if input.UserInputState == Enum.UserInputState.End then
					dragToggle = false
				end
			end)
		end
	end)
 
	UIS.InputChanged:Connect(function(input)
		if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
			if dragToggle then
				updateInput(input)
			end
		end
	end)
 
end
coroutine.wrap(MBUQEV_fake_script)()
local function NWAVVF_fake_script() -- Netless.NetlessScript 
	local script = Instance.new('LocalScript', Netless)
 
	script.Parent.MouseButton1Click:Connect(function()
		for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
			if v:IsA("BasePart") and v.Name ~="HumanoidRootPart" then 
				game:GetService("RunService").Heartbeat:connect(function()
					v.Velocity = Vector3.new(0,35,0)
					wait(0.5)
				end)
			end
		end
 
		game:GetService("StarterGui"):SetCore("SendNotification", { 
			Title = "Notification";
			Text = "Netless activated";
			Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
		Duration = 16;
	end)
end
coroutine.wrap(NWAVVF_fake_script)()
local function WSBO_fake_script() -- X.CloseUTGScript 
	local script = Instance.new('LocalScript', X)
 
	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.Parent.Main.Visible = false
		script.Parent.Parent.Parent.OpenUTG.Visible = true
	end)
end
coroutine.wrap(WSBO_fake_script)()
local function KZZCO_fake_script() -- OpenUTG.OpenUTGScript 
	local script = Instance.new('LocalScript', OpenUTG)
 
	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.Main.Visible = true
		script.Parent.Visible = false
	end)
end
coroutine.wrap(KZZCO_fake_script)()
 
AntiReport.MouseButton1Click:Connect(function()
setfflag("AbuseReportScreenshotPercentage", 0)
setfflag("DFFlagAbuseReportScreenshot", "False")
print("Anti-Report loaded")
end)
 
Among_Us.MouseButton1Click:Connect(function()
loadstring(game:HttpGet("https://pastebin.com/raw/JXUMavf3", true))()
end)
 
Ban.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/killermaster9999mega/thing/main/README.md"))()
end)
 
Chill.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/XmHFdTij"))()
end)
 
Chips.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/b289ts36"))()
end)
 
Cop.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/VAA5Mf60"))()
end)
 
Ender.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/bndCgupK"))()
end)
 
FlamingCube.MouseButton1Click:Connect(function()
loadstring(game:HttpGet("https://pastebin.com/raw/D7pigANg"))()
end)
 
Gale.MouseButton1Click:Connect(function()
loadstring(game:HttpGet(("https://pastebin.com/raw/PjJNLaFa"), true))()
end)
 
Grapple.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/AyASkDEG"))()
end)
 
Joy.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/LEAQuKj0"))()
end)
 
Killbot.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/G24tcRXA"))()
end)
 
NekoMaid.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://paste.ee/d/6bCwm/0"))()
end)
 
Neptunion.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/t0Mkc33N"))()
end)
 
RbNeptunion.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/gDi503fB"))()
end)
 
ServerAdmin.MouseButton1Click:Connect(function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/ONEReverseCard/My-Scripts/main/Netless%20Server%20Admin.md"))()
end)
 
ShadowBlade.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/kMYThpNG"))()
end)
 
Smug.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/ZuKy7HFF"))()
end)
 
Sonic.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/SyF5t70A"))()
end)
 
Spider.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/txsk1LJg"))()
end)
 
SwordStand.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://paste.ee/r/NwGVX/0"))()
end)
 
UMD.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/0QfjMKrF"))()
end)
 
Wall.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/AY6kA2AV"))()
end)
 
achroGlicher.MouseButton1Click:Connect(function()
loadstring(game:HttpGetAsync("https://pastebin.com/raw/T7cmny7C"))()
end)
