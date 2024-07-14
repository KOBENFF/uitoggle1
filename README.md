local UIKAITUN = Instance.new("ScreenGui")
local MainFrame = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local ToFrame = Instance.new("Frame")
local UICorner_2 = Instance.new("UICorner")
local SeaFrame = Instance.new("Frame")
local UICorner_3 = Instance.new("UICorner")
local NameHub = Instance.new("TextLabel")
local UICorner_4 = Instance.new("UICorner")
local MenuFrame = Instance.new("Frame")
local UICorner_5 = Instance.new("UICorner")
local Name = Instance.new("TextLabel")
local Lv = Instance.new("TextLabel")
local RACE = Instance.new("TextLabel")
local BELI = Instance.new("TextLabel")
local Health = Instance.new("TextLabel")
local ReFrame = Instance.new("Frame")
local UICorner_6 = Instance.new("UICorner")
local ImageLabel = Instance.new("ImageLabel")
local ProFile = Instance.new("ImageLabel")
local UICorner_7 = Instance.new("UICorner")
local FakeSetggie = Instance.new("ImageLabel")
local UICorner_8 = Instance.new("UICorner")
local UserInputService = game:GetService("UserInputService")
local TweenService = game:GetService("TweenService")
local RunService = game:GetService("RunService")
local LocalPlayer = game:GetService("Players").LocalPlayer
local Mouse = LocalPlayer:GetMouse()
function dragify(Frame, object)
	dragToggle = nil
	dragSpeed = .25
	dragInput = nil
	dragStart = nil
	dragPos = nil
	function updateInput(input)
		Delta = input.Position - dragStart
		Position =
			UDim2.new(startPos.X.Scale, startPos.X.Offset + Delta.X, startPos.Y.Scale, startPos.Y.Offset + Delta.Y)
		game:GetService("TweenService"):Create(object, TweenInfo.new(dragSpeed), {Position = Position}):Play()
	end
	Frame.InputBegan:Connect(
		function(input)
			if
				(input.UserInputType == Enum.UserInputType.MouseButton1 or
					input.UserInputType == Enum.UserInputType.Touch)
			then
				dragToggle = true
				dragStart = input.Position
				startPos = object.Position
				input.Changed:Connect(
					function()
						if (input.UserInputState == Enum.UserInputState.End) then
							dragToggle = false
						end
					end
				)
			end
		end
	)
	Frame.InputChanged:Connect(
		function(input)
			if
				(input.UserInputType == Enum.UserInputType.MouseMovement or
					input.UserInputType == Enum.UserInputType.Touch)
			then
				dragInput = input
			end
		end
	)
	game:GetService("UserInputService").InputChanged:Connect(
	function(input)
		if (input == dragInput and dragToggle) then
			updateInput(input)
		end
	end
	)
end
UIKAITUN.Name = "UIKAITUN"
UIKAITUN.Parent = game.CoreGui
UIKAITUN.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

MainFrame.Name = "MainFrame"
MainFrame.Parent = UIKAITUN
MainFrame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
MainFrame.BackgroundTransparency = 0.800
MainFrame.BorderColor3 = Color3.fromRGB(0, 0, 0)
MainFrame.BorderSizePixel = 0
MainFrame.Position = UDim2.new(0.214891151, 0, -0.0250696372, 0)
MainFrame.Size = UDim2.new(0.588776708, 0, 0.879460096, 0)

UICorner.CornerRadius = UDim.new(0, 11)
UICorner.Parent = MainFrame

ToFrame.Name = "ToFrame"
ToFrame.Parent = MainFrame
ToFrame.BackgroundColor3 = Color3.fromRGB(22, 22, 22)
ToFrame.BorderColor3 = Color3.fromRGB(0, 0, 0)
ToFrame.BorderSizePixel = 0
ToFrame.Position = UDim2.new(0.023108054, 0, 0.0221711118, 0)
ToFrame.Size = UDim2.new(0.619434893, 0, 0.934626102, 0)

