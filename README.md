local AttackHubuiV1 = Instance.new("ScreenGui")
local Hee = Instance.new("TextButton")
local UICorner = Instance.new("UICorner")
local MainFrame = Instance.new("Frame")
local UICorner_2 = Instance.new("UICorner")
local MainNew = Instance.new("ImageLabel")
local Name = Instance.new("TextLabel")
local FRA = Instance.new("Frame")
local Tap1 = Instance.new("ImageButton")
local UICorner_3 = Instance.new("UICorner")
local Page1 = Instance.new("ScrollingFrame")
local Toggle1 = Instance.new("TextButton")
local Frame = Instance.new("Frame")
local Toggle1_2 = Instance.new("TextButton")
local Frame_2 = Instance.new("Frame")
local Hum = Instance.new("TextButton")
local UICorner_4 = Instance.new("UICorner")
AttackHubuiV1.Name = "Attack Hub ui V1"
AttackHubuiV1.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
AttackHubuiV1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Hee.Name = "Hee"
Hee.Parent = AttackHubuiV1
Hee.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Hee.BorderColor3 = Color3.fromRGB(0, 0, 0)
Hee.BorderSizePixel = 0
Hee.Position = UDim2.new(0, 0, 0.278551519, 0)
Hee.Size = UDim2.new(0.0833508298, 0, 0.137902439, 0)
Hee.Font = Enum.Font.SourceSans
Hee.Text = ""
Hee.TextColor3 = Color3.fromRGB(0, 0, 0)
Hee.TextSize = 14.000

UICorner.Parent = Hee

MainFrame.Name = "MainFrame"
MainFrame.Parent = Hee
MainFrame.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
MainFrame.BorderColor3 = Color3.fromRGB(0, 0, 0)
MainFrame.BorderSizePixel = 0
MainFrame.Position = UDim2.new(1.93613982, 0, -2.04011512, 0)
MainFrame.Size = UDim2.new(8.11159039, 0, 5.97306728, 0)

UICorner_2.Parent = MainFrame

MainNew.Name = "MainNew"
MainNew.Parent = MainFrame
MainNew.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
MainNew.BackgroundTransparency = 1.000
MainNew.BorderColor3 = Color3.fromRGB(0, 0, 0)
MainNew.BorderSizePixel = 0
MainNew.Position = UDim2.new(0.0120739266, 0, -1.29001947e-08, 0)
MainNew.Size = UDim2.new(0.10451857, 0, 0.151118219, 0)
MainNew.Image = "http://www.roblox.com/asset/?id=16663324629"

Name.Name = "Name"
Name.Parent = MainFrame
Name.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Name.BackgroundTransparency = 1.000
Name.BorderColor3 = Color3.fromRGB(0, 0, 0)
Name.BorderSizePixel = 0
Name.Position = UDim2.new(0.148911476, 0, 0.0236719605, 0)
Name.Size = UDim2.new(0.691174388, 0, 0.100000001, 0)
Name.Font = Enum.Font.FredokaOne
Name.Text = "Attack Hub"
Name.TextColor3 = Color3.fromRGB(0, 255, 0)
Name.TextSize = 50.000
Name.TextWrapped = true

FRA.Name = "FRA"
FRA.Parent = MainFrame
FRA.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
FRA.BorderColor3 = Color3.fromRGB(0, 0, 0)
FRA.BorderSizePixel = 0
FRA.Position = UDim2.new(0.129455656, 0, 0.170033261, 0)
FRA.Size = UDim2.new(0.870544255, 0, 0.826584995, 0)

Tap1.Name = "Tap1"
Tap1.Parent = MainFrame
Tap1.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Tap1.BackgroundTransparency = 1.000
Tap1.BorderColor3 = Color3.fromRGB(0, 0, 0)
Tap1.BorderSizePixel = 0
Tap1.Position = UDim2.new(0.0120738959, 0, 0.226574481, 0)
Tap1.Size = UDim2.new(0.100000001, 0, 0.154522374, 0)
Tap1.Image = "rbxassetid://7040391851"

UICorner_3.Parent = Tap1

Page1.Name = "Page1"
Page1.Parent = MainFrame
Page1.Active = true
Page1.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
Page1.BorderColor3 = Color3.fromRGB(0, 0, 0)
Page1.BorderSizePixel = 0
Page1.Position = UDim2.new(0.129455686, 0, 0.170033291, 0)
Page1.Size = UDim2.new(0.870544314, 0, 0.829966784, 0)

