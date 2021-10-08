--Syntax V2
--credits Null, Vall, Lay

lplayer = game:GetService("Players").LocalPlayer

function GetPlayer(String)
	local Found = {}
	local strl = String:lower()
	if strl == "all" then
		for i,v in pairs(game:GetService("Players"):GetPlayers()) do
			table.insert(Found,v)
		end
	elseif strl == "others" then
		for i,v in pairs(game:GetService("Players"):GetPlayers()) do
			if v.Name ~= lplayer.Name then
				table.insert(Found,v)
			end
		end   
	elseif strl == "me" then
		for i,v in pairs(game:GetService("Players"):GetPlayers()) do
			if v.Name == lplayer.Name then
				table.insert(Found,v)
			end
		end  
	else
		for i,v in pairs(game:GetService("Players"):GetPlayers()) do
			if v.Name:lower():sub(1, #String) == String:lower() then
				table.insert(Found,v)
			end
		end    
	end
	return Found    
end
local Mouse = lplayer:GetMouse()

local SyntaxV2 = {
	SyntaxV2 = Instance.new("ScreenGui"),
	KeyFrame = Instance.new("Frame"),
	Title = Instance.new("TextLabel"),
	UIGradient = Instance.new("UIGradient"),
	UICorner = Instance.new("UICorner"),
	Login = Instance.new("TextButton"),
	UICorner_2 = Instance.new("UICorner"),
	UIGradient_2 = Instance.new("UIGradient"),
	Key = Instance.new("TextBox"),
	UICorner_3 = Instance.new("UICorner"),
	Discord = Instance.new("TextBox"),
	UICorner_4 = Instance.new("UICorner"),
	Title_2 = Instance.new("TextLabel"),
	UIGradient_3 = Instance.new("UIGradient"),
	UIGradient_4 = Instance.new("UIGradient"),
	Home = Instance.new("Frame"),
	xd4 = Instance.new("Frame"),
	Home_2 = Instance.new("Frame"),
	UICorner_5 = Instance.new("UICorner"),
	TextButton = Instance.new("TextButton"),
	UICorner_6 = Instance.new("UICorner"),
	HomeButton = Instance.new("ImageButton"),
	UIGradient_5 = Instance.new("UIGradient"),
	Commands = Instance.new("Frame"),
	UICorner_7 = Instance.new("UICorner"),
	TextButton_2 = Instance.new("TextButton"),
	UICorner_8 = Instance.new("UICorner"),
	ExecutorButton = Instance.new("ImageButton"),
	UIGradient_6 = Instance.new("UIGradient"),
	Commands_2 = Instance.new("Frame"),
	UICorner_9 = Instance.new("UICorner"),
	TextButton_3 = Instance.new("TextButton"),
	UICorner_10 = Instance.new("UICorner"),
	AnimationsButton = Instance.new("ImageButton"),
	UIGradient_7 = Instance.new("UIGradient"),
	Commands_3 = Instance.new("Frame"),
	UICorner_11 = Instance.new("UICorner"),
	TextButton_4 = Instance.new("TextButton"),
	UICorner_12 = Instance.new("UICorner"),
	HatButtons = Instance.new("ImageButton"),
	UIGradient_8 = Instance.new("UIGradient"),
	Title_3 = Instance.new("TextLabel"),
	UIGradient_9 = Instance.new("UIGradient"),
	Title_4 = Instance.new("TextLabel"),
	UIGradient_10 = Instance.new("UIGradient"),
	UIGradient_11 = Instance.new("UIGradient"),
	xd3 = Instance.new("Frame"),
	UICorner_13 = Instance.new("UICorner"),
	xd2 = Instance.new("Frame"),
	UICorner_14 = Instance.new("UICorner"),
	TextLabel = Instance.new("TextLabel"),
	UIGradient_12 = Instance.new("UIGradient"),
	TextInfo = Instance.new("TextLabel"),
	xd1 = Instance.new("Frame"),
	UICorner_15 = Instance.new("UICorner"),
	Main1 = Instance.new("Frame"),
	Main2 = Instance.new("Frame"),
	Executor = Instance.new("Frame"),
	Frame = Instance.new("Frame"),
	UICorner_16 = Instance.new("UICorner"),
	TextButton_5 = Instance.new("TextButton"),
	UICorner_17 = Instance.new("UICorner"),
	TextButton_6 = Instance.new("TextButton"),
	UICorner_18 = Instance.new("UICorner"),
	Executor_2 = Instance.new("TextBox"),
	UICorner_19 = Instance.new("UICorner"),
	UIGradient_13 = Instance.new("UIGradient"),
	Frame_2 = Instance.new("Frame"),
	TextLabel_2 = Instance.new("TextLabel"),
	UICorner_20 = Instance.new("UICorner"),
	ImageLabel = Instance.new("ImageLabel"),
	UICorner_21 = Instance.new("UICorner"),
	UIGradient_14 = Instance.new("UIGradient"),
	Frame_3 = Instance.new("Frame"),
	UICorner_22 = Instance.new("UICorner"),
	TextLabel_3 = Instance.new("TextLabel"),
	UIGradient_15 = Instance.new("UIGradient"),
	Commands_4 = Instance.new("Frame"),
	UIGradient_16 = Instance.new("UIGradient"),
	UICorner_23 = Instance.new("UICorner"),
	Frame_4 = Instance.new("Frame"),
	UICorner_24 = Instance.new("UICorner"),
	UIGradient_17 = Instance.new("UIGradient"),
	ScrollingFrame = Instance.new("ScrollingFrame"),
	Cmd1 = Instance.new("TextButton"),
	UIListLayout = Instance.new("UIListLayout"),
	Cmd2 = Instance.new("TextButton"),
	Cmd3 = Instance.new("TextButton"),
	Cmd4 = Instance.new("TextButton"),
	Cmd5 = Instance.new("TextButton"),
	Cmd6 = Instance.new("TextButton"),
	Cmd7 = Instance.new("TextButton"),
	Cmd8 = Instance.new("TextButton"),
	Cmd9 = Instance.new("TextButton"),
	Cmd10 = Instance.new("TextButton"),
	Cmd11 = Instance.new("TextButton"),
	Cmd12 = Instance.new("TextButton"),
	Cmd13 = Instance.new("TextButton"),
	Cmd14 = Instance.new("TextButton"),
	Cmd15 = Instance.new("TextButton"),
	Cmd16 = Instance.new("TextButton"),
	Cmd17 = Instance.new("TextButton"),
	Cmd18 = Instance.new("TextButton"),
	Cmd19 = Instance.new("TextButton"),
	Cmd20 = Instance.new("TextButton"),
	Cmd21 = Instance.new("TextButton"),
	Cmd22 = Instance.new("TextButton"),
	Cmd23 = Instance.new("TextButton"),
	Cmd24 = Instance.new("TextButton"),
	Cmd25 = Instance.new("TextButton"),
	Cmd26 = Instance.new("TextButton"),
	UICorner_25 = Instance.new("UICorner"),
	HatScripts = Instance.new("Frame"),
	Frame_5 = Instance.new("Frame"),
	UICorner_26 = Instance.new("UICorner"),
	ScrollingFrame_2 = Instance.new("ScrollingFrame"),
	Hat1 = Instance.new("TextButton"),
	UICorner_27 = Instance.new("UICorner"),
	UIListLayout_2 = Instance.new("UIListLayout"),
	Hat2 = Instance.new("TextButton"),
	UICorner_28 = Instance.new("UICorner"),
	Hat3 = Instance.new("TextButton"),
	UICorner_29 = Instance.new("UICorner"),
	Hat4 = Instance.new("TextButton"),
	UICorner_30 = Instance.new("UICorner"),
	Hat5 = Instance.new("TextButton"),
	UICorner_31 = Instance.new("UICorner"),
	Hat6 = Instance.new("TextButton"),
	UICorner_32 = Instance.new("UICorner"),
	Hat7 = Instance.new("TextButton"),
	UICorner_33 = Instance.new("UICorner"),
	Hat8 = Instance.new("TextButton"),
	UICorner_34 = Instance.new("UICorner"),
	Hat9 = Instance.new("TextButton"),
	UICorner_35 = Instance.new("UICorner"),
	Hat10 = Instance.new("TextButton"),
	UICorner_36 = Instance.new("UICorner"),
	Hat11 = Instance.new("TextButton"),
	UICorner_37 = Instance.new("UICorner"),
	Hat12 = Instance.new("TextButton"),
	UICorner_38 = Instance.new("UICorner"),
	Hat13 = Instance.new("TextButton"),
	UICorner_39 = Instance.new("UICorner"),
	Hat14 = Instance.new("TextButton"),
	UICorner_40 = Instance.new("UICorner"),
	Hat15 = Instance.new("TextButton"),
	UICorner_41 = Instance.new("UICorner"),
	Hat16 = Instance.new("TextButton"),
	UICorner_42 = Instance.new("UICorner"),
	Hat17 = Instance.new("TextButton"),
	UICorner_43 = Instance.new("UICorner"),
	Hat18 = Instance.new("TextButton"),
	UICorner_44 = Instance.new("UICorner"),
	Hat19 = Instance.new("TextButton"),
	UICorner_45 = Instance.new("UICorner"),
	Hat20 = Instance.new("TextButton"),
	UICorner_46 = Instance.new("UICorner"),
	Hat21 = Instance.new("TextButton"),
	UICorner_47 = Instance.new("UICorner"),
	Hat22 = Instance.new("TextButton"),
	UICorner_48 = Instance.new("UICorner"),
	Hat23 = Instance.new("TextButton"),
	UICorner_49 = Instance.new("UICorner"),
	Hat24 = Instance.new("TextButton"),
	UICorner_50 = Instance.new("UICorner"),
	Hat25 = Instance.new("TextButton"),
	UICorner_51 = Instance.new("UICorner"),
	Hat26 = Instance.new("TextButton"),
	UICorner_52 = Instance.new("UICorner"),
	Hat27 = Instance.new("TextButton"),
	UICorner_53 = Instance.new("UICorner"),
	Hat28 = Instance.new("TextButton"),
	UICorner_54 = Instance.new("UICorner"),
	UIGradient_18 = Instance.new("UIGradient"),
	ColorMenu1 = Instance.new("Frame"),
	UICorner_55 = Instance.new("UICorner"),
	ColorMenu1_2 = Instance.new("Frame"),
	UICorner_56 = Instance.new("UICorner"),
	UIGradient_19 = Instance.new("UIGradient"),
	TextLabel_4 = Instance.new("TextLabel"),
	xd4_2 = Instance.new("Frame"),
	UICorner_57 = Instance.new("UICorner"),
	AnimationsScripts = Instance.new("Frame"),
	Frame_6 = Instance.new("Frame"),
	UICorner_58 = Instance.new("UICorner"),
	ScrollingFrame_3 = Instance.new("ScrollingFrame"),
	UIListLayout_3 = Instance.new("UIListLayout"),
	Anim1 = Instance.new("TextButton"),
	UICorner_59 = Instance.new("UICorner"),
	Anim10 = Instance.new("TextButton"),
	UICorner_60 = Instance.new("UICorner"),
	Anim11 = Instance.new("TextButton"),
	UICorner_61 = Instance.new("UICorner"),
	Anim12 = Instance.new("TextButton"),
	UICorner_62 = Instance.new("UICorner"),
	Anim13 = Instance.new("TextButton"),
	UICorner_63 = Instance.new("UICorner"),
	Anim14 = Instance.new("TextButton"),
	UICorner_64 = Instance.new("UICorner"),
	Anim15 = Instance.new("TextButton"),
	UICorner_65 = Instance.new("UICorner"),
	Anim16 = Instance.new("TextButton"),
	UICorner_66 = Instance.new("UICorner"),
	Anim17 = Instance.new("TextButton"),
	UICorner_67 = Instance.new("UICorner"),
	Anim18 = Instance.new("TextButton"),
	UICorner_68 = Instance.new("UICorner"),
	Anim19 = Instance.new("TextButton"),
	UICorner_69 = Instance.new("UICorner"),
	Anim2 = Instance.new("TextButton"),
	UICorner_70 = Instance.new("UICorner"),
	Anim20 = Instance.new("TextButton"),
	UICorner_71 = Instance.new("UICorner"),
	Anim21 = Instance.new("TextButton"),
	UICorner_72 = Instance.new("UICorner"),
	Anim22 = Instance.new("TextButton"),
	UICorner_73 = Instance.new("UICorner"),
	Anim23 = Instance.new("TextButton"),
	UICorner_74 = Instance.new("UICorner"),
	Anim24 = Instance.new("TextButton"),
	UICorner_75 = Instance.new("UICorner"),
	Anim25 = Instance.new("TextButton"),
	UICorner_76 = Instance.new("UICorner"),
	Anim26 = Instance.new("TextButton"),
	UICorner_77 = Instance.new("UICorner"),
	Anim27 = Instance.new("TextButton"),
	UICorner_78 = Instance.new("UICorner"),
	Anim28 = Instance.new("TextButton"),
	UICorner_79 = Instance.new("UICorner"),
	Anim3 = Instance.new("TextButton"),
	UICorner_80 = Instance.new("UICorner"),
	Anim4 = Instance.new("TextButton"),
	UICorner_81 = Instance.new("UICorner"),
	Anim5 = Instance.new("TextButton"),
	UICorner_82 = Instance.new("UICorner"),
	Anim6 = Instance.new("TextButton"),
	UICorner_83 = Instance.new("UICorner"),
	Anim7 = Instance.new("TextButton"),
	UICorner_84 = Instance.new("UICorner"),
	Anim8 = Instance.new("TextButton"),
	UICorner_85 = Instance.new("UICorner"),
	Anim9 = Instance.new("TextButton"),
	UICorner_86 = Instance.new("UICorner"),
	UIGradient_20 = Instance.new("UIGradient"),
	ColorMenu1_3 = Instance.new("Frame"),
	UICorner_87 = Instance.new("UICorner"),
	ColorMenu1_4 = Instance.new("Frame"),
	UICorner_88 = Instance.new("UICorner"),
	UIGradient_21 = Instance.new("UIGradient"),
	TextLabel_5 = Instance.new("TextLabel"),
	xd4_3 = Instance.new("Frame"),
	UICorner_89 = Instance.new("UICorner"),
	Home_3 = Instance.new("Frame"),
	Frame_7 = Instance.new("Frame"),
	TextLabel_6 = Instance.new("TextLabel"),
	UICorner_90 = Instance.new("UICorner"),
	ImageLabel_2 = Instance.new("ImageLabel"),
	xd4_4 = Instance.new("Frame"),
	UICorner_91 = Instance.new("UICorner"),
	xd4_5 = Instance.new("Frame"),
	UICorner_92 = Instance.new("UICorner"),
	xd4_6 = Instance.new("Frame"),
	UICorner_93 = Instance.new("UICorner"),
	close = Instance.new("TextButton"),
	UICorner_94 = Instance.new("UICorner"),
}

--Properties:

SyntaxV2.SyntaxV2.Name = "SyntaxV2"
SyntaxV2.SyntaxV2.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
SyntaxV2.SyntaxV2.ResetOnSpawn = false

SyntaxV2.KeyFrame.Name = "KeyFrame"
SyntaxV2.KeyFrame.Parent = SyntaxV2.SyntaxV2
SyntaxV2.KeyFrame.BackgroundColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.KeyFrame.Position = UDim2.new(0.5, -250, 0.523312867, -150)
SyntaxV2.KeyFrame.Size = UDim2.new(0, 500, 0, 262)

SyntaxV2.Title.Name = "Title"
SyntaxV2.Title.Parent = SyntaxV2.KeyFrame
SyntaxV2.Title.BackgroundColor3 = Color3.fromRGB(170, 0, 0)
SyntaxV2.Title.BackgroundTransparency = 1.000
SyntaxV2.Title.Position = UDim2.new(0.296000004, 0, 0.113969408, 0)
SyntaxV2.Title.Size = UDim2.new(0, 149, 0, 48)
SyntaxV2.Title.Font = Enum.Font.SourceSans
SyntaxV2.Title.Text = "Syntax"
SyntaxV2.Title.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Title.TextScaled = true
SyntaxV2.Title.TextSize = 14.000
SyntaxV2.Title.TextStrokeTransparency = 0.690
SyntaxV2.Title.TextWrapped = true

SyntaxV2.UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(0.99, Color3.fromRGB(83, 0, 125)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(0, 0, 0))}
SyntaxV2.UIGradient.Rotation = 45
SyntaxV2.UIGradient.Parent = SyntaxV2.Title

SyntaxV2.UICorner.Parent = SyntaxV2.KeyFrame

SyntaxV2.Login.Name = "Login"
SyntaxV2.Login.Parent = SyntaxV2.KeyFrame
SyntaxV2.Login.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Login.BackgroundTransparency = 0.200
SyntaxV2.Login.Position = UDim2.new(0.340000004, 0, 0.729516387, 0)
SyntaxV2.Login.Size = UDim2.new(0, 159, 0, 30)
SyntaxV2.Login.Font = Enum.Font.SourceSansLight
SyntaxV2.Login.Text = "Enter"
SyntaxV2.Login.TextColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Login.TextScaled = true
SyntaxV2.Login.TextSize = 14.000
SyntaxV2.Login.TextWrapped = true
SyntaxV2.Login.MouseButton1Down:connect(function()
	--sounds and shits
	SyntaxV2.Login.Size = UDim2.new(0, 149, 0, 20)
	wait(0.1)
	SyntaxV2.Login.Size = UDim2.new(0, 159, 0, 30)
end)

SyntaxV2.UICorner_2.Parent = SyntaxV2.Login

SyntaxV2.UIGradient_2.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(42, 42, 42)), ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(255, 255, 255))}
SyntaxV2.UIGradient_2.Rotation = 45
SyntaxV2.UIGradient_2.Parent = SyntaxV2.Login

