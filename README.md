--[=[
 script by = MoonVM
 UI by = MoonVM
 project Trez Ultimate Hacking Suite
]=]

-- Instances: 31 | Scripts: 8 | Modules: 0 | Tags: 0
local G2L = {};



-- Load Only Once!
if not getgenv()._LOL then
	getgenv()._LOL = true
else
	print("Project Trez Already running")
	game.StarterGui:SetCore("SendNotification", {
		Title = "Settings";
		Text = "Project Trez Already Running !!";
		Duration = 5; 
	})
	return
end

game.StarterGui:SetCore("SendNotification", {
	Title = "Settings";
	Text = "Project Trez Loaded !!!";
	Duration = 5; 
})
-- StarterGui.ScreenGui
G2L["1"] = Instance.new("ScreenGui", game.CoreGui);
G2L["1"]["IgnoreGuiInset"] = true;
G2L["1"]["ScreenInsets"] = Enum.ScreenInsets.DeviceSafeInsets;
G2L["1"]["ZIndexBehavior"] = Enum.ZIndexBehavior.Sibling;
G2L["1"]["ResetOnSpawn"] = false;


-- StarterGui.ScreenGui.Logo
G2L["2"] = Instance.new("ImageLabel", G2L["1"]);
G2L["2"]["ZIndex"] = 2;
G2L["2"]["BorderSizePixel"] = 0;
G2L["2"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["2"]["ImageTransparency"] = 1;
-- [ERROR] cannot convert ImageContent, please report to "https://github.com/uniquadev/GuiToLuaConverter/issues"
G2L["2"]["ImageColor3"] = Color3.fromRGB(9, 141, 255);
G2L["2"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
G2L["2"]["Image"] = [[rbxassetid://14421964660]];
G2L["2"]["Size"] = UDim2.new(0.04857, 29, 0.05368, 26);
G2L["2"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["2"]["BackgroundTransparency"] = 1;
G2L["2"]["Name"] = [[Logo]];
G2L["2"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);


-- StarterGui.ScreenGui.Logo.UIAspectRatioConstraint
G2L["3"] = Instance.new("UIAspectRatioConstraint", G2L["2"]);



-- StarterGui.ScreenGui.Logo.LocalScript
G2L["4"] = Instance.new("LocalScript", G2L["2"]);



-- StarterGui.ScreenGui.Frame
G2L["5"] = Instance.new("Frame", G2L["1"]);
G2L["5"]["BorderSizePixel"] = 0;
G2L["5"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["5"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
G2L["5"]["Size"] = UDim2.new(0, 483, 0, 272);
G2L["5"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);
G2L["5"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);


-- StarterGui.ScreenGui.Frame.CodeFrame
G2L["6"] = Instance.new("ScrollingFrame", G2L["5"]);
G2L["6"]["Active"] = true;
G2L["6"]["BorderSizePixel"] = 0;
G2L["6"]["CanvasSize"] = UDim2.new(0, 0, 4, 0);
G2L["6"]["TopImage"] = [[]];
G2L["6"]["BackgroundColor3"] = Color3.fromRGB(242, 242, 242);
G2L["6"]["Name"] = [[CodeFrame]];
G2L["6"]["ScrollBarImageTransparency"] = 0.73;
G2L["6"]["BottomImage"] = [[]];
G2L["6"]["Size"] = UDim2.new(0, 351, 0, 223);
G2L["6"]["ScrollBarImageColor3"] = Color3.fromRGB(0, 0, 0);
G2L["6"]["Position"] = UDim2.new(0.01863, 0, 0.13971, 0);
G2L["6"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);


-- StarterGui.ScreenGui.Frame.CodeFrame.UIListLayout
G2L["7"] = Instance.new("UIListLayout", G2L["6"]);
G2L["7"]["SortOrder"] = Enum.SortOrder.LayoutOrder;


-- StarterGui.ScreenGui.Frame.CodeFrame.TextBox
G2L["8"] = Instance.new("TextBox", G2L["6"]);
G2L["8"]["CursorPosition"] = -1;
G2L["8"]["TextXAlignment"] = Enum.TextXAlignment.Left;
G2L["8"]["BorderSizePixel"] = 0;
G2L["8"]["TextWrapped"] = true;
G2L["8"]["TextSize"] = 18;
G2L["8"]["TextColor3"] = Color3.fromRGB(0, 0, 0);
G2L["8"]["TextYAlignment"] = Enum.TextYAlignment.Top;
G2L["8"]["BackgroundColor3"] = Color3.fromRGB(242, 242, 242);
G2L["8"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["8"]["MultiLine"] = true;
G2L["8"]["ClearTextOnFocus"] = false;
G2L["8"]["PlaceholderText"] = [[print("wow")]];
G2L["8"]["Size"] = UDim2.new(0, 339, 0, 1083);
G2L["8"]["Position"] = UDim2.new(-0.54701, 0, 0.07169, 0);
G2L["8"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["8"]["Text"] = [[]];


-- StarterGui.ScreenGui.Frame.CodeFrame.TextBox.LocalScript
G2L["9"] = Instance.new("LocalScript", G2L["8"]);



-- StarterGui.ScreenGui.Frame.CodeFrame.UIStroke
G2L["a"] = Instance.new("UIStroke", G2L["6"]);
G2L["a"]["Transparency"] = 0.69;
G2L["a"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
G2L["a"]["LineJoinMode"] = Enum.LineJoinMode.Miter;
G2L["a"]["Thickness"] = 0.4;


-- StarterGui.ScreenGui.Frame.Exe
G2L["b"] = Instance.new("TextButton", G2L["5"]);
G2L["b"]["BorderSizePixel"] = 0;
G2L["b"]["TextSize"] = 14;
G2L["b"]["TextColor3"] = Color3.fromRGB(162, 162, 162);
G2L["b"]["BackgroundColor3"] = Color3.fromRGB(242, 242, 242);
G2L["b"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["b"]["Size"] = UDim2.new(0, 100, 0, 92);
G2L["b"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["b"]["Text"] = [[Execute]];
G2L["b"]["Name"] = [[Exe]];
G2L["b"]["Position"] = UDim2.new(0.77019, 0, 0.13971, 0);


-- StarterGui.ScreenGui.Frame.Exe.UIStroke
G2L["c"] = Instance.new("UIStroke", G2L["b"]);
G2L["c"]["Transparency"] = 0.69;
G2L["c"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
G2L["c"]["LineJoinMode"] = Enum.LineJoinMode.Miter;
G2L["c"]["Thickness"] = 0.4;


-- StarterGui.ScreenGui.Frame.Exe.LocalScript
G2L["d"] = Instance.new("LocalScript", G2L["b"]);



-- StarterGui.ScreenGui.Frame.Clear
G2L["e"] = Instance.new("TextButton", G2L["5"]);
G2L["e"]["BorderSizePixel"] = 0;
G2L["e"]["TextSize"] = 14;
G2L["e"]["TextColor3"] = Color3.fromRGB(162, 162, 162);
G2L["e"]["BackgroundColor3"] = Color3.fromRGB(242, 242, 242);
G2L["e"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["e"]["Size"] = UDim2.new(0, 100, 0, 92);
G2L["e"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["e"]["Text"] = [[Clear]];
G2L["e"]["Name"] = [[Clear]];
G2L["e"]["Position"] = UDim2.new(0.77019, 0, 0.50735, 0);


-- StarterGui.ScreenGui.Frame.Clear.UIStroke
G2L["f"] = Instance.new("UIStroke", G2L["e"]);
G2L["f"]["Transparency"] = 0.69;
G2L["f"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
G2L["f"]["LineJoinMode"] = Enum.LineJoinMode.Miter;
G2L["f"]["Thickness"] = 0.4;


-- StarterGui.ScreenGui.Frame.Clear.LocalScript
G2L["10"] = Instance.new("LocalScript", G2L["e"]);



-- StarterGui.ScreenGui.Frame.Inject
G2L["11"] = Instance.new("TextButton", G2L["5"]);
G2L["11"]["BorderSizePixel"] = 0;
G2L["11"]["TextSize"] = 14;
G2L["11"]["TextColor3"] = Color3.fromRGB(162, 162, 162);
G2L["11"]["BackgroundColor3"] = Color3.fromRGB(242, 242, 242);
G2L["11"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["11"]["Size"] = UDim2.new(0, 100, 0, 22);
G2L["11"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["11"]["Text"] = [[Inject]];
G2L["11"]["Name"] = [[Inject]];
G2L["11"]["Position"] = UDim2.new(0.77019, 0, 0.87868, 0);


-- StarterGui.ScreenGui.Frame.Inject.UIStroke
G2L["12"] = Instance.new("UIStroke", G2L["11"]);
G2L["12"]["Transparency"] = 0.69;
G2L["12"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
G2L["12"]["LineJoinMode"] = Enum.LineJoinMode.Miter;
G2L["12"]["Thickness"] = 0.4;


-- StarterGui.ScreenGui.Frame.Inject.LocalScript
G2L["13"] = Instance.new("LocalScript", G2L["11"]);



-- StarterGui.ScreenGui.Frame.UIStroke
G2L["14"] = Instance.new("UIStroke", G2L["5"]);
G2L["14"]["Transparency"] = 0.69;
G2L["14"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
G2L["14"]["LineJoinMode"] = Enum.LineJoinMode.Miter;
G2L["14"]["Thickness"] = 0.4;


-- StarterGui.ScreenGui.Frame.ImageLabel
G2L["15"] = Instance.new("ImageLabel", G2L["5"]);
G2L["15"]["BorderSizePixel"] = 0;
G2L["15"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
-- [ERROR] cannot convert ImageContent, please report to "https://github.com/uniquadev/GuiToLuaConverter/issues"
G2L["15"]["ImageColor3"] = Color3.fromRGB(9, 141, 255);
G2L["15"]["Image"] = [[rbxassetid://14421964660]];
G2L["15"]["Size"] = UDim2.new(0, 29, -0.01, 26);
G2L["15"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["15"]["BackgroundTransparency"] = 1;
G2L["15"]["Position"] = UDim2.new(0.01859, 0, 0.03649, 0);


-- StarterGui.ScreenGui.Frame.ImageLabel.UIAspectRatioConstraint
G2L["16"] = Instance.new("UIAspectRatioConstraint", G2L["15"]);



-- StarterGui.ScreenGui.Frame.TextLabel
G2L["17"] = Instance.new("TextLabel", G2L["5"]);
G2L["17"]["BorderSizePixel"] = 0;
G2L["17"]["TextSize"] = 18;
G2L["17"]["TextXAlignment"] = Enum.TextXAlignment.Left;
G2L["17"]["BackgroundColor3"] = Color3.fromRGB(9, 132, 238);
G2L["17"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Bold, Enum.FontStyle.Italic);
G2L["17"]["TextColor3"] = Color3.fromRGB(9, 132, 238);
G2L["17"]["BackgroundTransparency"] = 1;
G2L["17"]["Size"] = UDim2.new(0, 201, 0, 22);
G2L["17"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["17"]["Text"] = [[Project Trez]];
G2L["17"]["Position"] = UDim2.new(0.08126, 0, 0.03649, 0);


-- StarterGui.ScreenGui.Frame.TextLabel.UIStroke
G2L["18"] = Instance.new("UIStroke", G2L["17"]);
G2L["18"]["LineJoinMode"] = Enum.LineJoinMode.Miter;
G2L["18"]["Thickness"] = 1.3;
G2L["18"]["Color"] = Color3.fromRGB(5, 66, 117);


-- StarterGui.ScreenGui.Frame.UIDrag
G2L["19"] = Instance.new("LocalScript", G2L["5"]);
G2L["19"]["Name"] = [[UIDrag]];


-- StarterGui.ScreenGui.Frame.RE
G2L["1a"] = Instance.new("TextButton", G2L["5"]);
G2L["1a"]["BorderSizePixel"] = 0;
G2L["1a"]["TextSize"] = 14;
G2L["1a"]["TextColor3"] = Color3.fromRGB(162, 162, 162);
G2L["1a"]["BackgroundColor3"] = Color3.fromRGB(242, 242, 242);
G2L["1a"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["1a"]["Size"] = UDim2.new(-0.02516, 100, 0, 22);
G2L["1a"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["1a"]["Text"] = [[RE]];
G2L["1a"]["Name"] = [[RE]];
G2L["1a"]["Position"] = UDim2.new(0.79534, 0, 0.03309, 0);


-- StarterGui.ScreenGui.Frame.RE.UIStroke
G2L["1b"] = Instance.new("UIStroke", G2L["1a"]);
G2L["1b"]["Transparency"] = 0.69;
G2L["1b"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
G2L["1b"]["LineJoinMode"] = Enum.LineJoinMode.Miter;
G2L["1b"]["Thickness"] = 0.4;


-- StarterGui.ScreenGui.Frame.RE.LocalScript
G2L["1c"] = Instance.new("LocalScript", G2L["1a"]);



-- StarterGui.ScreenGui.Frame.R6
G2L["1d"] = Instance.new("TextButton", G2L["5"]);
G2L["1d"]["BorderSizePixel"] = 0;
G2L["1d"]["TextSize"] = 14;
G2L["1d"]["TextColor3"] = Color3.fromRGB(162, 162, 162);
G2L["1d"]["BackgroundColor3"] = Color3.fromRGB(242, 242, 242);
G2L["1d"]["FontFace"] = Font.new([[rbxasset://fonts/families/Ubuntu.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["1d"]["Size"] = UDim2.new(-0.02516, 100, 0, 22);
G2L["1d"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["1d"]["Text"] = [[R6]];
G2L["1d"]["Name"] = [[R6]];
G2L["1d"]["Position"] = UDim2.new(0.59534, 0, 0.03309, 0);


-- StarterGui.ScreenGui.Frame.R6.UIStroke
G2L["1e"] = Instance.new("UIStroke", G2L["1d"]);
G2L["1e"]["Transparency"] = 0.69;
G2L["1e"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;
G2L["1e"]["LineJoinMode"] = Enum.LineJoinMode.Miter;
G2L["1e"]["Thickness"] = 0.4;


-- StarterGui.ScreenGui.Frame.R6.LocalScript
G2L["1f"] = Instance.new("LocalScript", G2L["1d"]);



-- StarterGui.ScreenGui.Logo.LocalScript
local function C_4()
local script = G2L["4"];
	for i = 1, 0, -0.05 do
		script.Parent.ImageTransparency = i
		wait(0.01)
		
	end
	
	script.Parent:TweenPosition(UDim2.new(0.04, 0,0.92, 0))
	
	while true do
		for i = 0, 25, 1 do
			script.Parent.Rotation = i
			wait(0.02)
		end
	
		for i = 25, -25, -1 do
			script.Parent.Rotation = i
			wait(0.02)
		end
	
		for i = -25, 0, 1 do
			script.Parent.Rotation = i
			wait(0.02)
		end
	end
	
end;
task.spawn(C_4);
-- StarterGui.ScreenGui.Frame.CodeFrame.TextBox.LocalScript
local function C_9()
local script = G2L["9"];
	getgenv().CodeBox = script.Parent
end;
task.spawn(C_9);
-- StarterGui.ScreenGui.Frame.Exe.LocalScript
local function C_d()
local script = G2L["d"];
	local function notify(msg)
		game.StarterGui:SetCore("SendNotification", {
			Title = "Project Trez",
			Text = msg,
			Duration = 5,
		})
	end
	
	
	local remote = game.ReplicatedStorage:FindFirstChild("MoonVM")
	script.Parent.MouseButton1Click:Connect(function()
		if not game.ReplicatedStorage:FindFirstChild("MoonVM") then
			notify("Please Inject Before running!")
		else
			pcall(function()
				loadstring(getgenv().CodeBox.Text)()
			end)
		end
	end)
end;
task.spawn(C_d);
-- StarterGui.ScreenGui.Frame.Clear.LocalScript
local function C_10()
local script = G2L["10"];
	script.Parent.MouseButton1Click:Connect(function()
		if not getgenv().CodeBox  then
			return getgenv().CodeBox == script.Parent.Parent.CodeFrame.TextBox
		end
		
		getgenv().CodeBox.Text = ""
	end)
end;
task.spawn(C_10);
-- StarterGui.ScreenGui.Frame.Inject.LocalScript
local function C_13()
local script = G2L["13"];
	local remote = Instance.new("BindableFunction")
	remote.Name = "MoonVM"
	local function IsInjected()
		if game.ReplicatedStorage:FindFirstChild("MoonVM") then
			return true
		else
			return false
		end
	end
	
	
	local function notify(msg)
		game.StarterGui:SetCore("SendNotification", {
			Title = "Project Trez",
			Text = msg,
			Duration = 5,
		})
	end
	
	
	script.Parent.MouseButton1Click:Connect(function()
		if IsInjected() then
			notify("Already Injected")
			return
		end
		remote.Parent = game.ReplicatedStorage
		notify("Successfully Injected")
		script.Parent.Parent.Parent.Logo:TweenPosition(UDim2.new(0.5, 0,0.5, 0))
		wait(2)
		script.Parent.Parent.Parent.Logo:TweenPosition(UDim2.new(0.04, 0,0.92, 0))
		
	
	end)
end;
task.spawn(C_13);
-- StarterGui.ScreenGui.Frame.UIDrag
local function C_19()
local script = G2L["19"];
	-- Made by Real_IceyDev (@lceyDex) --
	-- Simple UI dragger (PC Only/Any device that has a mouse) --
	
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
end;
task.spawn(C_19);
-- StarterGui.ScreenGui.Frame.RE.LocalScript
local function C_1c()
local script = G2L["1c"];
	script.Parent.MouseButton1Click:Connect(function()
		for i,v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
			if v:IsA("Humanoid") then
				v.Health = 0
			end
		end
	end)
end;
task.spawn(C_1c);
-- StarterGui.ScreenGui.Frame.R6.LocalScript
local function C_1f()
local script = G2L["1f"];
	
	script.Parent.MouseButton1Click:Connect(function()
		function oof()
			local Players = game:GetService("Players")
			local plr = Players.LocalPlayer
			local char = plr.Character or plr.CharacterAdded:Wait()
	
			
			if char:FindFirstChild("Humanoid") and char.Humanoid.RigType == Enum.HumanoidRigType.R15 then
				local desc = Players:GetHumanoidDescriptionFromUserId(plr.CharacterAppearanceId)
				local newChar = Players:CreateHumanoidModelFromDescription(desc, Enum.HumanoidRigType.R6)
				newChar.Name = plr.Name
	
				if not newChar.PrimaryPart and newChar:FindFirstChild("HumanoidRootPart") then
					newChar.PrimaryPart = newChar:FindFirstChild("HumanoidRootPart")
				end
				if newChar.PrimaryPart and char:FindFirstChild("HumanoidRootPart") then
					newChar:SetPrimaryPartCFrame(char.PrimaryPart.CFrame)
				end
	
				char:Destroy()
				newChar.Parent = workspace
				plr.Character = newChar
	
				local cam = workspace.CurrentCamera
				cam.CameraSubject = newChar:WaitForChild("Humanoid")
				cam.CameraType = Enum.CameraType.Custom
			end
	
			local c = workspace:WaitForChild(plr.Name)
			local Humanoid = c:WaitForChild("Humanoid")
			local pose = "Standing"
			local currentAnimTrack = nil
			local currentAnimSpeed = 1.0
	
			
			local anims = {
				idle = "http://www.roblox.com/asset/?id=180435571",
				walk = "http://www.roblox.com/asset/?id=180426354",
				jump = "http://www.roblox.com/asset/?id=125750702",
				fall = "http://www.roblox.com/asset/?id=180436148"
			}
	
			
			local function playAnim(animId, speed)
				if currentAnimTrack then
					currentAnimTrack:Stop()
					currentAnimTrack:Destroy()
				end
				local anim = Instance.new("Animation")
				anim.AnimationId = animId
				currentAnimTrack = Humanoid:LoadAnimation(anim)
				currentAnimTrack.Priority = Enum.AnimationPriority.Core
				currentAnimTrack:Play(0.1)
				if speed then
					currentAnimTrack:AdjustSpeed(speed)
				else
					currentAnimTrack:AdjustSpeed(1.0)
				end
			end
	
			
			Humanoid.Running:Connect(function(speed)
				if speed > 0.01 then
					playAnim(anims.walk, speed / Humanoid.WalkSpeed)
					pose = "Running"
				else
					playAnim(anims.idle)
					pose = "Standing"
				end
			end)
	
			Humanoid.Jumping:Connect(function()
				playAnim(anims.jump)
				pose = "Jumping"
			end)
	
			Humanoid.FreeFalling:Connect(function()
				if pose ~= "Jumping" then
					playAnim(anims.fall)
					pose = "FreeFall"
				end
			end)
	
			Humanoid.Died:Connect(function()
				pose = "Dead"
			end)
	
			
			playAnim(anims.idle)
			pose = "Standing"
		end
	
		oof()
	
		local UIS = game:GetService("UserInputService")
		local plr = game.Players.LocalPlayer
		local deathPos = nil
	
		plr.CharacterAdded:Connect(function(char)
			local hrp = char:WaitForChild("HumanoidRootPart")
			if deathPos then
				hrp.CFrame = deathPos
			end
		end)
	
		while true do wait(0.1)
			local char = plr.Character
			if char and char:FindFirstChild("Humanoid") then
				if char.Humanoid.Health <= 0 then
					local hrp = char:FindFirstChild("HumanoidRootPart")
					if hrp then
						deathPos = hrp.CFrame
					end
				end
			end
		end
	
	end)
end;
task.spawn(C_1f);

return G2L["1"], require;