UICorner_2.CornerRadius = UDim.new(0, 10)
UICorner_2.Parent = ToFrame

SeaFrame.Name = "SeaFrame"
SeaFrame.Parent = ToFrame
SeaFrame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
SeaFrame.BorderColor3 = Color3.fromRGB(0, 0, 0)
SeaFrame.BorderSizePixel = 0
SeaFrame.Position = UDim2.new(0.036066927, 0, 0.0372772813, 0)
SeaFrame.Size = UDim2.new(0.927149177, 0, 0.101665311, 0)

UICorner_3.CornerRadius = UDim.new(0, 50)
UICorner_3.Parent = SeaFrame

NameHub.Name = "NameHub"
NameHub.Parent = SeaFrame
NameHub.BackgroundColor3 = Color3.fromRGB(255, 85, 127)
NameHub.BorderColor3 = Color3.fromRGB(0, 0, 0)
NameHub.BorderSizePixel = 0
NameHub.Position = UDim2.new(0.321676373, 0, 0.100000001, 0)
NameHub.Size = UDim2.new(0.356336534, 0, 0.800000012, 0)
NameHub.Font = Enum.Font.SourceSans
NameHub.Text = "Attack Hub"
NameHub.TextColor3 = Color3.fromRGB(255, 255, 255)
NameHub.TextScaled = true
NameHub.TextSize = 14.000
NameHub.TextWrapped = true

UICorner_4.CornerRadius = UDim.new(0, 50)
UICorner_4.Parent = NameHub

MenuFrame.Name = "MenuFrame"
MenuFrame.Parent = ToFrame
MenuFrame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
MenuFrame.BorderColor3 = Color3.fromRGB(0, 0, 0)
MenuFrame.BorderSizePixel = 0
MenuFrame.Position = UDim2.new(0.0360668562, 0, 0.186386406, 0)
MenuFrame.Size = UDim2.new(0.927149296, 0, 0.781601489, 0)

UICorner_5.CornerRadius = UDim.new(0, 11)
UICorner_5.Parent = MenuFrame

Name.Name = "Name"
Name.Parent = MenuFrame
Name.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Name.BackgroundTransparency = 1.000
Name.BorderColor3 = Color3.fromRGB(0, 0, 0)
Name.BorderSizePixel = 0
Name.Position = UDim2.new(0.0482834093, 0, 0.0520292297, 0)
Name.Size = UDim2.new(0.482834101, 0, 0.130073071, 0)
Name.Font = Enum.Font.SourceSans
Name.Text = "Name : "..game.Players.LocalPlayer.Name
Name.TextColor3 = Color3.fromRGB(255, 255, 255)
Name.TextSize = 15.000
Name.TextXAlignment = Enum.TextXAlignment.Left

Lv.Name = "Lv"
Lv.Parent = MenuFrame
Lv.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Lv.BackgroundTransparency = 1.000
Lv.BorderColor3 = Color3.fromRGB(0, 0, 0)
Lv.BorderSizePixel = 0
Lv.Position = UDim2.new(0.0482834093, 0, 0.182102308, 0)
Lv.Size = UDim2.new(0.482834101, 0, 0.130073071, 0)
Lv.Font = Enum.Font.SourceSans
Lv.Text = "Level Wa : "..game:GetService("Players").LocalPlayer.Data.Level.Value
Lv.TextColor3 = Color3.fromRGB(255, 255, 255)
Lv.TextSize = 15.000
Lv.TextXAlignment = Enum.TextXAlignment.Left

RACE.Name = "RACE"
RACE.Parent = MenuFrame
RACE.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
RACE.BackgroundTransparency = 1.000
RACE.BorderColor3 = Color3.fromRGB(0, 0, 0)
RACE.BorderSizePixel = 0
RACE.Position = UDim2.new(0.0482834093, 0, 0.316511154, 0)
RACE.Size = UDim2.new(0.482834101, 0, 0.130073071, 0)
RACE.Font = Enum.Font.SourceSans
RACE.Text = "Race : "..game:GetService("Players").LocalPlayer.Data.Race.Value
RACE.TextColor3 = Color3.fromRGB(255, 255, 255)
RACE.TextSize = 15.000
RACE.TextXAlignment = Enum.TextXAlignment.Left