SyntaxV2.Key.Name = "Key"
SyntaxV2.Key.Parent = SyntaxV2.KeyFrame
SyntaxV2.Key.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Key.BackgroundTransparency = 0.700
SyntaxV2.Key.Position = UDim2.new(0, 0, 0.393333346, 0)
SyntaxV2.Key.Size = UDim2.new(0, 500, 0, 59)
SyntaxV2.Key.Font = Enum.Font.Code
SyntaxV2.Key.PlaceholderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Key.PlaceholderText = "Insert Key"
SyntaxV2.Key.Text = ""
SyntaxV2.Key.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Key.TextSize = 14.000

SyntaxV2.UICorner_3.Parent = SyntaxV2.Key

SyntaxV2.Discord.Name = "Discord"
SyntaxV2.Discord.Parent = SyntaxV2.KeyFrame
SyntaxV2.Discord.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Discord.BackgroundTransparency = 1.000
SyntaxV2.Discord.Position = UDim2.new(0, 0, 0.901272118, 0)
SyntaxV2.Discord.Size = UDim2.new(0, 500, 0, 25)
SyntaxV2.Discord.ClearTextOnFocus = false
SyntaxV2.Discord.Font = Enum.Font.SciFi
SyntaxV2.Discord.PlaceholderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Discord.Text = "https://discord.gg/tCjb5sr9Qu"
SyntaxV2.Discord.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Discord.TextSize = 14.000
SyntaxV2.Discord.TextWrapped = true

SyntaxV2.UICorner_4.Parent = SyntaxV2.Discord

SyntaxV2.Title_2.Name = "Title"
SyntaxV2.Title_2.Parent = SyntaxV2.KeyFrame
SyntaxV2.Title_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Title_2.BackgroundTransparency = 1.000
SyntaxV2.Title_2.Position = UDim2.new(0.569999993, 0, 0.113969408, 0)
SyntaxV2.Title_2.Size = UDim2.new(0, 51, 0, 48)
SyntaxV2.Title_2.Font = Enum.Font.SourceSans
SyntaxV2.Title_2.Text = "FE"
SyntaxV2.Title_2.TextColor3 = Color3.fromRGB(255, 128, 0)
SyntaxV2.Title_2.TextScaled = true
SyntaxV2.Title_2.TextSize = 14.000
SyntaxV2.Title_2.TextWrapped = true

SyntaxV2.UIGradient_3.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(0.96, Color3.fromRGB(170, 0, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(0, 0, 0))}
SyntaxV2.UIGradient_3.Rotation = 45
SyntaxV2.UIGradient_3.Parent = SyntaxV2.Title_2

SyntaxV2.UIGradient_4.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(43, 0, 65)), ColorSequenceKeypoint.new(0.34, Color3.fromRGB(85, 0, 127)), ColorSequenceKeypoint.new(0.45, Color3.fromRGB(170, 0, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(21, 21, 21))}
SyntaxV2.UIGradient_4.Rotation = 45
SyntaxV2.UIGradient_4.Parent = SyntaxV2.KeyFrame

SyntaxV2.Home.Name = "Home"
SyntaxV2.Home.Parent = SyntaxV2.SyntaxV2
SyntaxV2.Home.BackgroundColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.Home.BorderColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.Home.BorderSizePixel = 2
SyntaxV2.Home.Position = UDim2.new(-10, -250, 0.5, -150)
SyntaxV2.Home.Size = UDim2.new(0, 683, 0, 309)

SyntaxV2.xd4.Name = "xd4"
SyntaxV2.xd4.Parent = SyntaxV2.Home
SyntaxV2.xd4.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.xd4.BackgroundTransparency = 0.250
SyntaxV2.xd4.BorderColor3 = Color3.fromRGB(27, 42, 53)
SyntaxV2.xd4.BorderSizePixel = 0
SyntaxV2.xd4.Position = UDim2.new(0, 0, 0.134609684, 0)
SyntaxV2.xd4.Size = UDim2.new(0, 151, 0, 267)

SyntaxV2.Home_2.Name = "Home"
SyntaxV2.Home_2.Parent = SyntaxV2.xd4
SyntaxV2.Home_2.BackgroundColor3 = Color3.fromRGB(132, 0, 198)
SyntaxV2.Home_2.BorderSizePixel = 0
SyntaxV2.Home_2.Position = UDim2.new(0, 0, 0.0553505421, 0)
SyntaxV2.Home_2.Size = UDim2.new(0, 136, 0, 30)

SyntaxV2.UICorner_5.Parent = SyntaxV2.Home_2

SyntaxV2.TextButton.Parent = SyntaxV2.Home_2
SyntaxV2.TextButton.BackgroundColor3 = Color3.fromRGB(17, 17, 17)
SyntaxV2.TextButton.BackgroundTransparency = 0.250
SyntaxV2.TextButton.Position = UDim2.new(0.226904929, 0, 0.120172121, 0)
SyntaxV2.TextButton.Size = UDim2.new(0, 98, 0, 22)
SyntaxV2.TextButton.Font = Enum.Font.TitilliumWeb
SyntaxV2.TextButton.Text = "Home"
SyntaxV2.TextButton.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextButton.TextScaled = true
SyntaxV2.TextButton.TextSize = 1.000
SyntaxV2.TextButton.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextButton.TextWrapped = true
SyntaxV2.TextButton.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=4499400560"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()
	SyntaxV2.TextButton.Size = UDim2.new(0, 88, 0, 20)
	wait(0.1)
	SyntaxV2.TextButton.Size = UDim2.new(0, 98, 0, 22)
SyntaxV2.HomeButton.ImageColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.ExecutorButton.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.AnimationsButton.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.HatButtons.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Home_3.Visible = true
SyntaxV2.Executor.Visible = false
SyntaxV2.AnimationsScripts.Visible = false
SyntaxV2.HatScripts.Visible = false
end)

SyntaxV2.UICorner_6.Parent = SyntaxV2.TextButton

SyntaxV2.HomeButton.Name = "HomeButton"
SyntaxV2.HomeButton.Parent = SyntaxV2.TextButton
SyntaxV2.HomeButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.HomeButton.BackgroundTransparency = 1.000
SyntaxV2.HomeButton.Position = UDim2.new(-0.290088654, 0, -0.163871065, 0)
SyntaxV2.HomeButton.Size = UDim2.new(0, 27, 0, 30)
SyntaxV2.HomeButton.Image = "http://www.roblox.com/asset/?id=4034483344"
SyntaxV2.HomeButton.ImageColor3 = Color3.fromRGB(170, 0, 255)

SyntaxV2.UIGradient_5.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(43, 0, 65)), ColorSequenceKeypoint.new(0.72, Color3.fromRGB(169, 0, 254)), ColorSequenceKeypoint.new(0.73, Color3.fromRGB(170, 0, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(170, 0, 255))}
SyntaxV2.UIGradient_5.Rotation = 45
SyntaxV2.UIGradient_5.Parent = SyntaxV2.Home_2

SyntaxV2.Commands.Name = "Commands"
SyntaxV2.Commands.Parent = SyntaxV2.xd4
SyntaxV2.Commands.BackgroundColor3 = Color3.fromRGB(132, 0, 198)
SyntaxV2.Commands.BorderSizePixel = 0
SyntaxV2.Commands.Position = UDim2.new(0, 0, 0.221402198, 0)
SyntaxV2.Commands.Size = UDim2.new(0, 136, 0, 30)

SyntaxV2.UICorner_7.Parent = SyntaxV2.Commands

SyntaxV2.TextButton_2.Parent = SyntaxV2.Commands
SyntaxV2.TextButton_2.BackgroundColor3 = Color3.fromRGB(17, 17, 17)
SyntaxV2.TextButton_2.BackgroundTransparency = 0.250
SyntaxV2.TextButton_2.Position = UDim2.new(0.226904929, 0, 0.120172121, 0)
SyntaxV2.TextButton_2.Size = UDim2.new(0, 99, 0, 22)
SyntaxV2.TextButton_2.Font = Enum.Font.TitilliumWeb
SyntaxV2.TextButton_2.Text = "Executor"
SyntaxV2.TextButton_2.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextButton_2.TextScaled = true
SyntaxV2.TextButton_2.TextSize = 1.000
SyntaxV2.TextButton_2.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextButton_2.TextWrapped = true
SyntaxV2.TextButton_2.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=4499400560"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()
	SyntaxV2.TextButton_2.Size = UDim2.new(0, 88, 0, 20)
	wait(0.1)
	SyntaxV2.TextButton_2.Size = UDim2.new(0, 98, 0, 22)
SyntaxV2.ExecutorButton.ImageColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.HomeButton.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.AnimationsButton.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.HatButtons.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Executor.Visible = true
SyntaxV2.Home_3.Visible = false
SyntaxV2.AnimationsScripts.Visible = false
SyntaxV2.HatScripts.Visible = false
end)


SyntaxV2.UICorner_8.Parent = SyntaxV2.TextButton_2

SyntaxV2.ExecutorButton.Name = "ExecutorButton"
SyntaxV2.ExecutorButton.Parent = SyntaxV2.TextButton_2
SyntaxV2.ExecutorButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.ExecutorButton.BackgroundTransparency = 1.000
SyntaxV2.ExecutorButton.Position = UDim2.new(-0.253973156, 0, 0.0909090936, 0)
SyntaxV2.ExecutorButton.Size = UDim2.new(0, 21, 0, 24)
SyntaxV2.ExecutorButton.Image = "http://www.roblox.com/asset/?id=743952980"

SyntaxV2.UIGradient_6.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(43, 0, 65)), ColorSequenceKeypoint.new(0.72, Color3.fromRGB(169, 0, 254)), ColorSequenceKeypoint.new(0.73, Color3.fromRGB(170, 0, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(170, 0, 255))}
SyntaxV2.UIGradient_6.Rotation = 45
SyntaxV2.UIGradient_6.Parent = SyntaxV2.Commands

SyntaxV2.Commands_2.Name = "Commands"
SyntaxV2.Commands_2.Parent = SyntaxV2.xd4
SyntaxV2.Commands_2.BackgroundColor3 = Color3.fromRGB(132, 0, 198)
SyntaxV2.Commands_2.BorderSizePixel = 0
SyntaxV2.Commands_2.Position = UDim2.new(0, 0, 0.389941514, 0)
SyntaxV2.Commands_2.Size = UDim2.new(0, 136, 0, 30)

SyntaxV2.UICorner_9.Parent = SyntaxV2.Commands_2

SyntaxV2.TextButton_3.Parent = SyntaxV2.Commands_2
SyntaxV2.TextButton_3.BackgroundColor3 = Color3.fromRGB(17, 17, 17)
SyntaxV2.TextButton_3.BackgroundTransparency = 0.250
SyntaxV2.TextButton_3.Position = UDim2.new(0.226904929, 0, 0.120172121, 0)
SyntaxV2.TextButton_3.Size = UDim2.new(0, 99, 0, 22)
SyntaxV2.TextButton_3.Font = Enum.Font.TitilliumWeb
SyntaxV2.TextButton_3.Text = "Animations"
SyntaxV2.TextButton_3.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextButton_3.TextScaled = true
SyntaxV2.TextButton_3.TextSize = 1.000
SyntaxV2.TextButton_3.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextButton_3.TextWrapped = true
SyntaxV2.TextButton_3.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=4499400560"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()
	SyntaxV2.TextButton_3.Size = UDim2.new(0, 88, 0, 20)
	wait(0.1)
	SyntaxV2.TextButton_3.Size = UDim2.new(0, 98, 0, 22)
SyntaxV2.AnimationsButton.ImageColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.ExecutorButton.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.HomeButton.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.HatButtons.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.AnimationsScripts.Visible = true
SyntaxV2.Executor.Visible = false
SyntaxV2.Home_3.Visible = false
SyntaxV2.HatScripts.Visible = false
end)

SyntaxV2.UICorner_10.Parent = SyntaxV2.TextButton_3

SyntaxV2.AnimationsButton.Name = "AnimationsButton"
SyntaxV2.AnimationsButton.Parent = SyntaxV2.TextButton_3
SyntaxV2.AnimationsButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.AnimationsButton.BackgroundTransparency = 1.000
SyntaxV2.AnimationsButton.Position = UDim2.new(-0.253973156, 0, 0.0909090936, 0)
SyntaxV2.AnimationsButton.Size = UDim2.new(0, 21, 0, 24)
SyntaxV2.AnimationsButton.Image = "http://www.roblox.com/asset/?id=7059328055"

SyntaxV2.UIGradient_7.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(43, 0, 65)), ColorSequenceKeypoint.new(0.72, Color3.fromRGB(169, 0, 254)), ColorSequenceKeypoint.new(0.73, Color3.fromRGB(170, 0, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(170, 0, 255))}
SyntaxV2.UIGradient_7.Rotation = 45
SyntaxV2.UIGradient_7.Parent = SyntaxV2.Commands_2

SyntaxV2.Commands_3.Name = "Commands"
SyntaxV2.Commands_3.Parent = SyntaxV2.xd4
SyntaxV2.Commands_3.BackgroundColor3 = Color3.fromRGB(132, 0, 198)
SyntaxV2.Commands_3.BorderSizePixel = 0
SyntaxV2.Commands_3.Position = UDim2.new(0, 0, 0.569716811, 0)
SyntaxV2.Commands_3.Size = UDim2.new(0, 136, 0, 30)

SyntaxV2.UICorner_11.Parent = SyntaxV2.Commands_3

SyntaxV2.TextButton_4.Parent = SyntaxV2.Commands_3
SyntaxV2.TextButton_4.BackgroundColor3 = Color3.fromRGB(17, 17, 17)
SyntaxV2.TextButton_4.BackgroundTransparency = 0.250
SyntaxV2.TextButton_4.Position = UDim2.new(0.226904929, 0, 0.120172121, 0)
SyntaxV2.TextButton_4.Size = UDim2.new(0, 99, 0, 22)
SyntaxV2.TextButton_4.Font = Enum.Font.TitilliumWeb
SyntaxV2.TextButton_4.Text = "Hats, Fling"
SyntaxV2.TextButton_4.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextButton_4.TextScaled = true
SyntaxV2.TextButton_4.TextSize = 1.000
SyntaxV2.TextButton_4.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextButton_4.TextWrapped = true
SyntaxV2.TextButton_4.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=4499400560"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()
	SyntaxV2.TextButton_4.Size = UDim2.new(0, 88, 0, 20)
	wait(0.1)
	SyntaxV2.TextButton_4.Size = UDim2.new(0, 98, 0, 22)
SyntaxV2.HatButtons.ImageColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.HomeButton.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.ExecutorButton.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.AnimationsButton.ImageColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.HatScripts.Visible = true
SyntaxV2.AnimationsScripts.Visible = false
SyntaxV2.Executor.Visible = false
SyntaxV2.Home_3.Visible = false
end)


SyntaxV2.UICorner_12.Parent = SyntaxV2.TextButton_4

SyntaxV2.HatButtons.Name = "HatButtons"
SyntaxV2.HatButtons.Parent = SyntaxV2.TextButton_4
SyntaxV2.HatButtons.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.HatButtons.BackgroundTransparency = 1.000
SyntaxV2.HatButtons.Position = UDim2.new(-0.264074177, 0, 0, 0)
SyntaxV2.HatButtons.Size = UDim2.new(0, 21, 0, 24)
SyntaxV2.HatButtons.Image = "http://www.roblox.com/asset/?id=7407483146"

SyntaxV2.UIGradient_8.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(43, 0, 65)), ColorSequenceKeypoint.new(0.72, Color3.fromRGB(169, 0, 254)), ColorSequenceKeypoint.new(0.73, Color3.fromRGB(170, 0, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(170, 0, 255))}
SyntaxV2.UIGradient_8.Rotation = 45
SyntaxV2.UIGradient_8.Parent = SyntaxV2.Commands_3

SyntaxV2.Title_3.Name = "Title"
SyntaxV2.Title_3.Parent = SyntaxV2.Home
SyntaxV2.Title_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Title_3.BackgroundTransparency = 1.000
SyntaxV2.Title_3.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Title_3.Size = UDim2.new(0, 83, 0, 30)
SyntaxV2.Title_3.Font = Enum.Font.SourceSansBold
SyntaxV2.Title_3.Text = "Syntax"
SyntaxV2.Title_3.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Title_3.TextSize = 28.000
SyntaxV2.Title_3.TextStrokeTransparency = 0.000
SyntaxV2.Title_3.TextWrapped = true

SyntaxV2.UIGradient_9.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(0.98, Color3.fromRGB(133, 0, 200)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(170, 85, 255))}
SyntaxV2.UIGradient_9.Rotation = 45
SyntaxV2.UIGradient_9.Parent = SyntaxV2.Title_3

SyntaxV2.Title_4.Name = "Title"
SyntaxV2.Title_4.Parent = SyntaxV2.Home
SyntaxV2.Title_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Title_4.BackgroundTransparency = 1.000
SyntaxV2.Title_4.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Title_4.Position = UDim2.new(0.111273795, 0, 0.0245773159, 0)
SyntaxV2.Title_4.Size = UDim2.new(0, 34, 0, 22)
SyntaxV2.Title_4.Font = Enum.Font.SourceSansBold
SyntaxV2.Title_4.Text = "V2"
SyntaxV2.Title_4.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Title_4.TextSize = 16.000
SyntaxV2.Title_4.TextStrokeTransparency = 0.000
SyntaxV2.Title_4.TextWrapped = true

SyntaxV2.UIGradient_10.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(0.99, Color3.fromRGB(83, 0, 125)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(0, 0, 0))}
SyntaxV2.UIGradient_10.Rotation = 45
SyntaxV2.UIGradient_10.Parent = SyntaxV2.Title_4