Toggle1.Name = "Toggle1"
Toggle1.Parent = Page1
Toggle1.BackgroundColor3 = Color3.fromRGB(102, 102, 102)
Toggle1.BorderColor3 = Color3.fromRGB(0, 0, 0)
Toggle1.BorderSizePixel = 0
Toggle1.Position = UDim2.new(0.0208040718, 0, 0.108464301, 0)
Toggle1.Size = UDim2.new(0.887488067, 0, -0.0688038841, 0)
Toggle1.Font = Enum.Font.SourceSansSemibold
Toggle1.LineHeight = 3.000
Toggle1.Text = "Auto Farm Lv"
Toggle1.TextColor3 = Color3.fromRGB(255, 255, 255)
Toggle1.TextSize = 30.000
Toggle1.TextWrapped = true
Toggle1.TextXAlignment = Enum.TextXAlignment.Left

Frame.Parent = Toggle1
Frame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame.BorderColor3 = Color3.fromRGB(0, 0, 0)
Frame.BorderSizePixel = 0
Frame.Position = UDim2.new(0.867336571, 0, 0.957378685, 0)
Frame.Size = UDim2.new(0.107416555, 0, -0.929860651, 0)

Toggle1_2.Name = "Toggle1"
Toggle1_2.Parent = Toggle1
Toggle1_2.BackgroundColor3 = Color3.fromRGB(102, 102, 102)
Toggle1_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
Toggle1_2.BorderSizePixel = 0
Toggle1_2.Position = UDim2.new(-1.58973009e-07, 0, 3.74984495e-07, 0)
Toggle1_2.Size = UDim2.new(1.00000036, 0, 0.972481012, 0)
Toggle1_2.Visible = false
Toggle1_2.Font = Enum.Font.SourceSans
Toggle1_2.Text = "Auto Farm Lv"
Toggle1_2.TextColor3 = Color3.fromRGB(255, 255, 255)
Toggle1_2.TextSize = 30.000
Toggle1_2.TextXAlignment = Enum.TextXAlignment.Left

Frame_2.Parent = Toggle1_2
Frame_2.BackgroundColor3 = Color3.fromRGB(0, 200, 255)
Frame_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
Frame_2.BorderSizePixel = 0
Frame_2.Position = UDim2.new(0.866999984, 0, 0.957000017, 0)
Frame_2.Size = UDim2.new(0.107000001, 0, -0.930000007, 0)

Hum.Name = "Hum"
Hum.Parent = MainFrame
Hum.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Hum.BorderColor3 = Color3.fromRGB(0, 0, 0)
Hum.BorderSizePixel = 0
Hum.Position = UDim2.new(-0.238688082, 0, 0.34663415, 0)
Hum.Size = UDim2.new(0.123280391, 0, 0.162336409, 0)
Hum.Font = Enum.Font.SourceSans
Hum.Text = ""
Hum.TextColor3 = Color3.fromRGB(0, 0, 0)
Hum.TextSize = 14.000

UICorner_4.Parent = Hum

-- Scripts:

local function JAHECFZ_fake_script() -- Toggle1_2.LocalScript 
	local script = Instance.new('LocalScript', Toggle1_2)

	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.Toggle1.Visible = false
	end)
end
coroutine.wrap(JAHECFZ_fake_script)()
local function PLMYIQZ_fake_script() -- Toggle1.LocalScript 
	local script = Instance.new('LocalScript', Toggle1)

	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Toggle1.Visible = true
	end)
end
coroutine.wrap(PLMYIQZ_fake_script)()
local function HYNOC_fake_script() -- Hum.LocalScript 
	local script = Instance.new('LocalScript', Hum)

	function Hum ()
		script.Parent.Parent.Parent.MainFrame.Visible = false
	end
	script.Parent.MouseButton1Click:Connect(Hum)
end
coroutine.wrap(HYNOC_fake_script)()
local function HZNLGGX_fake_script() -- Hee.LocalScript 
	local script = Instance.new('LocalScript', Hee)

	function Hee ()
		script.Parent.MainFrame.Visible = true
	end
	script.Parent.MouseButton1Click:Connect(Hee)
end
coroutine.wrap(HZNLGGX_fake_script)()

Toggle1.MouseButton1Down(function()
	
end)