BELI.Name = "BELI"
BELI.Parent = MenuFrame
BELI.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
BELI.BackgroundTransparency = 1.000
BELI.BorderColor3 = Color3.fromRGB(0, 0, 0)
BELI.BorderSizePixel = 0
BELI.Position = UDim2.new(0.0482834093, 0, 0.459591538, 0)
BELI.Size = UDim2.new(0.482834101, 0, 0.130073071, 0)
BELI.Font = Enum.Font.SourceSans
BELI.Text = "Beli : "..game:GetService("Players").LocalPlayer.Data.Beli.Value
BELI.TextColor3 = Color3.fromRGB(255, 255, 255)
BELI.TextSize = 15.000
BELI.TextXAlignment = Enum.TextXAlignment.Left

Health.Name = "Health"
Health.Parent = MenuFrame
Health.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Health.BackgroundTransparency = 1.000
Health.BorderColor3 = Color3.fromRGB(0, 0, 0)
Health.BorderSizePixel = 0
Health.Position = UDim2.new(0.0482834093, 0, 0.576657295, 0)
Health.Size = UDim2.new(0.482834101, 0, 0.130073071, 0)
Health.Font = Enum.Font.SourceSans
Health.Text = "Health : "..game.Players.LocalPlayer.Character.Humanoid.Health
Health.TextColor3 = Color3.fromRGB(255, 255, 255)
Health.TextSize = 15.000
Health.TextXAlignment = Enum.TextXAlignment.Left

ReFrame.Name = "ReFrame"
ReFrame.Parent = MainFrame
ReFrame.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
ReFrame.BorderColor3 = Color3.fromRGB(0, 0, 0)
ReFrame.BorderSizePixel = 0
ReFrame.Position = UDim2.new(0.670446157, 0, 0.0221711118, 0)
ReFrame.Size = UDim2.new(0.307331592, 0, 0.465525299, 0)

UICorner_6.CornerRadius = UDim.new(0, 11)
UICorner_6.Parent = ReFrame

ImageLabel.Parent = ReFrame
ImageLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ImageLabel.BackgroundTransparency = 1.000
ImageLabel.BorderColor3 = Color3.fromRGB(0, 0, 0)
ImageLabel.BorderSizePixel = 0
ImageLabel.Position = UDim2.new(0, 0, 0.0748408213, 0)
ImageLabel.Size = UDim2.new(1.00000024, 0, 0.843030632, 0)
ImageLabel.Image = "rbxassetid://16663324629"

ProFile.Name = "ProFile"
ProFile.Parent = MainFrame
ProFile.BackgroundColor3 = Color3.fromRGB(173, 58, 87)
ProFile.BorderColor3 = Color3.fromRGB(0, 0, 0)
ProFile.BorderSizePixel = 0
ProFile.Position = UDim2.new(0.670131505, 0, 0.522604764, 0)
ProFile.Size = UDim2.new(0.307646304, 0, 0.434192419, 0)
ProFile.Image = "https://www.roblox.com/headshot-thumbnail/image?userId=" .. game.Players.LocalPlayer.UserId .. "&width=420&height=420&format=png"

UICorner_7.Parent = ProFile

FakeSetggie.Name = "FakeSetggie"
FakeSetggie.Parent = ProFile
FakeSetggie.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
FakeSetggie.BorderColor3 = Color3.fromRGB(0, 0, 0)
FakeSetggie.BorderSizePixel = 0
FakeSetggie.Position = UDim2.new(0.05257852, 0, 0.0510628708, 0)
FakeSetggie.Size = UDim2.new(0.199314073, 0, 0.16850251, 0)
FakeSetggie.Image = "rbxassetid://16162323955"

UICorner_8.CornerRadius = UDim.new(0, 50)
UICorner_8.Parent = FakeSetggie