SyntaxV2.UIGradient_11.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(43, 0, 65)), ColorSequenceKeypoint.new(0.34, Color3.fromRGB(85, 0, 127)), ColorSequenceKeypoint.new(0.45, Color3.fromRGB(170, 0, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(21, 21, 21))}
SyntaxV2.UIGradient_11.Rotation = 45
SyntaxV2.UIGradient_11.Parent = SyntaxV2.Home

SyntaxV2.xd3.Name = "xd3"
SyntaxV2.xd3.Parent = SyntaxV2.Home
SyntaxV2.xd3.BackgroundColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.xd3.BackgroundTransparency = 0.350
SyntaxV2.xd3.BorderColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.xd3.Position = UDim2.new(0.21815519, 0, 0.125501618, 0)
SyntaxV2.xd3.Size = UDim2.new(0, 2, 0, 270)

SyntaxV2.UICorner_13.Parent = SyntaxV2.xd3

SyntaxV2.xd2.Name = "xd2"
SyntaxV2.xd2.Parent = SyntaxV2.Home
SyntaxV2.xd2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.xd2.BackgroundTransparency = 0.250
SyntaxV2.xd2.BorderColor3 = Color3.fromRGB(27, 42, 53)
SyntaxV2.xd2.BorderSizePixel = 0
SyntaxV2.xd2.Position = UDim2.new(0.233940244, 0, 0.134609684, 0)
SyntaxV2.xd2.Size = UDim2.new(0, 514, 0, 41)

SyntaxV2.UICorner_14.Parent = SyntaxV2.xd2

SyntaxV2.TextLabel.Parent = SyntaxV2.xd2
SyntaxV2.TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel.BackgroundTransparency = 1.000
SyntaxV2.TextLabel.Position = UDim2.new(-0.000587608665, 0, -0.00963014364, 0)
SyntaxV2.TextLabel.Size = UDim2.new(0, 49, 0, 18)
SyntaxV2.TextLabel.Font = Enum.Font.SourceSansBold
SyntaxV2.TextLabel.Text = "INFO"
SyntaxV2.TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel.TextSize = 14.000
SyntaxV2.TextLabel.TextStrokeTransparency = 0.460

SyntaxV2.UIGradient_12.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(170, 0, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(255, 255, 255))}
SyntaxV2.UIGradient_12.Rotation = 45
SyntaxV2.UIGradient_12.Parent = SyntaxV2.TextLabel

SyntaxV2.TextInfo.Name = "TextInfo"
SyntaxV2.TextInfo.Parent = SyntaxV2.xd2
SyntaxV2.TextInfo.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextInfo.BackgroundTransparency = 1.000
SyntaxV2.TextInfo.Position = UDim2.new(0.0190137569, 0, 0.424517393, 0)
SyntaxV2.TextInfo.Size = UDim2.new(0, 531, 0, 15)
SyntaxV2.TextInfo.Font = Enum.Font.TitilliumWeb
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."
SyntaxV2.TextInfo.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextInfo.TextSize = 19.000
SyntaxV2.TextInfo.TextXAlignment = Enum.TextXAlignment.Left

SyntaxV2.xd1.Name = "xd1"
SyntaxV2.xd1.Parent = SyntaxV2.Home
SyntaxV2.xd1.BackgroundColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.xd1.BackgroundTransparency = 0.350
SyntaxV2.xd1.BorderColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.xd1.Position = UDim2.new(-0.00292825769, 0, 0.0963753983, 0)
SyntaxV2.xd1.Size = UDim2.new(0, 112, 0, 2)

SyntaxV2.UICorner_15.Parent = SyntaxV2.xd1

SyntaxV2.Main1.Name = "Main1"
SyntaxV2.Main1.Parent = SyntaxV2.Home
SyntaxV2.Main1.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Main1.BackgroundTransparency = 1.000
SyntaxV2.Main1.Position = UDim2.new(0.233940244, 0, 0.279524237, 0)
SyntaxV2.Main1.Size = UDim2.new(0, 521, 0, 213)

SyntaxV2.Main2.Name = "Main2"
SyntaxV2.Main2.Parent = SyntaxV2.Main1
SyntaxV2.Main2.BackgroundColor3 = Color3.fromRGB(3, 0, 0)
SyntaxV2.Main2.BackgroundTransparency = 0.650
SyntaxV2.Main2.Position = UDim2.new(0.00587636186, 0, 0.0348671228, 0)
SyntaxV2.Main2.Size = UDim2.new(0, 507, 0, 199)

SyntaxV2.Executor.Name = "Executor"
SyntaxV2.Executor.Parent = SyntaxV2.Main2
SyntaxV2.Executor.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Executor.BackgroundTransparency = 1.000
SyntaxV2.Executor.Position = UDim2.new(0, 0, 1.0497365, 0)
SyntaxV2.Executor.Size = UDim2.new(0, 682, 0, 203)
SyntaxV2.Executor.Visible = false

SyntaxV2.Frame.Parent = SyntaxV2.Executor
SyntaxV2.Frame.BackgroundColor3 = Color3.fromRGB(143, 0, 214)
SyntaxV2.Frame.BackgroundTransparency = 1.000
SyntaxV2.Frame.Position = UDim2.new(-0.0782664865, 0, 0.178403541, 0)
SyntaxV2.Frame.Size = UDim2.new(0, 651, 0, 188)

SyntaxV2.UICorner_16.Parent = SyntaxV2.Frame

SyntaxV2.TextButton_5.Parent = SyntaxV2.Frame
SyntaxV2.TextButton_5.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextButton_5.BorderSizePixel = 0
SyntaxV2.TextButton_5.Position = UDim2.new(0.317000002, 0, -0.368999988, 0)
SyntaxV2.TextButton_5.Size = UDim2.new(0, 103, 0, 16)
SyntaxV2.TextButton_5.Font = Enum.Font.Sarpanch
SyntaxV2.TextButton_5.Text = "Clear"
SyntaxV2.TextButton_5.TextColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.TextButton_5.TextSize = 14.000
SyntaxV2.TextButton_5.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()
	SyntaxV2.TextButton_5.Size = UDim2.new(0, 90, 0, 13)
	wait(0.1)
	SyntaxV2.TextButton_5.Size = UDim2.new(0, 103, 0, 16)
	SyntaxV2.Executor_2.Text = ""
end)

SyntaxV2.UICorner_17.Parent = SyntaxV2.TextButton_5

SyntaxV2.TextButton_6.Parent = SyntaxV2.Frame
SyntaxV2.TextButton_6.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextButton_6.BorderSizePixel = 0
SyntaxV2.TextButton_6.Position = UDim2.new(0.1185361, 0, -0.368999988, 0)
SyntaxV2.TextButton_6.Size = UDim2.new(0, 103, 0, 16)
SyntaxV2.TextButton_6.Font = Enum.Font.Sarpanch
SyntaxV2.TextButton_6.Text = "Execute"
SyntaxV2.TextButton_6.TextColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.TextButton_6.TextSize = 14.000
SyntaxV2.TextButton_6.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()
	SyntaxV2.TextButton_6.Size = UDim2.new(0, 90, 0, 13)
	wait(0.1)
	SyntaxV2.TextButton_6.Size = UDim2.new(0, 103, 0, 16)

	if SyntaxV2.Executor_2.Text == "fly" then
SyntaxV2.TextInfo.Text = "[ FLY ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."
			SyntaxV2.Executor_2.Text = ""
--start
		Flying = true
		local Speed = 0
		local keys = {a = false, d = false, w = false, s = false}
		local Part = Instance.new("Part")
		local Weld = Instance.new("Weld", Part)
		Weld.Part0 = Part
		local Player = game:GetService("Players").LocalPlayer
		local Character = Player.Character
		repeat
			game:GetService("RunService").Heartbeat:wait()
		until Character:FindFirstChildOfClass("Humanoid")
		local HumanoidRootPart = Character.Humanoid.RootPart
		Part.Parent = workspace
		Weld.Parent = Part
		Part.Size = HumanoidRootPart.Size
		Part.CanCollide = false
		Part.Transparency = 1
		Weld.Part1 = HumanoidRootPart

		local pos = Instance.new("BodyPosition", Part)
		local gyro = Instance.new("BodyGyro", Part)

		pos.Name = "ProjectNull"
		gyro.Name = "OnTop"
		pos.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
		pos.Position = HumanoidRootPart.Position
		gyro.MaxTorque = Vector3.new(9e9, 9e9, 9e9)
		gyro.CFrame = HumanoidRootPart.CFrame

		local UserInputService = game:GetService("UserInputService")

		local ConnectA =
			UserInputService.InputBegan:Connect(
				function(Input, GameProcess)
				if not GameProcess then
					if Input.KeyCode == Enum.KeyCode.W then
						keys.w = true
					elseif Input.KeyCode == Enum.KeyCode.S then
						keys.s = true
					elseif Input.KeyCode == Enum.KeyCode.A then
						keys.a = true
					elseif Input.KeyCode == Enum.KeyCode.D then
						keys.d = true
					end
				end
			end
			)

		local ConnectB =
			UserInputService.InputEnded:Connect(
				function(Input, GameProcess)
				if not GameProcess then
					if Input.KeyCode == Enum.KeyCode.W then
						keys.w = false
					elseif Input.KeyCode == Enum.KeyCode.S then
						keys.s = false
					elseif Input.KeyCode == Enum.KeyCode.A then
						keys.a = false
					elseif Input.KeyCode == Enum.KeyCode.D then
						keys.d = false
					end
				end
			end
			)

		repeat
			game:GetService("RunService").Heartbeat:wait()
			Character:FindFirstChildOfClass("Humanoid").PlatformStand = true
			local new = gyro.cframe - gyro.cframe.p + pos.position
			if not keys.w and not keys.s and not keys.a and not keys.d then
				Speed = 1
			end

			if keys.w then
				new = new + workspace.CurrentCamera.CoordinateFrame.lookVector * Speed
				Speed = Speed + 0.01
			end

			if keys.s then
				new = new - workspace.CurrentCamera.CoordinateFrame.lookVector * Speed
				Speed = Speed + 0.01
			end

			if keys.d then
				new = new * CFrame.new(Speed, 0, 0)
				Speed = Speed + 0.01
			end

			if keys.a then
				new = new * CFrame.new(-Speed, 0, 0)
				Speed = Speed + 0.01
			end

			if Speed > 5 then
				Speed = 5
			end

			pos.position = new.p

			if keys.w then
				gyro.cframe = workspace.CurrentCamera.CoordinateFrame
			elseif keys.s then
				gyro.cframe = workspace.CurrentCamera.CoordinateFrame
			else
				gyro.cframe = workspace.CurrentCamera.CoordinateFrame
			end
		until not Flying

		if gyro then
			gyro:Destroy()
		end
		if pos then
			pos:Destroy()
		end
		Part:Destroy()
		Character:FindFirstChildOfClass("Humanoid").PlatformStand = false
		Speed = 0
		ConnectA:Disconnect()
		ConnectB:Disconnect()
		Fly()
--here info

	end


	if SyntaxV2.Executor_2.Text == "unfly" then

--here info

			SyntaxV2.Executor_2.Text = ""

		Flying = false
SyntaxV2.TextInfo.Text = "[ DISABLE FLY ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."
	end

	if SyntaxV2.Executor_2.Text == "noclip" then
--here info

			SyntaxV2.Executor_2.Text = ""
	local function nocl()
			for _, part in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
				if part:IsA("BasePart") and part.CanCollide == true then
					part.CanCollide = false
				end
			end
		end
		connectcl = game:GetService("RunService").Stepped:Connect(nocl)
SyntaxV2.TextInfo.Text = "[ NO-CLIP ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."
end
	if SyntaxV2.Executor_2.Text == "bodybomb" then
SyntaxV2.TextInfo.Text = "[ HumanoidBomb ] command loaded."
wait(1)

for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
			if v:IsA("BasePart") and v.Name ~="HumanoidRootPart" then 
				game:GetService("RunService").Heartbeat:connect(function()
					v.Velocity = Vector3.new(9999,0,0)
				end)
			end
		end
		wait()


game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = true
		local part1 = Instance.new("Part")
		part1.Parent = game.Workspace
		part1.Name = "Part1"
		wait()
		local humanoid = Instance.new("Humanoid")
		humanoid.Parent = part1
		game.Workspace.CurrentCamera.CameraSubject =game.Workspace.Part1
		hrp = game.Players.LocalPlayer.Character.HumanoidRootPart    
		bv = Instance.new("BodyVelocity", hrp)
		bv.Velocity = Vector3.new(50,5,40)
		wait()
		bv.Velocity = Vector3.new(50,5,40)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
		wait(2)
		game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = false

		power = 100
		wait()
		local bambam = Instance.new("BodyThrust")
		bambam.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
		bambam.Force = Vector3.new(power,0,power)
		bambam.Location = game.Players.LocalPlayer.Character.HumanoidRootPart.Position
		LocalPlayer = game.Players.LocalPlayer
		wait()
		spawn(function()
			game.Players.LocalPlayer.Character:BreakJoints()
			game.Players.LocalPlayer.Character.Head.CanCollide = false
			game.Players.LocalPlayer.Character.Torso.CanCollide = false
			game.Players.LocalPlayer.Character["Left Leg"].CanCollide = false
			game.Players.LocalPlayer.Character["Right Leg"].CanCollide = false
		end)
		local char = game.Players.LocalPlayer.Character
		local b = char["Right Arm"]
		local b1 = char["Left Arm"]
		local b2 = char["Right Leg"]
		local b3 = char["Left Leg"]
		hrp = game.Players.LocalPlayer.Character.HumanoidRootPart
		local bav = Instance.new("BodyAngularVelocity", hrp)
		bav.AngularVelocity = Vector3.new(0, 0, -1000)
		bav.MaxTorque = Vector3.new(math.huge, math.huge, math.huge)

		bv = Instance.new("BodyVelocity", hrp)
		bv.Velocity = Vector3.new(0,0,0)
		wait()
		bv.Velocity = Vector3.new(0,0,0)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)

		--bruh
		local bav = Instance.new("BodyAngularVelocity", b)
		bav.AngularVelocity = Vector3.new(0, 0, -10000)
		bav.MaxTorque = Vector3.new(math.huge, math.huge, math.huge)

		bv = Instance.new("BodyVelocity", b)
		bv.Velocity = Vector3.new(0,0,0)
		wait()
		bv.Velocity = Vector3.new(0,0,0)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
		--bruh

		--bruh
		local bav = Instance.new("BodyAngularVelocity", b1)
		bav.AngularVelocity = Vector3.new(0, 0, -10000)
		bav.MaxTorque = Vector3.new(math.huge, math.huge, math.huge)

		bv = Instance.new("BodyVelocity", b1)
		bv.Velocity = Vector3.new(0,0,0)
		wait()
		bv.Velocity = Vector3.new(0,0,0)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
		--bruh

		--bruh
		local bav = Instance.new("BodyAngularVelocity", b2)
		bav.AngularVelocity = Vector3.new(99, 99, -10000)
		bav.MaxTorque = Vector3.new(math.huge, math.huge, math.huge)

		bv = Instance.new("BodyVelocity", b2)
		bv.Velocity = Vector3.new(99,99,99)
		wait()
		bv.Velocity = Vector3.new(99,99,99)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
		--bruh
		--bruh
		local bav = Instance.new("BodyAngularVelocity", b3)
		bav.AngularVelocity = Vector3.new(9999, 9999, -10000)
		bav.MaxTorque = Vector3.new(math.huge, math.huge, math.huge)

		bv = Instance.new("BodyVelocity", b3)
		bv.Velocity = Vector3.new(99,99,99)
		wait()
		bv.Velocity = Vector3.new(99,99,99)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
		--bruh

		local Players = Game:GetService("Players")
		local GetPlayers = Players:GetPlayers()
		local Player = Players.LocalPlayer
		local Character = Player.Character
		local RunService = Game:GetService("RunService")
		local Heartbeat = RunService.Heartbeat
		local Sitting = {}

		while true do
			wait(0.000000000000000000000000000000000000000000000000000000000000000000000000000000001)
			for _,Players in next, GetPlayers do
				if Players.Character then
					repeat Heartbeat:wait() until Character:FindFirstChild("Right Arm")
					repeat Heartbeat:wait() until Players.Character:FindFirstChild("Humanoid")
					repeat Heartbeat:wait() until Players.Character:FindFirstChild("HumanoidRootPart")
					if Players.Character:FindFirstChild("Humanoid").Sit ~= true then
						table.insert(Sitting,x)
						Character["Right Arm"]:BreakJoints()
						Character["Left Arm"]:BreakJoints()
						Character["Right Leg"]:BreakJoints()
						Character["Left Leg"]:BreakJoints()
						Character:FindFirstChild("Right Arm").CFrame = Players.Character:FindFirstChild("HumanoidRootPart").CFrame
						Character:FindFirstChild("Left Arm").CFrame = Players.Character:FindFirstChild("HumanoidRootPart").CFrame
						Character:FindFirstChild("Right Leg").CFrame = Players.Character:FindFirstChild("HumanoidRootPart").CFrame
						Character:FindFirstChild("Left Leg").CFrame = Players.Character:FindFirstChild("HumanoidRootPart").CFrame
						Character:FindFirstChild("HumanoidRootPart").CFrame = Players.Character:FindFirstChild("HumanoidRootPart").CFrame
					end
				end
				SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."
			SyntaxV2.Executor_2.Text = ""
	end
			end
			end
	
	if SyntaxV2.Executor_2.Text == "rj" then
		game:GetService("TeleportService"):Teleport(game.PlaceId,
		game:GetService("Players").LocalPlayer)
end
	if SyntaxV2.Executor_2.Text == "re" then
SyntaxV2.TextInfo.Text = "[ RESPAWN ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."
			SyntaxV2.Executor_2.Text = ""
	lplayer = game:GetService("Players").LocalPlayer
		saved = lplayer.Character.HumanoidRootPart.CFrame

		for _, child in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
			if child:IsA("BasePart") then
				child:Destroy()
			end
		end
		wait(6)
		lplayer.Character.HumanoidRootPart.CFrame = saved
lplayer.Character.ForceField:Destroy()
--here info

end
	if SyntaxV2.Executor_2.Text == "clip" then
--here info
SyntaxV2.TextInfo.Text = "[ DISABLE NOCLIP ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."
			SyntaxV2.Executor_2.Text = ""
		connectcl:Disconnect()
end

	if SyntaxV2.Executor_2.Text == "bodybomb" then
--here info
SyntaxV2.TextInfo.Text = "[ HUMANOID BOMB ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."
			SyntaxV2.Executor_2.Text = ""
	for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
			if v:IsA("BasePart") and v.Name ~="HumanoidRootPart" then 
				game:GetService("RunService").Heartbeat:connect(function()
					v.Velocity = Vector3.new(99999,0,0)
				end)
			end
		end
		wait()

		game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = true
		local part1 = Instance.new("Part")
		part1.Parent = game.Workspace
		part1.Name = "Part1"
		wait()
		local humanoid = Instance.new("Humanoid")
		humanoid.Parent = part1
		game.Workspace.CurrentCamera.CameraSubject =game.Workspace.Part1
		hrp = game.Players.LocalPlayer.Character.HumanoidRootPart    
		bv = Instance.new("BodyVelocity", hrp)
		bv.Velocity = Vector3.new(50,5,40)
		wait()
		bv.Velocity = Vector3.new(50,5,40)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
		wait(2)
		game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = false

		power = 100
		wait()
		local bambam = Instance.new("BodyThrust")
		bambam.Parent = game.Players.LocalPlayer.Character.HumanoidRootPart
		bambam.Force = Vector3.new(power,0,power)
		bambam.Location = game.Players.LocalPlayer.Character.HumanoidRootPart.Position
		LocalPlayer = game.Players.LocalPlayer
		wait()
		spawn(function()
			game.Players.LocalPlayer.Character:BreakJoints()
			game.Players.LocalPlayer.Character.Head.CanCollide = false
			game.Players.LocalPlayer.Character.Torso.CanCollide = false
			game.Players.LocalPlayer.Character["Left Leg"].CanCollide = false
			game.Players.LocalPlayer.Character["Right Leg"].CanCollide = false
		end)
		local char = game.Players.LocalPlayer.Character
		local b = char["Right Arm"]
		local b1 = char["Left Arm"]
		local b2 = char["Right Leg"]
		local b3 = char["Left Leg"]
		hrp = game.Players.LocalPlayer.Character.HumanoidRootPart
		local bav = Instance.new("BodyAngularVelocity", hrp)
		bav.AngularVelocity = Vector3.new(0, 0, -1000)
		bav.MaxTorque = Vector3.new(math.huge, math.huge, math.huge)

		bv = Instance.new("BodyVelocity", hrp)
		bv.Velocity = Vector3.new(0,0,0)
		wait()
		bv.Velocity = Vector3.new(0,0,0)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)

		--bruh
		local bav = Instance.new("BodyAngularVelocity", b)
		bav.AngularVelocity = Vector3.new(0, 0, -10000)
		bav.MaxTorque = Vector3.new(math.huge, math.huge, math.huge)

		bv = Instance.new("BodyVelocity", b)
		bv.Velocity = Vector3.new(0,0,0)
		wait()
		bv.Velocity = Vector3.new(0,0,0)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
		--bruh

		--bruh
		local bav = Instance.new("BodyAngularVelocity", b1)
		bav.AngularVelocity = Vector3.new(0, 0, -10000)
		bav.MaxTorque = Vector3.new(math.huge, math.huge, math.huge)

		bv = Instance.new("BodyVelocity", b1)
		bv.Velocity = Vector3.new(0,0,0)
		wait()
		bv.Velocity = Vector3.new(0,0,0)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
		--bruh

		--bruh
		local bav = Instance.new("BodyAngularVelocity", b2)
		bav.AngularVelocity = Vector3.new(99, 99, -10000)
		bav.MaxTorque = Vector3.new(math.huge, math.huge, math.huge)

		bv = Instance.new("BodyVelocity", b2)
		bv.Velocity = Vector3.new(99,99,99)
		wait()
		bv.Velocity = Vector3.new(99,99,99)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
		--bruh
		--bruh
		local bav = Instance.new("BodyAngularVelocity", b3)
		bav.AngularVelocity = Vector3.new(9999, 9999, -10000)
		bav.MaxTorque = Vector3.new(math.huge, math.huge, math.huge)

		bv = Instance.new("BodyVelocity", b3)
		bv.Velocity = Vector3.new(99,99,99)
		wait()
		bv.Velocity = Vector3.new(99,99,99)
		bv.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
		--bruh

		local Players = Game:GetService("Players")
		local GetPlayers = Players:GetPlayers()
		local Player = Players.LocalPlayer
		local Character = Player.Character
		local RunService = Game:GetService("RunService")
		local Heartbeat = RunService.Heartbeat
		local Sitting = {}

		while true do
			wait(0.000000000000000000000000000000000000000000000000000000000000000000000000000000001)
			for _,Players in next, GetPlayers do
				if Players.Character then
					repeat Heartbeat:wait() until Character:FindFirstChild("Right Arm")
					repeat Heartbeat:wait() until Players.Character:FindFirstChild("Humanoid")
					repeat Heartbeat:wait() until Players.Character:FindFirstChild("HumanoidRootPart")
					if Players.Character:FindFirstChild("Humanoid").Sit ~= true then
						table.insert(Sitting,x)
						Character["Right Arm"]:BreakJoints()
						Character["Left Arm"]:BreakJoints()
						Character["Right Leg"]:BreakJoints()
						Character["Left Leg"]:BreakJoints()
						Character:FindFirstChild("Right Arm").CFrame = Players.Character:FindFirstChild("HumanoidRootPart").CFrame
						Character:FindFirstChild("Left Arm").CFrame = Players.Character:FindFirstChild("HumanoidRootPart").CFrame
						Character:FindFirstChild("Right Leg").CFrame = Players.Character:FindFirstChild("HumanoidRootPart").CFrame
						Character:FindFirstChild("Left Leg").CFrame = Players.Character:FindFirstChild("HumanoidRootPart").CFrame
						Character:FindFirstChild("HumanoidRootPart").CFrame = Players.Character:FindFirstChild("HumanoidRootPart").CFrame
					end
				end
			end
		end
	end

	if string.sub(SyntaxV2.Executor_2.Text, 1, 7) == ("finger ") then

		for i,v in pairs(GetPlayer(string.sub(SyntaxV2.Executor_2.Text, 8)))do

			for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
				if v:IsA("BasePart") and v.Name ~="HumanoidRootPart" then 
					game:GetService("RunService").Heartbeat:connect(function()
						v.Velocity = Vector3.new(45,0,0)
					end)
				end
			end
			wait(0.1)

			local player = game.Players.LocalPlayer
			local target = game.Players[v.Name].Character

			local head = player.Character.WDW_FoamFinger

			local root = target.HumanoidRootPart


			function weld(hat, position, orientation)
				local attachment = Instance.new("Attachment")
				attachment.Parent = root
				attachment.Name = hat:GetFullName()
				attachment.Position = position
				attachment.Orientation = orientation

				local attach0 = hat.Handle:FindFirstChildOfClass("Attachment")
				local attach1 = attachment

				hat.Handle.AccessoryWeld:Destroy()
				local alignP = Instance.new("AlignPosition")
				alignP.Parent = hat.Handle
				alignP.Attachment0 = attach0
				alignP.Attachment1 = attach1
				alignP.Responsiveness = 200
				alignP.RigidityEnabled = true

				local alignO = Instance.new("AlignOrientation")
				alignO.Parent = hat.Handle
				alignO.Attachment0 = attach0
				alignO.Attachment1 = attach1
				alignO.MaxTorque = 9e99
				alignO.MaxAngularVelocity = 9e99
				alignO.PrimaryAxisOnly = false
				alignO.ReactionTorqueEnabled = false
				alignO.Responsiveness = 200
				alignO.RigidityEnabled = false
			end

			function reWeld(hat, position, orientation) --Object, Vector3, Optional Vector3
				local attachmentP = hat.Handle:FindFirstChildOfClass("AlignPosition").Attachment1
				local attachmentO = hat.Handle:FindFirstChildOfClass("AlignOrientation").Attachment1
				attachmentP.Position = position
				orientation = orientation or attachmentO.Orientation --this line is what makes orientation an optional argument
				attachmentO.Orientation = orientation --under the circumstances of this unmodified script attachmentP and attachmentO are the same. the redundancy for people who wanna edit this who don't know what they're doing.
			end

			weld(head, Vector3.new(0.2, -2, 2), Vector3.new(-0, -90, 90))

			--reweld example
			local UIS = game:GetService("UserInputService")
			local readySlam = true
			UIS.InputBegan:Connect(function(key, gpi)
				if readySlam and key.KeyCode == Enum.KeyCode.Q and not gpi then --gpi or GameProcessedEvent tells you whether the button (Q) was pressed in chat or a TextBox GUI etc. for more information on the KeyCodes (say if you want to detect pressing enter) go to https://developer.roblox.com/en-us/api-reference/property/InputObject/KeyCode
					--preparing slam
					readySlam = false
					reWeld(head, Vector3.new(0.2, -1.6, 1.5), Vector3.new(-0, -90, 110))
					wait(0.5)
					reWeld(head, Vector3.new(0.2, -2, 2), Vector3.new(-0, -90, 90))
					wait(0.5)
					reWeld(head, Vector3.new(0.2, -1.6, 1.5), Vector3.new(-0, -90, 110))
					wait(0.5)
					reWeld(head, Vector3.new(0.2, -2, 2), Vector3.new(-0, -90, 90))
					wait(0.5)
					reWeld(head, Vector3.new(0.2, -1.6, 1.5), Vector3.new(-0, -90, 110))
					wait(0.5)
					reWeld(head, Vector3.new(0.2, -2, 2), Vector3.new(-0, -90, 90))
					readySlam = true
				end
			end)

		end
	end


	if string.sub(SyntaxV2.Executor_2.Text, 1, 3) == ("pp ") then

		for i,v in pairs(GetPlayer(string.sub(SyntaxV2.Executor_2.Text, 4)))do


local player = game.Players.LocalPlayer
local target = game.Players[v.Name].Character --you can change this to give the titan to someone else and get them banned probably lol

			for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
				if v:IsA("BasePart") and v.Name ~="HumanoidRootPart" then 
					game:GetService("RunService").Heartbeat:connect(function()
						v.Velocity = Vector3.new(45,0,0)
					end)
				end
			end
			wait(0.1)

local LocalPlayer = game.Players.LocalPlayer;local Character = LocalPlayer.Character;local Mouse = LocalPlayer:GetMouse()
Character["Pal Hair"].Name = "Test1";Character["InternationalFedora"].Name = "Test2"
Character["InternationalFedora"].Name = "Test3"

local char = game.Players.LocalPlayer.Character
local HatName = "Test1"
local Hat = char[HatName]
Hat.Handle:FindFirstChild("Mesh"):Destroy()
Hat.Handle.CanCollide = false

local char = game.Players.LocalPlayer.Character
local HatName = "LavanderHair"
local Hat = char[HatName]
Hat.Handle:FindFirstChild("Mesh"):Destroy()
Hat.Handle.CanCollide = false

local char = game.Players.LocalPlayer.Character
local HatName = "Test2"
local Hat = char[HatName]
Hat.Handle.SpecialMesh:Destroy()
Hat.Handle.CanCollide = false

local char = game.Players.LocalPlayer.Character
local HatName = "Test3"
local Hat = char[HatName]
Hat.Handle.SpecialMesh:Destroy()
Hat.Handle.CanCollide = false

local d1 = player.Character["Test1"]
local d2 = player.Character["Test2"]
local d3 = player.Character["Test3"]
local d4 = player.Character["LavanderHair"]

local root = target.HumanoidRootPart


--terrible coding over

function weld(hat, position, orientation) --Object, Vector3, Vector3
local attachment = Instance.new("Attachment")
attachment.Parent = root
attachment.Name = hat:GetFullName()
attachment.Position = position
attachment.Orientation = orientation

local attach0 = hat.Handle:FindFirstChildOfClass("Attachment")
local attach1 = attachment

hat.Handle.AccessoryWeld:Destroy()
local alignP = Instance.new("AlignPosition")
alignP.Parent = hat.Handle
alignP.Attachment0 = attach0
alignP.Attachment1 = attach1
alignP.Responsiveness = 200
alignP.RigidityEnabled = true

local alignO = Instance.new("AlignOrientation")
alignO.Parent = hat.Handle
alignO.Attachment0 = attach0
alignO.Attachment1 = attach1
alignO.MaxTorque = 9e99
alignO.MaxAngularVelocity = 9e99
alignO.PrimaryAxisOnly = false
alignO.ReactionTorqueEnabled = false
alignO.Responsiveness = 200
alignO.RigidityEnabled = false
end

function reWeld(hat, position, orientation) --Object, Vector3, Optional Vector3
local attachmentP = hat.Handle:FindFirstChildOfClass("AlignPosition").Attachment1
local attachmentO = hat.Handle:FindFirstChildOfClass("AlignOrientation").Attachment1
attachmentP.Position = position
orientation = orientation or attachmentO.Orientation --this line is what makes orientation an optional argument
attachmentO.Orientation = orientation --under the circumstances of this unmodified script attachmentP and attachmentO are the same. the redundancy for people who wanna edit this who don't know what they're doing.
end

weld(d1, Vector3.new(0,-0.8,4), Vector3.new(0, 0,0))
weld(d2, Vector3.new(-0.6, -2,4.6), Vector3.new(0, 0, 0))
weld(d3, Vector3.new(0.6, -2,4.6), Vector3.new(0, 0, 0))
weld(d4, Vector3.new(0,-0.95,2), Vector3.new(0, 0,0))

--reweld example
local UIS = game:GetService("UserInputService")
local readySlam = true
UIS.InputBegan:Connect(function(key, gpi)
if readySlam and key.KeyCode == Enum.KeyCode.Q and not gpi then --gpi or GameProcessedEvent tells you whether the button (Q) was pressed in chat or a TextBox GUI etc. for more information on the KeyCodes (say if you want to detect pressing enter) go to https://developer.roblox.com/en-us/api-reference/property/InputObject/KeyCode
--preparing slam
readySlam = false
reWeld(d1, Vector3.new(0,-0.8,2), Vector3.new(0, 0,0))
reWeld(d2, Vector3.new(-0.6, -2,2.6), Vector3.new(0, 0, 0))
reWeld(d3, Vector3.new(0.6, -2,2.6), Vector3.new(0, 0, 0))
reWeld(d4, Vector3.new(0,-0.95,0.5), Vector3.new(0, 0,0))
wait(1)
reWeld(d1, Vector3.new(0,-0.8,4), Vector3.new(0, 0,0))
reWeld(d2, Vector3.new(-0.6, -2,4.6), Vector3.new(0, 0, 0))
reWeld(d3, Vector3.new(0.6, -2,4.6), Vector3.new(0, 0, 0))
reWeld(d4, Vector3.new(0,-0.95,2), Vector3.new(0, 0,0))

readySlam = true
end
end)

local UIS = game:GetService("UserInputService")
local readySlam = true
UIS.InputBegan:Connect(function(key, gpi)
if readySlam and key.KeyCode == Enum.KeyCode.E and not gpi then
--preparing slam
readySlam = false

reWeld(d1, Vector3.new(0,1.5,-0.8), Vector3.new(0, 0,0))
reWeld(d2, Vector3.new(-0.6, 0.5,-3), Vector3.new(0, 0, 0))
reWeld(d3, Vector3.new(0.6, 0.5,-3), Vector3.new(0, 0, 0))
reWeld(d4, Vector3.new(0,1.35,-2.5), Vector3.new(0, 0,0))
wait(1)
reWeld(d1, Vector3.new(0,1.5,-3.5), Vector3.new(0, 0,0))
reWeld(d2, Vector3.new(-0.6, 0.5,-4.6), Vector3.new(0, 0, 0))
reWeld(d3, Vector3.new(0.6, 0.5,-4.6), Vector3.new(0, 0, 0))
reWeld(d4, Vector3.new(0,1.35,-2.5), Vector3.new(0, 0,0))

readySlam = true
end
end)
end
end



end)

SyntaxV2.UICorner_18.Parent = SyntaxV2.TextButton_6

SyntaxV2.Executor_2.Name = "Executor"
SyntaxV2.Executor_2.Parent = SyntaxV2.Frame
SyntaxV2.Executor_2.BackgroundColor3 = Color3.fromRGB(118, 59, 177)
SyntaxV2.Executor_2.Position = UDim2.new(0.108136393, 0, -0.639649749, 0)
SyntaxV2.Executor_2.Size = UDim2.new(0, 246, 0, 44)
SyntaxV2.Executor_2.Font = Enum.Font.Sarpanch
SyntaxV2.Executor_2.PlaceholderText = "Insert Command"
SyntaxV2.Executor_2.Text = ""
SyntaxV2.Executor_2.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Executor_2.TextSize = 14.000

SyntaxV2.UICorner_19.Parent = SyntaxV2.Executor_2

SyntaxV2.UIGradient_13.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 85, 127)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(45, 45, 45))}
SyntaxV2.UIGradient_13.Rotation = 45
SyntaxV2.UIGradient_13.Parent = SyntaxV2.Executor_2

SyntaxV2.Frame_2.Parent = SyntaxV2.Frame
SyntaxV2.Frame_2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Frame_2.BackgroundTransparency = 0.450
SyntaxV2.Frame_2.BorderColor3 = Color3.fromRGB(27, 42, 53)
SyntaxV2.Frame_2.Position = UDim2.new(0.118660502, 0, -0.80279237, 0)
SyntaxV2.Frame_2.Size = UDim2.new(0, 233, 0, 21)

SyntaxV2.TextLabel_2.Parent = SyntaxV2.Frame_2
SyntaxV2.TextLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel_2.BackgroundTransparency = 1.000
SyntaxV2.TextLabel_2.Position = UDim2.new(0.00899999961, 0, 0.100000001, 0)
SyntaxV2.TextLabel_2.Size = UDim2.new(0, 230, 0, 16)
SyntaxV2.TextLabel_2.Font = Enum.Font.TitilliumWeb
SyntaxV2.TextLabel_2.Text = "Execute commands without capitals"
SyntaxV2.TextLabel_2.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel_2.TextSize = 19.000
SyntaxV2.TextLabel_2.TextStrokeTransparency = 0.000
SyntaxV2.TextLabel_2.TextWrapped = true

SyntaxV2.UICorner_20.Parent = SyntaxV2.Frame_2

SyntaxV2.ImageLabel.Parent = SyntaxV2.Frame
SyntaxV2.ImageLabel.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
SyntaxV2.ImageLabel.BackgroundTransparency = 0.600
SyntaxV2.ImageLabel.Position = UDim2.new(0.246268809, 0, -1.23364341, 0)
SyntaxV2.ImageLabel.Size = UDim2.new(0, 68, 0, 68)
SyntaxV2.ImageLabel.ZIndex = 3
SyntaxV2.ImageLabel.Image = "https://www.roblox.com/headshot-thumbnail/image?userId=1852211292&width=420&height=420&format=png"

SyntaxV2.UICorner_21.CornerRadius = UDim.new(0, 40)
SyntaxV2.UICorner_21.Parent = SyntaxV2.ImageLabel

SyntaxV2.UIGradient_14.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(115, 57, 173)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(45, 45, 45))}
SyntaxV2.UIGradient_14.Rotation = 45
SyntaxV2.UIGradient_14.Parent = SyntaxV2.Frame

SyntaxV2.Frame_3.Parent = SyntaxV2.Frame
SyntaxV2.Frame_3.BackgroundColor3 = Color3.fromRGB(105, 0, 158)
SyntaxV2.Frame_3.BackgroundTransparency = 0.250
SyntaxV2.Frame_3.BorderColor3 = Color3.fromRGB(27, 42, 53)
SyntaxV2.Frame_3.Position = UDim2.new(0.509826124, 0, -1.23723018, 0)
SyntaxV2.Frame_3.Size = UDim2.new(0, 215, 0, 23)

SyntaxV2.UICorner_22.Parent = SyntaxV2.Frame_3

SyntaxV2.TextLabel_3.Parent = SyntaxV2.Frame_3
SyntaxV2.TextLabel_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel_3.BackgroundTransparency = 1.000
SyntaxV2.TextLabel_3.BorderColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.TextLabel_3.Position = UDim2.new(0, 0, -0.0377807617, 0)
SyntaxV2.TextLabel_3.Size = UDim2.new(0, 215, 0, 23)
SyntaxV2.TextLabel_3.Font = Enum.Font.SourceSansBold
SyntaxV2.TextLabel_3.Text = "Commands List"
SyntaxV2.TextLabel_3.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel_3.TextSize = 17.000
SyntaxV2.TextLabel_3.TextStrokeTransparency = 0.000
SyntaxV2.TextLabel_3.TextWrapped = true

SyntaxV2.UIGradient_15.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(43, 0, 65)), ColorSequenceKeypoint.new(0.03, Color3.fromRGB(169, 0, 254)), ColorSequenceKeypoint.new(0.73, Color3.fromRGB(170, 0, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(170, 0, 255))}
SyntaxV2.UIGradient_15.Rotation = 45
SyntaxV2.UIGradient_15.Parent = SyntaxV2.Frame_3

SyntaxV2.Commands_4.Name = "Commands"
SyntaxV2.Commands_4.Parent = SyntaxV2.Frame
SyntaxV2.Commands_4.BackgroundColor3 = Color3.fromRGB(170, 0, 127)
SyntaxV2.Commands_4.BackgroundTransparency = 1.000
SyntaxV2.Commands_4.Position = UDim2.new(0.842904389, -250, 0.943212807, -150)
SyntaxV2.Commands_4.Size = UDim2.new(0, 342, 0, 150)

SyntaxV2.UIGradient_16.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(115, 57, 173)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(45, 45, 45))}
SyntaxV2.UIGradient_16.Rotation = 45
SyntaxV2.UIGradient_16.Parent = SyntaxV2.Commands_4

SyntaxV2.UICorner_23.Parent = SyntaxV2.Commands_4

SyntaxV2.Frame_4.Parent = SyntaxV2.Commands_4
SyntaxV2.Frame_4.BackgroundColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.Frame_4.BackgroundTransparency = 1.000
SyntaxV2.Frame_4.Position = UDim2.new(0.124754429, 0, -1.57018936, 0)
SyntaxV2.Frame_4.Size = UDim2.new(0, 218, 0, 161)

SyntaxV2.UICorner_24.Parent = SyntaxV2.Frame_4

SyntaxV2.UIGradient_17.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(115, 57, 173)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(45, 45, 45))}
SyntaxV2.UIGradient_17.Rotation = 45
SyntaxV2.UIGradient_17.Parent = SyntaxV2.Frame_4

SyntaxV2.ScrollingFrame.Parent = SyntaxV2.Frame_4
SyntaxV2.ScrollingFrame.Active = true
SyntaxV2.ScrollingFrame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.ScrollingFrame.BackgroundTransparency = 1.000
SyntaxV2.ScrollingFrame.BorderColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.ScrollingFrame.Position = UDim2.new(-0.0733944923, 0, 0.0559002422, 0)
SyntaxV2.ScrollingFrame.Size = UDim2.new(0, 234, 0, 145)
SyntaxV2.ScrollingFrame.CanvasSize = UDim2.new(0, 0, 5, 0)

SyntaxV2.Cmd1.Name = "Cmd1"
SyntaxV2.Cmd1.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd1.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd1.BackgroundTransparency = 0.550
SyntaxV2.Cmd1.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd1.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd1.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd1.Font = Enum.Font.Nunito
SyntaxV2.Cmd1.Text = "pp [VICTIM]"
SyntaxV2.Cmd1.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd1.TextSize = 14.000
SyntaxV2.Cmd1.TextStrokeTransparency = 0.000

SyntaxV2.UIListLayout.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
SyntaxV2.UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
SyntaxV2.UIListLayout.Padding = UDim.new(0, 7)

SyntaxV2.Cmd2.Name = "Cmd2"
SyntaxV2.Cmd2.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd2.BackgroundTransparency = 0.550
SyntaxV2.Cmd2.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd2.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd2.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd2.Font = Enum.Font.Nunito
SyntaxV2.Cmd2.Text = "finger [VICTIM]"
SyntaxV2.Cmd2.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd2.TextSize = 14.000
SyntaxV2.Cmd2.TextStrokeTransparency = 0.000

SyntaxV2.Cmd3.Name = "Cmd3"
SyntaxV2.Cmd3.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd3.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd3.BackgroundTransparency = 0.550
SyntaxV2.Cmd3.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd3.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd3.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd3.Font = Enum.Font.Nunito
SyntaxV2.Cmd3.Text = "re | respawn"
SyntaxV2.Cmd3.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd3.TextSize = 14.000
SyntaxV2.Cmd3.TextStrokeTransparency = 0.000

SyntaxV2.Cmd4.Name = "Cmd4"
SyntaxV2.Cmd4.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd4.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd4.BackgroundTransparency = 0.550
SyntaxV2.Cmd4.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd4.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd4.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd4.Font = Enum.Font.Nunito
SyntaxV2.Cmd4.Text = "bodybomb"
SyntaxV2.Cmd4.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd4.TextSize = 14.000
SyntaxV2.Cmd4.TextStrokeTransparency = 0.000

SyntaxV2.Cmd5.Name = "Cmd5"
SyntaxV2.Cmd5.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd5.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd5.BackgroundTransparency = 0.550
SyntaxV2.Cmd5.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd5.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd5.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd5.Font = Enum.Font.Nunito
SyntaxV2.Cmd5.Text = "fly | enable fly"
SyntaxV2.Cmd5.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd5.TextSize = 14.000
SyntaxV2.Cmd5.TextStrokeTransparency = 0.000

SyntaxV2.Cmd6.Name = "Cmd6"
SyntaxV2.Cmd6.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd6.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd6.BackgroundTransparency = 0.550
SyntaxV2.Cmd6.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd6.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd6.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd6.Font = Enum.Font.Nunito
SyntaxV2.Cmd6.Text = "unfly | disable fly"
SyntaxV2.Cmd6.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd6.TextSize = 14.000
SyntaxV2.Cmd6.TextStrokeTransparency = 0.000

SyntaxV2.Cmd7.Name = "Cmd7"
SyntaxV2.Cmd7.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd7.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd7.BackgroundTransparency = 0.550
SyntaxV2.Cmd7.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd7.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd7.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd7.Font = Enum.Font.Nunito
SyntaxV2.Cmd7.Text = "noclip | enable"
SyntaxV2.Cmd7.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd7.TextSize = 14.000
SyntaxV2.Cmd7.TextStrokeTransparency = 0.000

SyntaxV2.Cmd8.Name = "Cmd8"
SyntaxV2.Cmd8.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd8.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd8.BackgroundTransparency = 0.550
SyntaxV2.Cmd8.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd8.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd8.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd8.Font = Enum.Font.Nunito
SyntaxV2.Cmd8.Text = "clip | disable"
SyntaxV2.Cmd8.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd8.TextSize = 14.000
SyntaxV2.Cmd8.TextStrokeTransparency = 0.000

SyntaxV2.Cmd9.Name = "Cmd9"
SyntaxV2.Cmd9.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd9.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd9.BackgroundTransparency = 0.550
SyntaxV2.Cmd9.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd9.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd9.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd9.Visible = true
SyntaxV2.Cmd9.Font = Enum.Font.Nunito
SyntaxV2.Cmd9.Text = "rj | rejoin game"
SyntaxV2.Cmd9.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd9.TextSize = 14.000
SyntaxV2.Cmd9.TextStrokeTransparency = 0.000

SyntaxV2.Cmd10.Name = "Cmd10"
SyntaxV2.Cmd10.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd10.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd10.BackgroundTransparency = 0.550
SyntaxV2.Cmd10.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd10.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd10.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd10.Visible = false
SyntaxV2.Cmd10.Font = Enum.Font.Nunito
SyntaxV2.Cmd10.Text = "x"
SyntaxV2.Cmd10.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd10.TextSize = 14.000
SyntaxV2.Cmd10.TextStrokeTransparency = 0.000

SyntaxV2.Cmd11.Name = "Cmd11"
SyntaxV2.Cmd11.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd11.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd11.BackgroundTransparency = 0.550
SyntaxV2.Cmd11.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd11.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd11.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd11.Visible = false
SyntaxV2.Cmd11.Font = Enum.Font.Nunito
SyntaxV2.Cmd11.Text = "x"
SyntaxV2.Cmd11.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd11.TextSize = 14.000
SyntaxV2.Cmd11.TextStrokeTransparency = 0.000

SyntaxV2.Cmd12.Name = "Cmd12"
SyntaxV2.Cmd12.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd12.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd12.BackgroundTransparency = 0.550
SyntaxV2.Cmd12.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd12.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd12.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd12.Visible = false
SyntaxV2.Cmd12.Font = Enum.Font.Nunito
SyntaxV2.Cmd12.Text = "x"
SyntaxV2.Cmd12.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd12.TextSize = 14.000
SyntaxV2.Cmd12.TextStrokeTransparency = 0.000

SyntaxV2.Cmd13.Name = "Cmd13"
SyntaxV2.Cmd13.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd13.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd13.BackgroundTransparency = 0.550
SyntaxV2.Cmd13.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd13.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd13.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd13.Visible = false
SyntaxV2.Cmd13.Font = Enum.Font.Nunito
SyntaxV2.Cmd13.Text = "x"
SyntaxV2.Cmd13.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd13.TextSize = 14.000
SyntaxV2.Cmd13.TextStrokeTransparency = 0.000

SyntaxV2.Cmd14.Name = "Cmd14"
SyntaxV2.Cmd14.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd14.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd14.BackgroundTransparency = 0.550
SyntaxV2.Cmd14.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd14.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd14.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd14.Visible = false
SyntaxV2.Cmd14.Font = Enum.Font.Nunito
SyntaxV2.Cmd14.Text = "x"
SyntaxV2.Cmd14.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd14.TextSize = 14.000
SyntaxV2.Cmd14.TextStrokeTransparency = 0.000

SyntaxV2.Cmd15.Name = "Cmd15"
SyntaxV2.Cmd15.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd15.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd15.BackgroundTransparency = 0.550
SyntaxV2.Cmd15.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd15.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd15.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd15.Visible = false
SyntaxV2.Cmd15.Font = Enum.Font.Nunito
SyntaxV2.Cmd15.Text = "x"
SyntaxV2.Cmd15.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd15.TextSize = 14.000
SyntaxV2.Cmd15.TextStrokeTransparency = 0.000

SyntaxV2.Cmd16.Name = "Cmd16"
SyntaxV2.Cmd16.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd16.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd16.BackgroundTransparency = 0.550
SyntaxV2.Cmd16.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd16.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd16.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd16.Visible = false
SyntaxV2.Cmd16.Font = Enum.Font.Nunito
SyntaxV2.Cmd16.Text = "x"
SyntaxV2.Cmd16.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd16.TextSize = 14.000
SyntaxV2.Cmd16.TextStrokeTransparency = 0.000

SyntaxV2.Cmd17.Name = "Cmd17"
SyntaxV2.Cmd17.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd17.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd17.BackgroundTransparency = 0.550
SyntaxV2.Cmd17.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd17.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd17.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd17.Visible = false
SyntaxV2.Cmd17.Font = Enum.Font.Nunito
SyntaxV2.Cmd17.Text = "x"
SyntaxV2.Cmd17.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd17.TextSize = 14.000
SyntaxV2.Cmd17.TextStrokeTransparency = 0.000

SyntaxV2.Cmd18.Name = "Cmd18"
SyntaxV2.Cmd18.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd18.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd18.BackgroundTransparency = 0.550
SyntaxV2.Cmd18.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd18.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd18.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd18.Visible = false
SyntaxV2.Cmd18.Font = Enum.Font.Nunito
SyntaxV2.Cmd18.Text = "x"
SyntaxV2.Cmd18.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd18.TextSize = 14.000
SyntaxV2.Cmd18.TextStrokeTransparency = 0.000

SyntaxV2.Cmd19.Name = "Cmd19"
SyntaxV2.Cmd19.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd19.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd19.BackgroundTransparency = 0.550
SyntaxV2.Cmd19.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd19.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd19.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd19.Visible = false
SyntaxV2.Cmd19.Font = Enum.Font.Nunito
SyntaxV2.Cmd19.Text = "x"
SyntaxV2.Cmd19.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd19.TextSize = 14.000
SyntaxV2.Cmd19.TextStrokeTransparency = 0.000

SyntaxV2.Cmd20.Name = "Cmd20"
SyntaxV2.Cmd20.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd20.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd20.BackgroundTransparency = 0.550
SyntaxV2.Cmd20.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd20.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd20.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd20.Visible = false
SyntaxV2.Cmd20.Font = Enum.Font.Nunito
SyntaxV2.Cmd20.Text = "x"
SyntaxV2.Cmd20.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd20.TextSize = 14.000
SyntaxV2.Cmd20.TextStrokeTransparency = 0.000

SyntaxV2.Cmd21.Name = "Cmd21"
SyntaxV2.Cmd21.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd21.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd21.BackgroundTransparency = 0.550
SyntaxV2.Cmd21.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd21.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd21.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd21.Visible = false
SyntaxV2.Cmd21.Font = Enum.Font.Nunito
SyntaxV2.Cmd21.Text = "x"
SyntaxV2.Cmd21.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd21.TextSize = 14.000
SyntaxV2.Cmd21.TextStrokeTransparency = 0.000

SyntaxV2.Cmd22.Name = "Cmd22"
SyntaxV2.Cmd22.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd22.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd22.BackgroundTransparency = 0.550
SyntaxV2.Cmd22.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd22.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd22.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd22.Visible = false
SyntaxV2.Cmd22.Font = Enum.Font.Nunito
SyntaxV2.Cmd22.Text = "x"
SyntaxV2.Cmd22.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd22.TextSize = 14.000
SyntaxV2.Cmd22.TextStrokeTransparency = 0.000

SyntaxV2.Cmd23.Name = "Cmd23"
SyntaxV2.Cmd23.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd23.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd23.BackgroundTransparency = 0.550
SyntaxV2.Cmd23.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd23.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd23.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd23.Visible = false
SyntaxV2.Cmd23.Font = Enum.Font.Nunito
SyntaxV2.Cmd23.Text = "x"
SyntaxV2.Cmd23.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd23.TextSize = 14.000
SyntaxV2.Cmd23.TextStrokeTransparency = 0.000

SyntaxV2.Cmd24.Name = "Cmd24"
SyntaxV2.Cmd24.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd24.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd24.BackgroundTransparency = 0.550
SyntaxV2.Cmd24.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd24.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd24.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd24.Visible = false
SyntaxV2.Cmd24.Font = Enum.Font.Nunito
SyntaxV2.Cmd24.Text = "x"
SyntaxV2.Cmd24.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd24.TextSize = 14.000
SyntaxV2.Cmd24.TextStrokeTransparency = 0.000

SyntaxV2.Cmd25.Name = "Cmd25"
SyntaxV2.Cmd25.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd25.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd25.BackgroundTransparency = 0.550
SyntaxV2.Cmd25.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd25.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd25.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd25.Visible = false
SyntaxV2.Cmd25.Font = Enum.Font.Nunito
SyntaxV2.Cmd25.Text = "x"
SyntaxV2.Cmd25.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd25.TextSize = 14.000
SyntaxV2.Cmd25.TextStrokeTransparency = 0.000

SyntaxV2.Cmd26.Name = "Cmd26"
SyntaxV2.Cmd26.Parent = SyntaxV2.ScrollingFrame
SyntaxV2.Cmd26.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Cmd26.BackgroundTransparency = 0.550
SyntaxV2.Cmd26.BorderColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd26.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Cmd26.Size = UDim2.new(0, 221, 0, 21)
SyntaxV2.Cmd26.Visible = false
SyntaxV2.Cmd26.Font = Enum.Font.Nunito
SyntaxV2.Cmd26.Text = "x"
SyntaxV2.Cmd26.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Cmd26.TextSize = 14.000
SyntaxV2.Cmd26.TextStrokeTransparency = 0.000

SyntaxV2.UICorner_25.Parent = SyntaxV2.Main2

SyntaxV2.HatScripts.Name = "HatScripts"
SyntaxV2.HatScripts.Parent = SyntaxV2.Main2
SyntaxV2.HatScripts.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.HatScripts.BackgroundTransparency = 1.000
SyntaxV2.HatScripts.Position = UDim2.new(0.0118343197, 0, 0.201005027, 0)
SyntaxV2.HatScripts.Size = UDim2.new(0, 100, 0, 100)
SyntaxV2.HatScripts.Visible = false

SyntaxV2.Frame_5.Parent = SyntaxV2.HatScripts
SyntaxV2.Frame_5.BackgroundColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.Frame_5.BackgroundTransparency = 1.000
SyntaxV2.Frame_5.Position = UDim2.new(-0.0599999987, 0, 0.175142512, 0)
SyntaxV2.Frame_5.Size = UDim2.new(0, 511, 0, 141)

SyntaxV2.UICorner_26.Parent = SyntaxV2.Frame_5

SyntaxV2.ScrollingFrame_2.Parent = SyntaxV2.Frame_5
SyntaxV2.ScrollingFrame_2.Active = true
SyntaxV2.ScrollingFrame_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.ScrollingFrame_2.BackgroundTransparency = 1.000
SyntaxV2.ScrollingFrame_2.BorderColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.ScrollingFrame_2.Position = UDim2.new(0.00775194261, 0, 0.141843975, 0)
SyntaxV2.ScrollingFrame_2.Size = UDim2.new(0, 503, 0, 120)
SyntaxV2.ScrollingFrame_2.CanvasSize = UDim2.new(0, 0, 5, 0)
SyntaxV2.ScrollingFrame_2.VerticalScrollBarInset = Enum.ScrollBarInset.Always

SyntaxV2.Hat1.Name = "Hat1"
SyntaxV2.Hat1.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat1.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat1.BackgroundTransparency = 0.250
SyntaxV2.Hat1.Position = UDim2.new(-0.0514999479, 0, 0, 0)
SyntaxV2.Hat1.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat1.Font = Enum.Font.Nunito
SyntaxV2.Hat1.Text = "Wings [ FREE HATS ]"
SyntaxV2.Hat1.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat1.TextSize = 14.000
SyntaxV2.Hat1.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Hat1.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Hat1.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Wings ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571566859")[1].Source)()

end)

SyntaxV2.UICorner_27.Parent = SyntaxV2.Hat1

SyntaxV2.UIListLayout_2.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.UIListLayout_2.HorizontalAlignment = Enum.HorizontalAlignment.Center
SyntaxV2.UIListLayout_2.SortOrder = Enum.SortOrder.LayoutOrder
SyntaxV2.UIListLayout_2.Padding = UDim.new(0, 7)

SyntaxV2.Hat2.Name = "Hat2"
SyntaxV2.Hat2.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat2.BackgroundTransparency = 0.250
SyntaxV2.Hat2.Position = UDim2.new(-0.0514999479, 0, 0.187919468, 0)
SyntaxV2.Hat2.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat2.Font = Enum.Font.Nunito
SyntaxV2.Hat2.Text = "Knife [FLING]"
SyntaxV2.Hat2.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat2.TextSize = 14.000
SyntaxV2.Hat2.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Hat2.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Hat2.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Knife ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7572066757")[1].Source)()

end)

SyntaxV2.UICorner_28.Parent = SyntaxV2.Hat2

SyntaxV2.Hat3.Name = "Hat3"
SyntaxV2.Hat3.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat3.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat3.BackgroundTransparency = 0.250
SyntaxV2.Hat3.Position = UDim2.new(-0.0514999479, 0, 0.375838935, 0)
SyntaxV2.Hat3.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat3.Font = Enum.Font.Nunito
SyntaxV2.Hat3.Text = "Shotgun V2 [ FLING ]"
SyntaxV2.Hat3.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat3.TextSize = 14.000
SyntaxV2.Hat3.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Hat3.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Hat3.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Shotgun V2 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7572112051")[1].Source)()

end)

SyntaxV2.UICorner_29.Parent = SyntaxV2.Hat3

SyntaxV2.Hat4.Name = "Hat4"
SyntaxV2.Hat4.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat4.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat4.BackgroundTransparency = 0.250
SyntaxV2.Hat4.Position = UDim2.new(-0.0514999479, 0, 0.563758373, 0)
SyntaxV2.Hat4.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat4.Font = Enum.Font.Nunito
SyntaxV2.Hat4.Text = "Dual Pink Guns [ FLING ]"
SyntaxV2.Hat4.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat4.TextSize = 14.000
SyntaxV2.Hat4.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Hat4.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Hat4.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Dual Pink Guns ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7572156021")[1].Source)()

end)

SyntaxV2.UICorner_30.Parent = SyntaxV2.Hat4

SyntaxV2.Hat5.Name = "Hat5"
SyntaxV2.Hat5.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat5.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat5.BackgroundTransparency = 0.250
SyntaxV2.Hat5.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat5.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat5.Visible = true
SyntaxV2.Hat5.Font = Enum.Font.Nunito
SyntaxV2.Hat5.Text = "Brawler [ FLING ]"
SyntaxV2.Hat5.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat5.TextSize = 14.000
SyntaxV2.Hat5.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Hat5.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Hat5.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Brawler ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7572220770")[1].Source)()

end)

SyntaxV2.UICorner_31.Parent = SyntaxV2.Hat5

SyntaxV2.Hat6.Name = "Hat6"
SyntaxV2.Hat6.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat6.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat6.BackgroundTransparency = 0.250
SyntaxV2.Hat6.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat6.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat6.Visible = true
SyntaxV2.Hat6.Font = Enum.Font.Nunito
SyntaxV2.Hat6.Text = "Spider Bot [ FLING ]"
SyntaxV2.Hat6.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat6.TextSize = 14.000
SyntaxV2.Hat6.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Hat6.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Hat6.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Spider Bot ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7572330871")[1].Source)()

end)

SyntaxV2.UICorner_32.Parent = SyntaxV2.Hat6

SyntaxV2.Hat7.Name = "Hat7"
SyntaxV2.Hat7.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat7.BackgroundColor3 = Color3.fromRGB(170, 0, 0)
SyntaxV2.Hat7.BackgroundTransparency = 0.250
SyntaxV2.Hat7.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat7.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat7.Visible = true
SyntaxV2.Hat7.Font = Enum.Font.Nunito
SyntaxV2.Hat7.Text = "SCP FIXED [ SOON ]"
SyntaxV2.Hat7.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat7.TextSize = 14.000
SyntaxV2.Hat7.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Hat7.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Hat7.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Not working for now ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

--loadstring(game:GetObjects("rbxassetid://7572330871")[1].Source)()

end)

SyntaxV2.UICorner_33.Parent = SyntaxV2.Hat7

SyntaxV2.Hat8.Name = "Hat8"
SyntaxV2.Hat8.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat8.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat8.BackgroundTransparency = 0.250
SyntaxV2.Hat8.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat8.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat8.Visible = false
SyntaxV2.Hat8.Font = Enum.Font.Nunito
SyntaxV2.Hat8.Text = "x"
SyntaxV2.Hat8.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat8.TextSize = 14.000

SyntaxV2.UICorner_34.Parent = SyntaxV2.Hat8

SyntaxV2.Hat9.Name = "Hat9"
SyntaxV2.Hat9.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat9.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat9.BackgroundTransparency = 0.250
SyntaxV2.Hat9.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat9.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat9.Visible = false
SyntaxV2.Hat9.Font = Enum.Font.Nunito
SyntaxV2.Hat9.Text = "x"
SyntaxV2.Hat9.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat9.TextSize = 14.000

SyntaxV2.UICorner_35.Parent = SyntaxV2.Hat9

SyntaxV2.Hat10.Name = "Hat10"
SyntaxV2.Hat10.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat10.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat10.BackgroundTransparency = 0.250
SyntaxV2.Hat10.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat10.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat10.Visible = false
SyntaxV2.Hat10.Font = Enum.Font.Nunito
SyntaxV2.Hat10.Text = "x"
SyntaxV2.Hat10.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat10.TextSize = 14.000

SyntaxV2.UICorner_36.Parent = SyntaxV2.Hat10

SyntaxV2.Hat11.Name = "Hat11"
SyntaxV2.Hat11.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat11.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat11.BackgroundTransparency = 0.250
SyntaxV2.Hat11.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat11.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat11.Visible = false
SyntaxV2.Hat11.Font = Enum.Font.Nunito
SyntaxV2.Hat11.Text = "x"
SyntaxV2.Hat11.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat11.TextSize = 14.000

SyntaxV2.UICorner_37.Parent = SyntaxV2.Hat11

SyntaxV2.Hat12.Name = "Hat12"
SyntaxV2.Hat12.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat12.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat12.BackgroundTransparency = 0.250
SyntaxV2.Hat12.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat12.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat12.Visible = false
SyntaxV2.Hat12.Font = Enum.Font.Nunito
SyntaxV2.Hat12.Text = "x"
SyntaxV2.Hat12.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat12.TextSize = 14.000

SyntaxV2.UICorner_38.Parent = SyntaxV2.Hat12

SyntaxV2.Hat13.Name = "Hat13"
SyntaxV2.Hat13.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat13.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat13.BackgroundTransparency = 0.250
SyntaxV2.Hat13.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat13.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat13.Visible = false
SyntaxV2.Hat13.Font = Enum.Font.Nunito
SyntaxV2.Hat13.Text = "x"
SyntaxV2.Hat13.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat13.TextSize = 14.000

SyntaxV2.UICorner_39.Parent = SyntaxV2.Hat13

SyntaxV2.Hat14.Name = "Hat14"
SyntaxV2.Hat14.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat14.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat14.BackgroundTransparency = 0.250
SyntaxV2.Hat14.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat14.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat14.Visible = false
SyntaxV2.Hat14.Font = Enum.Font.Nunito
SyntaxV2.Hat14.Text = "x"
SyntaxV2.Hat14.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat14.TextSize = 14.000

SyntaxV2.UICorner_40.Parent = SyntaxV2.Hat14

SyntaxV2.Hat15.Name = "Hat15"
SyntaxV2.Hat15.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat15.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat15.BackgroundTransparency = 0.250
SyntaxV2.Hat15.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat15.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat15.Visible = false
SyntaxV2.Hat15.Font = Enum.Font.Nunito
SyntaxV2.Hat15.Text = "x"
SyntaxV2.Hat15.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat15.TextSize = 14.000

SyntaxV2.UICorner_41.Parent = SyntaxV2.Hat15

SyntaxV2.Hat16.Name = "Hat16"
SyntaxV2.Hat16.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat16.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat16.BackgroundTransparency = 0.250
SyntaxV2.Hat16.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat16.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat16.Visible = false
SyntaxV2.Hat16.Font = Enum.Font.Nunito
SyntaxV2.Hat16.Text = "x"
SyntaxV2.Hat16.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat16.TextSize = 14.000

SyntaxV2.UICorner_42.Parent = SyntaxV2.Hat16

SyntaxV2.Hat17.Name = "Hat17"
SyntaxV2.Hat17.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat17.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat17.BackgroundTransparency = 0.250
SyntaxV2.Hat17.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat17.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat17.Visible = false
SyntaxV2.Hat17.Font = Enum.Font.Nunito
SyntaxV2.Hat17.Text = "x"
SyntaxV2.Hat17.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat17.TextSize = 14.000

SyntaxV2.UICorner_43.Parent = SyntaxV2.Hat17

SyntaxV2.Hat18.Name = "Hat18"
SyntaxV2.Hat18.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat18.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat18.BackgroundTransparency = 0.250
SyntaxV2.Hat18.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat18.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat18.Visible = false
SyntaxV2.Hat18.Font = Enum.Font.Nunito
SyntaxV2.Hat18.Text = "x"
SyntaxV2.Hat18.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat18.TextSize = 14.000

SyntaxV2.UICorner_44.Parent = SyntaxV2.Hat18

SyntaxV2.Hat19.Name = "Hat19"
SyntaxV2.Hat19.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat19.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat19.BackgroundTransparency = 0.250
SyntaxV2.Hat19.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat19.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat19.Visible = false
SyntaxV2.Hat19.Font = Enum.Font.Nunito
SyntaxV2.Hat19.Text = "x"
SyntaxV2.Hat19.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat19.TextSize = 14.000

SyntaxV2.UICorner_45.Parent = SyntaxV2.Hat19

SyntaxV2.Hat20.Name = "Hat20"
SyntaxV2.Hat20.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat20.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat20.BackgroundTransparency = 0.250
SyntaxV2.Hat20.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat20.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat20.Visible = false
SyntaxV2.Hat20.Font = Enum.Font.Nunito
SyntaxV2.Hat20.Text = "x"
SyntaxV2.Hat20.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat20.TextSize = 14.000

SyntaxV2.UICorner_46.Parent = SyntaxV2.Hat20

SyntaxV2.Hat21.Name = "Hat21"
SyntaxV2.Hat21.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat21.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat21.BackgroundTransparency = 0.250
SyntaxV2.Hat21.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat21.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat21.Visible = false
SyntaxV2.Hat21.Font = Enum.Font.Nunito
SyntaxV2.Hat21.Text = "x"
SyntaxV2.Hat21.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat21.TextSize = 14.000

SyntaxV2.UICorner_47.Parent = SyntaxV2.Hat21

SyntaxV2.Hat22.Name = "Hat22"
SyntaxV2.Hat22.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat22.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat22.BackgroundTransparency = 0.250
SyntaxV2.Hat22.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat22.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat22.Visible = false
SyntaxV2.Hat22.Font = Enum.Font.Nunito
SyntaxV2.Hat22.Text = "x"
SyntaxV2.Hat22.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat22.TextSize = 14.000

SyntaxV2.UICorner_48.Parent = SyntaxV2.Hat22

SyntaxV2.Hat23.Name = "Hat23"
SyntaxV2.Hat23.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat23.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat23.BackgroundTransparency = 0.250
SyntaxV2.Hat23.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat23.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat23.Visible = false
SyntaxV2.Hat23.Font = Enum.Font.Nunito
SyntaxV2.Hat23.Text = "x"
SyntaxV2.Hat23.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat23.TextSize = 14.000

SyntaxV2.UICorner_49.Parent = SyntaxV2.Hat23

SyntaxV2.Hat24.Name = "Hat24"
SyntaxV2.Hat24.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat24.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat24.BackgroundTransparency = 0.250
SyntaxV2.Hat24.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat24.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat24.Visible = false
SyntaxV2.Hat24.Font = Enum.Font.Nunito
SyntaxV2.Hat24.Text = "x"
SyntaxV2.Hat24.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat24.TextSize = 14.000

SyntaxV2.UICorner_50.Parent = SyntaxV2.Hat24

SyntaxV2.Hat25.Name = "Hat25"
SyntaxV2.Hat25.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat25.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat25.BackgroundTransparency = 0.250
SyntaxV2.Hat25.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat25.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat25.Visible = false
SyntaxV2.Hat25.Font = Enum.Font.Nunito
SyntaxV2.Hat25.Text = "x"
SyntaxV2.Hat25.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat25.TextSize = 14.000

SyntaxV2.UICorner_51.Parent = SyntaxV2.Hat25

SyntaxV2.Hat26.Name = "Hat26"
SyntaxV2.Hat26.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat26.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat26.BackgroundTransparency = 0.250
SyntaxV2.Hat26.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat26.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat26.Visible = false
SyntaxV2.Hat26.Font = Enum.Font.Nunito
SyntaxV2.Hat26.Text = "x"
SyntaxV2.Hat26.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat26.TextSize = 14.000

SyntaxV2.UICorner_52.Parent = SyntaxV2.Hat26

SyntaxV2.Hat27.Name = "Hat27"
SyntaxV2.Hat27.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat27.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat27.BackgroundTransparency = 0.250
SyntaxV2.Hat27.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat27.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat27.Visible = false
SyntaxV2.Hat27.Font = Enum.Font.Nunito
SyntaxV2.Hat27.Text = "x"
SyntaxV2.Hat27.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat27.TextSize = 14.000

SyntaxV2.UICorner_53.Parent = SyntaxV2.Hat27

SyntaxV2.Hat28.Name = "Hat28"
SyntaxV2.Hat28.Parent = SyntaxV2.ScrollingFrame_2
SyntaxV2.Hat28.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Hat28.BackgroundTransparency = 0.250
SyntaxV2.Hat28.Position = UDim2.new(-0.284023672, 0, 0, 0)
SyntaxV2.Hat28.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Hat28.Visible = false
SyntaxV2.Hat28.Font = Enum.Font.Nunito
SyntaxV2.Hat28.Text = "x"
SyntaxV2.Hat28.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Hat28.TextSize = 14.000

SyntaxV2.UICorner_54.Parent = SyntaxV2.Hat28

SyntaxV2.UIGradient_18.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(0, 0, 0)), ColorSequenceKeypoint.new(0.50, Color3.fromRGB(89, 0, 134)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(0, 0, 0))}
SyntaxV2.UIGradient_18.Rotation = 45
SyntaxV2.UIGradient_18.Parent = SyntaxV2.Frame_5

SyntaxV2.ColorMenu1.Name = "ColorMenu1"
SyntaxV2.ColorMenu1.Parent = SyntaxV2.HatScripts
SyntaxV2.ColorMenu1.BackgroundColor3 = Color3.fromRGB(59, 0, 89)
SyntaxV2.ColorMenu1.BackgroundTransparency = 0.050
SyntaxV2.ColorMenu1.Position = UDim2.new(0.703139663, 0, -0.274857491, 0)
SyntaxV2.ColorMenu1.Size = UDim2.new(0, 344, 0, 44)

SyntaxV2.UICorner_55.Parent = SyntaxV2.ColorMenu1

SyntaxV2.ColorMenu1_2.Name = "ColorMenu1"
SyntaxV2.ColorMenu1_2.Parent = SyntaxV2.ColorMenu1
SyntaxV2.ColorMenu1_2.BackgroundColor3 = Color3.fromRGB(121, 0, 182)
SyntaxV2.ColorMenu1_2.BackgroundTransparency = 0.450
SyntaxV2.ColorMenu1_2.Position = UDim2.new(0.0712972805, 0, 0.216909245, 0)
SyntaxV2.ColorMenu1_2.Size = UDim2.new(0, 301, 0, 24)

SyntaxV2.UICorner_56.Parent = SyntaxV2.ColorMenu1_2

SyntaxV2.UIGradient_19.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(43, 0, 65)), ColorSequenceKeypoint.new(0.03, Color3.fromRGB(169, 0, 254)), ColorSequenceKeypoint.new(0.73, Color3.fromRGB(170, 0, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(170, 0, 255))}
SyntaxV2.UIGradient_19.Rotation = 45
SyntaxV2.UIGradient_19.Parent = SyntaxV2.ColorMenu1

SyntaxV2.TextLabel_4.Parent = SyntaxV2.HatScripts
SyntaxV2.TextLabel_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel_4.BackgroundTransparency = 1.000
SyntaxV2.TextLabel_4.Position = UDim2.new(0.970000029, 0, -0.156666875, 0)
SyntaxV2.TextLabel_4.Size = UDim2.new(0, 301, 0, 20)
SyntaxV2.TextLabel_4.Font = Enum.Font.TitilliumWeb
SyntaxV2.TextLabel_4.Text = "Hats, Fling Scripts"
SyntaxV2.TextLabel_4.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel_4.TextSize = 24.000
SyntaxV2.TextLabel_4.TextWrapped = true

SyntaxV2.xd4_2.Name = "xd4"
SyntaxV2.xd4_2.Parent = SyntaxV2.HatScripts
SyntaxV2.xd4_2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.xd4_2.BackgroundTransparency = 0.350
SyntaxV2.xd4_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.xd4_2.Position = UDim2.new(-0.0599999987, 0, 0.275501728, 0)
SyntaxV2.xd4_2.Size = UDim2.new(0, 507, 0, 2)

SyntaxV2.UICorner_57.Parent = SyntaxV2.xd4_2

SyntaxV2.AnimationsScripts.Name = "AnimationsScripts"
SyntaxV2.AnimationsScripts.Parent = SyntaxV2.Main2
SyntaxV2.AnimationsScripts.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.AnimationsScripts.BackgroundTransparency = 1.000
SyntaxV2.AnimationsScripts.Position = UDim2.new(0.0118343197, 0, 0.201005027, 0)
SyntaxV2.AnimationsScripts.Size = UDim2.new(0, 100, 0, 100)
SyntaxV2.AnimationsScripts.Visible = false

SyntaxV2.Frame_6.Parent = SyntaxV2.AnimationsScripts
SyntaxV2.Frame_6.BackgroundColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.Frame_6.BackgroundTransparency = 1.000
SyntaxV2.Frame_6.Position = UDim2.new(-0.0599999987, 0, 0.175142512, 0)
SyntaxV2.Frame_6.Size = UDim2.new(0, 511, 0, 141)

SyntaxV2.UICorner_58.Parent = SyntaxV2.Frame_6

SyntaxV2.ScrollingFrame_3.Parent = SyntaxV2.Frame_6
SyntaxV2.ScrollingFrame_3.Active = true
SyntaxV2.ScrollingFrame_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.ScrollingFrame_3.BackgroundTransparency = 1.000
SyntaxV2.ScrollingFrame_3.BorderColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.ScrollingFrame_3.Position = UDim2.new(0.00775194261, 0, 0.141843975, 0)
SyntaxV2.ScrollingFrame_3.Size = UDim2.new(0, 503, 0, 120)
SyntaxV2.ScrollingFrame_3.CanvasSize = UDim2.new(0, 0, 5, 0)
SyntaxV2.ScrollingFrame_3.VerticalScrollBarInset = Enum.ScrollBarInset.Always

SyntaxV2.UIListLayout_3.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.UIListLayout_3.HorizontalAlignment = Enum.HorizontalAlignment.Center
SyntaxV2.UIListLayout_3.SortOrder = Enum.SortOrder.LayoutOrder
SyntaxV2.UIListLayout_3.Padding = UDim.new(0, 7)

SyntaxV2.Anim1.Name = "Anim1"
SyntaxV2.Anim1.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim1.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Anim1.BackgroundTransparency = 0.250
SyntaxV2.Anim1.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim1.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim1.Font = Enum.Font.Nunito
SyntaxV2.Anim1.Text = "Ninja"
SyntaxV2.Anim1.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim1.TextSize = 14.000
SyntaxV2.Anim1.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim1.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim1.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ NINJA ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571249114")[1].Source)()

end)

SyntaxV2.UICorner_59.Parent = SyntaxV2.Anim1

SyntaxV2.Anim10.Name = "Anim10"
SyntaxV2.Anim10.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim10.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim10.BackgroundTransparency = 0.250
SyntaxV2.Anim10.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim10.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim10.Font = Enum.Font.Nunito
SyntaxV2.Anim10.Text = "Fancy Feet Dance [R15]"
SyntaxV2.Anim10.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim10.TextSize = 14.000
SyntaxV2.Anim10.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim10.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim10.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Fancy Feet R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571405391")[1].Source)()
end)

SyntaxV2.UICorner_60.Parent = SyntaxV2.Anim10

SyntaxV2.Anim11.Name = "Anim11"
SyntaxV2.Anim11.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim11.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim11.BackgroundTransparency = 0.250
SyntaxV2.Anim11.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim11.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim11.Font = Enum.Font.Nunito
SyntaxV2.Anim11.Text = "Electro Swing Dance [R15]"
SyntaxV2.Anim11.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim11.TextSize = 14.000
SyntaxV2.Anim11.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim11.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim11.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Electro Swing R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571412130")[1].Source)()
end)

SyntaxV2.UICorner_61.Parent = SyntaxV2.Anim11

SyntaxV2.Anim12.Name = "Anim12"
SyntaxV2.Anim12.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim12.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim12.BackgroundTransparency = 0.250
SyntaxV2.Anim12.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim12.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim12.Font = Enum.Font.Nunito
SyntaxV2.Anim12.Text = "Default Dance [R15]"
SyntaxV2.Anim12.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim12.TextSize = 14.000
SyntaxV2.Anim12.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim12.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim12.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Default Dance R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571444357")[1].Source)()
end)

SyntaxV2.UICorner_62.Parent = SyntaxV2.Anim12

SyntaxV2.Anim13.Name = "Anim13"
SyntaxV2.Anim13.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim13.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim13.BackgroundTransparency = 0.250
SyntaxV2.Anim13.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim13.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim13.Visible = true
SyntaxV2.Anim13.Font = Enum.Font.Nunito
SyntaxV2.Anim13.Text = "Cool dance [R15]"
SyntaxV2.Anim13.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim13.TextSize = 14.000
SyntaxV2.Anim13.TextWrapped = true
SyntaxV2.Anim13.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim13.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim13.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Cool dance R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571434396")[1].Source)()
end)

SyntaxV2.UICorner_63.Parent = SyntaxV2.Anim13

SyntaxV2.Anim14.Name = "Anim14"
SyntaxV2.Anim14.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim14.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim14.BackgroundTransparency = 0.250
SyntaxV2.Anim14.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim14.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim14.Visible = true
SyntaxV2.Anim14.Font = Enum.Font.Nunito
SyntaxV2.Anim14.Text = "Whip Dance"
SyntaxV2.Anim14.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim14.TextSize = 14.000
SyntaxV2.Anim14.TextWrapped = true
SyntaxV2.Anim14.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim14.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim14.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Whip Dance R6 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571867060")[1].Source)()
end)

SyntaxV2.UICorner_64.Parent = SyntaxV2.Anim14

SyntaxV2.Anim15.Name = "Anim15"
SyntaxV2.Anim15.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim15.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim15.BackgroundTransparency = 0.250
SyntaxV2.Anim15.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim15.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim15.Visible = true
SyntaxV2.Anim15.Font = Enum.Font.Nunito
SyntaxV2.Anim15.Text = "Kitty Dance"
SyntaxV2.Anim15.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim15.TextSize = 14.000
SyntaxV2.Anim15.TextWrapped = true
SyntaxV2.Anim15.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim15.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim15.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Kitty dance R6 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571826421")[1].Source)()
end)


SyntaxV2.UICorner_65.Parent = SyntaxV2.Anim15

SyntaxV2.Anim16.Name = "Anim16"
SyntaxV2.Anim16.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim16.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim16.BackgroundTransparency = 0.250
SyntaxV2.Anim16.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim16.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim16.Visible = true
SyntaxV2.Anim16.Font = Enum.Font.Nunito
SyntaxV2.Anim16.Text = "Ok dance"
SyntaxV2.Anim16.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim16.TextSize = 14.000
SyntaxV2.Anim16.TextWrapped = true
SyntaxV2.Anim16.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim16.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim16.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Ok dance R6 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571910129")[1].Source)()
end)


SyntaxV2.UICorner_66.Parent = SyntaxV2.Anim16

SyntaxV2.Anim17.Name = "Anim17"
SyntaxV2.Anim17.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim17.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim17.BackgroundTransparency = 0.250
SyntaxV2.Anim17.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim17.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim17.Visible = false
SyntaxV2.Anim17.Font = Enum.Font.Nunito
SyntaxV2.Anim17.Text = "x"
SyntaxV2.Anim17.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim17.TextSize = 14.000
SyntaxV2.Anim17.TextWrapped = true

SyntaxV2.UICorner_67.Parent = SyntaxV2.Anim17

SyntaxV2.Anim18.Name = "Anim18"
SyntaxV2.Anim18.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim18.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim18.BackgroundTransparency = 0.250
SyntaxV2.Anim18.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim18.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim18.Visible = false
SyntaxV2.Anim18.Font = Enum.Font.Nunito
SyntaxV2.Anim18.Text = "x"
SyntaxV2.Anim18.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim18.TextSize = 14.000
SyntaxV2.Anim18.TextWrapped = true

SyntaxV2.UICorner_68.Parent = SyntaxV2.Anim18

SyntaxV2.Anim19.Name = "Anim19"
SyntaxV2.Anim19.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim19.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim19.BackgroundTransparency = 0.250
SyntaxV2.Anim19.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim19.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim19.Visible = false
SyntaxV2.Anim19.Font = Enum.Font.Nunito
SyntaxV2.Anim19.Text = "x"
SyntaxV2.Anim19.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim19.TextSize = 14.000
SyntaxV2.Anim19.TextWrapped = true

SyntaxV2.UICorner_69.Parent = SyntaxV2.Anim19

SyntaxV2.Anim2.Name = "Anim2"
SyntaxV2.Anim2.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Anim2.BackgroundTransparency = 0.250
SyntaxV2.Anim2.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim2.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim2.Font = Enum.Font.Nunito
SyntaxV2.Anim2.Text = "Sexy Dance [R15]"
SyntaxV2.Anim2.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim2.TextSize = 14.000
SyntaxV2.Anim2.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim2.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim2.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Sexy Dance R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571271531")[1].Source)()
end)

SyntaxV2.UICorner_70.Parent = SyntaxV2.Anim2

SyntaxV2.Anim20.Name = "Anim20"
SyntaxV2.Anim20.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim20.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim20.BackgroundTransparency = 0.250
SyntaxV2.Anim20.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim20.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim20.Visible = false
SyntaxV2.Anim20.Font = Enum.Font.Nunito
SyntaxV2.Anim20.Text = "x"
SyntaxV2.Anim20.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim20.TextSize = 14.000
SyntaxV2.Anim20.TextWrapped = true

SyntaxV2.UICorner_71.Parent = SyntaxV2.Anim20

SyntaxV2.Anim21.Name = "Anim21"
SyntaxV2.Anim21.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim21.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim21.BackgroundTransparency = 0.250
SyntaxV2.Anim21.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim21.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim21.Visible = false
SyntaxV2.Anim21.Font = Enum.Font.Nunito
SyntaxV2.Anim21.Text = "x"
SyntaxV2.Anim21.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim21.TextSize = 14.000
SyntaxV2.Anim21.TextWrapped = true

SyntaxV2.UICorner_72.Parent = SyntaxV2.Anim21

SyntaxV2.Anim22.Name = "Anim22"
SyntaxV2.Anim22.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim22.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim22.BackgroundTransparency = 0.250
SyntaxV2.Anim22.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim22.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim22.Visible = false
SyntaxV2.Anim22.Font = Enum.Font.Nunito
SyntaxV2.Anim22.Text = "x"
SyntaxV2.Anim22.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim22.TextSize = 14.000
SyntaxV2.Anim22.TextWrapped = true

SyntaxV2.UICorner_73.Parent = SyntaxV2.Anim22

SyntaxV2.Anim23.Name = "Anim23"
SyntaxV2.Anim23.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim23.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim23.BackgroundTransparency = 0.250
SyntaxV2.Anim23.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim23.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim23.Visible = false
SyntaxV2.Anim23.Font = Enum.Font.Nunito
SyntaxV2.Anim23.Text = "x"
SyntaxV2.Anim23.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim23.TextSize = 14.000
SyntaxV2.Anim23.TextWrapped = true

SyntaxV2.UICorner_74.Parent = SyntaxV2.Anim23

SyntaxV2.Anim24.Name = "Anim24"
SyntaxV2.Anim24.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim24.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim24.BackgroundTransparency = 0.250
SyntaxV2.Anim24.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim24.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim24.Visible = false
SyntaxV2.Anim24.Font = Enum.Font.Nunito
SyntaxV2.Anim24.Text = "x"
SyntaxV2.Anim24.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim24.TextSize = 14.000
SyntaxV2.Anim24.TextWrapped = true

SyntaxV2.UICorner_75.Parent = SyntaxV2.Anim24

SyntaxV2.Anim25.Name = "Anim25"
SyntaxV2.Anim25.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim25.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim25.BackgroundTransparency = 0.250
SyntaxV2.Anim25.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim25.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim25.Visible = false
SyntaxV2.Anim25.Font = Enum.Font.Nunito
SyntaxV2.Anim25.Text = "x"
SyntaxV2.Anim25.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim25.TextSize = 14.000
SyntaxV2.Anim25.TextWrapped = true

SyntaxV2.UICorner_76.Parent = SyntaxV2.Anim25

SyntaxV2.Anim26.Name = "Anim26"
SyntaxV2.Anim26.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim26.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim26.BackgroundTransparency = 0.250
SyntaxV2.Anim26.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim26.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim26.Visible = false
SyntaxV2.Anim26.Font = Enum.Font.Nunito
SyntaxV2.Anim26.Text = "x"
SyntaxV2.Anim26.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim26.TextSize = 14.000
SyntaxV2.Anim26.TextWrapped = true

SyntaxV2.UICorner_77.Parent = SyntaxV2.Anim26

SyntaxV2.Anim27.Name = "Anim27"
SyntaxV2.Anim27.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim27.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim27.BackgroundTransparency = 0.250
SyntaxV2.Anim27.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim27.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim27.Visible = false
SyntaxV2.Anim27.Font = Enum.Font.Nunito
SyntaxV2.Anim27.Text = "x"
SyntaxV2.Anim27.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim27.TextSize = 14.000
SyntaxV2.Anim27.TextWrapped = true

SyntaxV2.UICorner_78.Parent = SyntaxV2.Anim27

SyntaxV2.Anim28.Name = "Anim28"
SyntaxV2.Anim28.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim28.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim28.BackgroundTransparency = 0.250
SyntaxV2.Anim28.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim28.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim28.Visible = false
SyntaxV2.Anim28.Font = Enum.Font.Nunito
SyntaxV2.Anim28.Text = "x"
SyntaxV2.Anim28.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim28.TextSize = 14.000
SyntaxV2.Anim28.TextWrapped = true

SyntaxV2.UICorner_79.Parent = SyntaxV2.Anim28

SyntaxV2.Anim3.Name = "Anim3"
SyntaxV2.Anim3.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim3.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Anim3.BackgroundTransparency = 0.250
SyntaxV2.Anim3.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim3.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim3.Font = Enum.Font.Nunito
SyntaxV2.Anim3.Text = "Twerk [R15]"
SyntaxV2.Anim3.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim3.TextSize = 14.000
SyntaxV2.Anim3.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim3.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim3.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Twerk R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571284708")[1].Source)()
end)

SyntaxV2.UICorner_80.Parent = SyntaxV2.Anim3

SyntaxV2.Anim4.Name = "Anim4"
SyntaxV2.Anim4.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim4.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Anim4.BackgroundTransparency = 0.250
SyntaxV2.Anim4.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim4.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim4.Font = Enum.Font.Nunito
SyntaxV2.Anim4.Text = "Hug Sex [R15]"
SyntaxV2.Anim4.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim4.TextSize = 14.000
SyntaxV2.Anim4.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim4.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim4.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Hug Sex R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."
--7571306367
loadstring(game:GetObjects("rbxassetid://7571306367")[1].Source)()
end)

SyntaxV2.UICorner_81.Parent = SyntaxV2.Anim4

SyntaxV2.Anim5.Name = "Anim5"
SyntaxV2.Anim5.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim5.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Anim5.BackgroundTransparency = 0.250
SyntaxV2.Anim5.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim5.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim5.Font = Enum.Font.Nunito
SyntaxV2.Anim5.Text = "Fresh Dance [R15]"
SyntaxV2.Anim5.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim5.TextSize = 14.000
SyntaxV2.Anim5.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim5.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim5.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Fresh Dance R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571293825")[1].Source)()
end)

SyntaxV2.UICorner_82.Parent = SyntaxV2.Anim5

SyntaxV2.Anim6.Name = "Anim6"
SyntaxV2.Anim6.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim6.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim6.BackgroundTransparency = 0.250
SyntaxV2.Anim6.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim6.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim6.Font = Enum.Font.Nunito
SyntaxV2.Anim6.Text = "Reanimated Dance [R15]"
SyntaxV2.Anim6.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim6.TextSize = 14.000
SyntaxV2.Anim6.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim6.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim6.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Reanimated Dance R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571319382")[1].Source)()
end)

SyntaxV2.UICorner_83.Parent = SyntaxV2.Anim6

SyntaxV2.Anim7.Name = "Anim7"
SyntaxV2.Anim7.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim7.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim7.BackgroundTransparency = 0.250
SyntaxV2.Anim7.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim7.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim7.Font = Enum.Font.Nunito
SyntaxV2.Anim7.Text = "Take The L Dance [R15]"
SyntaxV2.Anim7.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim7.TextSize = 14.000
SyntaxV2.Anim7.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim7.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim7.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Take The L Dance R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571337660")[1].Source)()
end)

SyntaxV2.UICorner_84.Parent = SyntaxV2.Anim7

SyntaxV2.Anim8.Name = "Anim8"
SyntaxV2.Anim8.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim8.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim8.BackgroundTransparency = 0.250
SyntaxV2.Anim8.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim8.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim8.Font = Enum.Font.Nunito
SyntaxV2.Anim8.Text = "The Robot Dance [R15]"
SyntaxV2.Anim8.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim8.TextSize = 14.000
SyntaxV2.Anim8.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim8.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim8.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ The Robot R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571378592")[1].Source)()
end)

SyntaxV2.UICorner_85.Parent = SyntaxV2.Anim8

SyntaxV2.Anim9.Name = "Anim9"
SyntaxV2.Anim9.Parent = SyntaxV2.ScrollingFrame_3
SyntaxV2.Anim9.BackgroundColor3 = Color3.fromRGB(9, 9, 9)
SyntaxV2.Anim9.BackgroundTransparency = 0.250
SyntaxV2.Anim9.Position = UDim2.new(0.0901960805, 0, 0.46442154, 0)
SyntaxV2.Anim9.Size = UDim2.new(0, 296, 0, 21)
SyntaxV2.Anim9.Font = Enum.Font.Nunito
SyntaxV2.Anim9.Text = "Orange Justice [R15]"
SyntaxV2.Anim9.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Anim9.TextSize = 14.000
SyntaxV2.Anim9.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6042054037"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()

	SyntaxV2.Anim9.Size = UDim2.new(0, 206, 0, 21)
	wait(0.1)
	SyntaxV2.Anim9.Size = UDim2.new(0, 296, 0, 21)
	SyntaxV2.Executor_2.Text = ""
SyntaxV2.TextInfo.Text = "[ Orange Justice R15 ] command loaded."
wait(1)
SyntaxV2.TextInfo.Text = "Welcome to Syntax V2 New Updates."

loadstring(game:GetObjects("rbxassetid://7571389889")[1].Source)()
end)

SyntaxV2.UICorner_86.Parent = SyntaxV2.Anim9

SyntaxV2.UIGradient_20.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(0, 0, 0)), ColorSequenceKeypoint.new(0.50, Color3.fromRGB(89, 0, 134)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(0, 0, 0))}
SyntaxV2.UIGradient_20.Rotation = 45
SyntaxV2.UIGradient_20.Parent = SyntaxV2.Frame_6

SyntaxV2.ColorMenu1_3.Name = "ColorMenu1"
SyntaxV2.ColorMenu1_3.Parent = SyntaxV2.AnimationsScripts
SyntaxV2.ColorMenu1_3.BackgroundColor3 = Color3.fromRGB(59, 0, 89)
SyntaxV2.ColorMenu1_3.BackgroundTransparency = 0.050
SyntaxV2.ColorMenu1_3.Position = UDim2.new(0.703139663, 0, -0.274857491, 0)
SyntaxV2.ColorMenu1_3.Size = UDim2.new(0, 344, 0, 44)

SyntaxV2.UICorner_87.Parent = SyntaxV2.ColorMenu1_3

SyntaxV2.ColorMenu1_4.Name = "ColorMenu1"
SyntaxV2.ColorMenu1_4.Parent = SyntaxV2.ColorMenu1_3
SyntaxV2.ColorMenu1_4.BackgroundColor3 = Color3.fromRGB(121, 0, 182)
SyntaxV2.ColorMenu1_4.BackgroundTransparency = 0.450
SyntaxV2.ColorMenu1_4.Position = UDim2.new(0.0712972805, 0, 0.216909245, 0)
SyntaxV2.ColorMenu1_4.Size = UDim2.new(0, 301, 0, 24)

SyntaxV2.UICorner_88.Parent = SyntaxV2.ColorMenu1_4

SyntaxV2.UIGradient_21.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(43, 0, 65)), ColorSequenceKeypoint.new(0.03, Color3.fromRGB(169, 0, 254)), ColorSequenceKeypoint.new(0.73, Color3.fromRGB(170, 0, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(170, 0, 255))}
SyntaxV2.UIGradient_21.Rotation = 45
SyntaxV2.UIGradient_21.Parent = SyntaxV2.ColorMenu1_3

SyntaxV2.TextLabel_5.Parent = SyntaxV2.AnimationsScripts
SyntaxV2.TextLabel_5.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel_5.BackgroundTransparency = 1.000
SyntaxV2.TextLabel_5.Position = UDim2.new(0.970000029, 0, -0.156666875, 0)
SyntaxV2.TextLabel_5.Size = UDim2.new(0, 301, 0, 20)
SyntaxV2.TextLabel_5.Font = Enum.Font.TitilliumWeb
SyntaxV2.TextLabel_5.Text = "Animations Scripts"
SyntaxV2.TextLabel_5.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel_5.TextSize = 24.000
SyntaxV2.TextLabel_5.TextWrapped = true

SyntaxV2.xd4_3.Name = "xd4"
SyntaxV2.xd4_3.Parent = SyntaxV2.AnimationsScripts
SyntaxV2.xd4_3.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.xd4_3.BackgroundTransparency = 0.350
SyntaxV2.xd4_3.BorderColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.xd4_3.Position = UDim2.new(-0.0599999987, 0, 0.275501728, 0)
SyntaxV2.xd4_3.Size = UDim2.new(0, 507, 0, 2)

SyntaxV2.UICorner_89.Parent = SyntaxV2.xd4_3

SyntaxV2.Home_3.Name = "Home"
SyntaxV2.Home_3.Parent = SyntaxV2.Main2
SyntaxV2.Home_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.Home_3.BackgroundTransparency = 1.000
SyntaxV2.Home_3.Size = UDim2.new(0, 511, 0, 199)

SyntaxV2.Frame_7.Parent = SyntaxV2.Home_3
SyntaxV2.Frame_7.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.Frame_7.BackgroundTransparency = 0.450
SyntaxV2.Frame_7.BorderColor3 = Color3.fromRGB(27, 42, 53)
SyntaxV2.Frame_7.Position = UDim2.new(0.013134025, 0, 0.0628856868, 0)
SyntaxV2.Frame_7.Size = UDim2.new(0, 492, 0, 174)

SyntaxV2.TextLabel_6.Parent = SyntaxV2.Frame_7
SyntaxV2.TextLabel_6.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel_6.BackgroundTransparency = 1.000
SyntaxV2.TextLabel_6.Position = UDim2.new(0.0926344097, 0, 0.0229885057, 0)
SyntaxV2.TextLabel_6.Size = UDim2.new(0, 425, 0, 40)
SyntaxV2.TextLabel_6.Font = Enum.Font.TitilliumWeb
SyntaxV2.TextLabel_6.Text = "Syntax project developed by the Null community all credits to them"
SyntaxV2.TextLabel_6.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.TextLabel_6.TextSize = 22.000
SyntaxV2.TextLabel_6.TextStrokeTransparency = 0.000
SyntaxV2.TextLabel_6.TextWrapped = true
SyntaxV2.TextLabel_6.TextXAlignment = Enum.TextXAlignment.Left

SyntaxV2.UICorner_90.Parent = SyntaxV2.Frame_7

SyntaxV2.ImageLabel_2.Parent = SyntaxV2.Frame_7
SyntaxV2.ImageLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.ImageLabel_2.BackgroundTransparency = 1.000
SyntaxV2.ImageLabel_2.Position = UDim2.new(0.0246913582, 0, 0.0632183924, 0)
SyntaxV2.ImageLabel_2.Size = UDim2.new(0, 26, 0, 26)
SyntaxV2.ImageLabel_2.Image = "http://www.roblox.com/asset/?id=3523243755"

SyntaxV2.xd4_4.Name = "xd4"
SyntaxV2.xd4_4.Parent = SyntaxV2.Home
SyntaxV2.xd4_4.BackgroundColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.xd4_4.BackgroundTransparency = 0.350
SyntaxV2.xd4_4.BorderColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.xd4_4.Position = UDim2.new(0, 0, 0.125501618, 0)
SyntaxV2.xd4_4.Size = UDim2.new(0, 150, 0, 2)

SyntaxV2.UICorner_91.Parent = SyntaxV2.xd4_4

SyntaxV2.xd4_5.Name = "xd4"
SyntaxV2.xd4_5.Parent = SyntaxV2.Home
SyntaxV2.xd4_5.BackgroundColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.xd4_5.BackgroundTransparency = 0.350
SyntaxV2.xd4_5.BorderColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.xd4_5.Position = UDim2.new(-0.00292825769, 0, 0.999288142, 0)
SyntaxV2.xd4_5.Size = UDim2.new(0, 152, 0, 2)

SyntaxV2.UICorner_92.Parent = SyntaxV2.xd4_5

SyntaxV2.xd4_6.Name = "xd4"
SyntaxV2.xd4_6.Parent = SyntaxV2.Home
SyntaxV2.xd4_6.BackgroundColor3 = Color3.fromRGB(170, 0, 255)
SyntaxV2.xd4_6.BackgroundTransparency = 0.350
SyntaxV2.xd4_6.BorderColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.xd4_6.Position = UDim2.new(0.237188876, 0, 0.26466018, 0)
SyntaxV2.xd4_6.Size = UDim2.new(0, 512, 0, 2)

SyntaxV2.UICorner_93.Parent = SyntaxV2.xd4_6

SyntaxV2.close.Name = "close"
SyntaxV2.close.Parent = SyntaxV2.Home
SyntaxV2.close.Active = false
SyntaxV2.close.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.close.BorderColor3 = Color3.fromRGB(0, 0, 0)
SyntaxV2.close.Position = UDim2.new(0.955705285, 0, 0, 0)
SyntaxV2.close.Size = UDim2.new(0, 30, 0, 23)
SyntaxV2.close.Font = Enum.Font.Gotham
SyntaxV2.close.Text = "X"
SyntaxV2.close.TextColor3 = Color3.fromRGB(255, 255, 255)
SyntaxV2.close.TextSize = 14.000
SyntaxV2.close.TextWrapped = true
SyntaxV2.close.MouseButton1Down:connect(function()
	--sounds and shits
	local s = Instance.new("Sound")
	s.Name = "Sound"
	s.SoundId = "https://web.roblox.com/asset/?id=6655851046"
	s.Volume = 0.5
	s.Looped = false
	s.archivable = false
	s.Parent = game.Workspace
	s:play()
	SyntaxV2.close.Size = UDim2.new(0, 25, 0, 19)
	wait(0.1)
	SyntaxV2.close.Size = UDim2.new(0, 30, 0, 23)
	SyntaxV2.SyntaxV2:Destroy()
end)


SyntaxV2.UICorner_94.Parent = SyntaxV2.close

-- Scripts:

local function VAGHUIK_fake_script() -- SyntaxV2.Login.LocalScript 
	local script = Instance.new('LocalScript', SyntaxV2.Login)

	local Key = script.Parent.Parent.Key
	
	script.Parent.MouseButton1Click:Connect(function()
		if Key.Text == "Syntaxbesthub" then
			script.Parent.Parent:TweenPosition(UDim2.new(0.383,0,-0.9,0), "Out", "Quad", 1, true)
			wait(2)
	local s = Instance.new("Sound")
			s.Name = "Sound"
			s.SoundId = "https://web.roblox.com/asset/?id=6228337171"
			s.Volume = 0.5
			s.Looped = false
			s.archivable = false
			s.Parent = game.Workspace
			s:play()
			script.Parent.Parent.Parent.Home:TweenPosition(UDim2.new(0.454, -250,0.523, -150), "Out", "Quad", 1, true)
			wait(5)
			script.Parent.Parent:Destroy()
		elseif
			Key.Text == "" then
			Key.Text = "" else
	local s = Instance.new("Sound")
			s.Name = "Sound"
			s.SoundId = "https://web.roblox.com/asset/?id=2851048659"
			s.Volume = 0.5
			s.Looped = false
			s.archivable = false
			s.Parent = game.Workspace
			s:play()
			Key.Text = "Wrong key, join Discord server"
			wait(2)
			Key.Text = ""
		end
	end)
end
coroutine.wrap(VAGHUIK_fake_script)()
local function XNIRQX_fake_script() -- SyntaxV2.SyntaxV2.Script 
	local script = Instance.new('Script', SyntaxV2.SyntaxV2)

	--last cordination {-10, -250},{0.5, -150}
	
	
	--new cordination {0.5, -250},{0.523, -150}
	
end
coroutine.wrap(XNIRQX_fake_script)()
local function WXQWPV_fake_script() -- SyntaxV2.Home.Dragify 
	local script = Instance.new('LocalScript', SyntaxV2.Home)

	local UIS = game:GetService("UserInputService")
	function dragify(Frame)
	    dragToggle = nil
	    local dragSpeed = 0.50
	    dragInput = nil
	    dragStart = nil
	    local dragPos = nil
	    function updateInput(input)
	        local Delta = input.Position - dragStart
	        local Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + Delta.X, startPos.Y.Scale, startPos.Y.Offset + Delta.Y)
	        game:GetService("TweenService"):Create(Frame, TweenInfo.new(0.30), {Position = Position}):Play()
	    end
	    Frame.InputBegan:Connect(function(input)
	        if (input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch) and UIS:GetFocusedTextBox() == nil then
	            dragToggle = true
	            dragStart = input.Position
	            startPos = Frame.Position
	            input.Changed:Connect(function()
	                if input.UserInputState == Enum.UserInputState.End then
	                    dragToggle = false
	                end
	            end)
	        end
	    end)
	    Frame.InputChanged:Connect(function(input)
	        if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
	            dragInput = input
	        end
	    end)
	    game:GetService("UserInputService").InputChanged:Connect(function(input)
	        if input == dragInput and dragToggle then
	            updateInput(input)
	        end
	    end)
	end
	
	dragify(script.Parent)
end
coroutine.wrap(WXQWPV_fake_script)()
local function OAZA_fake_script() -- SyntaxV2.Executor_2.Script 
	local script = Instance.new('Script', SyntaxV2.Executor_2)

	local TweenService = game:GetService("TweenService")
	
	local part = script.Parent
	
	local colors =
	{
		Color3.fromRGB(255, 0, 0); --red
		Color3.fromRGB(255, 0, 255); --pink
		Color3.fromRGB(0, 0, 255); --blue
		Color3.fromRGB(0, 255, 255); --cyan
		Color3.fromRGB(0, 255, 0); --green
		Color3.fromRGB(255, 255, 0); --yellow
	}
	
	local tweenTime = 0.8
	 
	while true do
		for i, v in pairs(colors) do
			local goal = {}
			goal.TextColor3 = v
			 
			local tweenInfo = TweenInfo.new(tweenTime, Enum.EasingStyle.Linear, Enum.EasingDirection.Out, 0, false)
			 
			local tween = TweenService:Create(part, tweenInfo, goal)
			 
			tween:Play()
			wait(tweenTime)
		end
		wait()
	end
end
coroutine.wrap(OAZA_fake_script)()
local function QXTX_fake_script() -- SyntaxV2.ImageLabel.LocalScript 
	local script = Instance.new('LocalScript', SyntaxV2.ImageLabel)

	
	local Players = game:GetService("Players")
	
	local player = Players.LocalPlayer
	
	local userId = player.UserId
	local thumbType = Enum.ThumbnailType.HeadShot
	local thumbSize = Enum.ThumbnailSize.Size420x420
	local content, isReady = Players:GetUserThumbnailAsync(userId, thumbType, thumbSize)
	
	local imageLabel = script.Parent
	imageLabel.Image = content
end
coroutine.wrap(QXTX_fake_script)()
