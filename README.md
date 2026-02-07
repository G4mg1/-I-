--[=[
 d888b  db    db d888888b      .d888b.      db      db    db  .d8b.  
88' Y8b 88    88   `88'        VP  `8D      88      88    88 d8' `8b 
88      88    88    88            odD'      88      88    88 88ooo88 
88  ooo 88    88    88          .88'        88      88    88 88~~~88 
88. ~8~ 88b  d88   .88.        j88.         88booo. 88b  d88 88   88    @uniquadev
 Y888P  ~Y8888P' Y888888P      888888D      Y88888P ~Y8888P' YP   YP  CONVERTER 
]=]

-- Instances: 30 | Scripts: 7 | Modules: 0 | Tags: 0
local G2L = {};

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

-- StarterGui.Trez
G2L["1"] = Instance.new("ScreenGui", game.CoreGui);
G2L["1"]["Name"] = [[Trez]];
G2L["1"]["ZIndexBehavior"] = Enum.ZIndexBehavior.Sibling;


-- StarterGui.Trez.MainBG
G2L["2"] = Instance.new("Frame", G2L["1"]);
G2L["2"]["BorderSizePixel"] = 0;
G2L["2"]["BackgroundColor3"] = Color3.fromRGB(44, 44, 44);
G2L["2"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
G2L["2"]["Size"] = UDim2.new(0, 384, 0, 233);
G2L["2"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);
G2L["2"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["2"]["Name"] = [[MainBG]];


-- StarterGui.Trez.MainBG.TopBar
G2L["3"] = Instance.new("Frame", G2L["2"]);
G2L["3"]["BorderSizePixel"] = 0;
G2L["3"]["BackgroundColor3"] = Color3.fromRGB(66, 66, 66);
G2L["3"]["Size"] = UDim2.new(0, 384, 0, 24);
G2L["3"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["3"]["Name"] = [[TopBar]];


-- StarterGui.Trez.MainBG.TopBar.Close
G2L["4"] = Instance.new("TextButton", G2L["3"]);
G2L["4"]["BorderSizePixel"] = 0;
G2L["4"]["TextSize"] = 19;
G2L["4"]["TextColor3"] = Color3.fromRGB(100, 100, 100);
G2L["4"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["4"]["FontFace"] = Font.new([[rbxasset://fonts/families/Jura.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
G2L["4"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
G2L["4"]["BackgroundTransparency"] = 1;
G2L["4"]["Size"] = UDim2.new(-0.02, 22, 0, 22);
G2L["4"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["4"]["Text"] = [[>]];
G2L["4"]["Name"] = [[Close]];
G2L["4"]["Rotation"] = 90;
G2L["4"]["Position"] = UDim2.new(0.97, 0, 0.5, 0);


-- StarterGui.Trez.MainBG.TopBar.Close.UIPadding
G2L["5"] = Instance.new("UIPadding", G2L["4"]);



-- StarterGui.Trez.MainBG.TopBar.Close.UIAspectRatioConstraint
G2L["6"] = Instance.new("UIAspectRatioConstraint", G2L["4"]);



-- StarterGui.Trez.MainBG.TopBar.Toggle
G2L["7"] = Instance.new("LocalScript", G2L["3"]);
G2L["7"]["Name"] = [[Toggle]];


-- StarterGui.Trez.MainBG.TopBar.PName
G2L["8"] = Instance.new("TextLabel", G2L["3"]);
G2L["8"]["TextWrapped"] = true;
G2L["8"]["BorderSizePixel"] = 0;
G2L["8"]["TextSize"] = 14;
G2L["8"]["TextXAlignment"] = Enum.TextXAlignment.Left;
G2L["8"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["8"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["8"]["TextColor3"] = Color3.fromRGB(181, 181, 181);
G2L["8"]["BackgroundTransparency"] = 1;
G2L["8"]["Size"] = UDim2.new(0, 296, 0, 19);
G2L["8"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["8"]["Text"] = [[Project Trez]];
G2L["8"]["Name"] = [[PName]];
G2L["8"]["Position"] = UDim2.new(0.01604, 0, 0.16667, 0);


-- StarterGui.Trez.MainBG.TopBar.PName.UIPadding
G2L["9"] = Instance.new("UIPadding", G2L["8"]);
G2L["9"]["PaddingLeft"] = UDim.new(0, 2);
G2L["9"]["PaddingBottom"] = UDim.new(0, 5);


-- StarterGui.Trez.MainBG.TopBar.UltimateClose
G2L["a"] = Instance.new("TextButton", G2L["3"]);
G2L["a"]["BorderSizePixel"] = 0;
G2L["a"]["TextSize"] = 19;
G2L["a"]["TextColor3"] = Color3.fromRGB(100, 100, 100);
G2L["a"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["a"]["FontFace"] = Font.new([[rbxasset://fonts/families/Jura.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
G2L["a"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
G2L["a"]["BackgroundTransparency"] = 1;
G2L["a"]["Size"] = UDim2.new(-0.02, 22, 0, 22);
G2L["a"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["a"]["Text"] = [[-]];
G2L["a"]["Name"] = [[UltimateClose]];
G2L["a"]["Position"] = UDim2.new(0.92, 0, 0.5, 0);


-- StarterGui.Trez.MainBG.TopBar.UltimateClose.UIPadding
G2L["b"] = Instance.new("UIPadding", G2L["a"]);



-- StarterGui.Trez.MainBG.TopBar.UltimateClose.UIAspectRatioConstraint
G2L["c"] = Instance.new("UIAspectRatioConstraint", G2L["a"]);



-- StarterGui.Trez.MainBG.UIDrag
G2L["d"] = Instance.new("LocalScript", G2L["2"]);
G2L["d"]["Name"] = [[UIDrag]];


-- StarterGui.Trez.MainBG.Executor
G2L["e"] = Instance.new("Folder", G2L["2"]);
G2L["e"]["Name"] = [[Executor]];


-- StarterGui.Trez.MainBG.Executor.Clear
G2L["f"] = Instance.new("TextButton", G2L["e"]);
G2L["f"]["BorderSizePixel"] = 0;
G2L["f"]["TextSize"] = 14;
G2L["f"]["TextColor3"] = Color3.fromRGB(166, 166, 166);
G2L["f"]["BackgroundColor3"] = Color3.fromRGB(60, 60, 60);
G2L["f"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["f"]["Size"] = UDim2.new(-0.00597, 182, 0.00009, 20);
G2L["f"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["f"]["Text"] = [[Clear]];
G2L["f"]["Name"] = [[Clear]];
G2L["f"]["Visible"] = false;
G2L["f"]["Position"] = UDim2.new(0.51358, 0, 0.88492, 0);


-- StarterGui.Trez.MainBG.Executor.Clear.LocalScript
G2L["10"] = Instance.new("LocalScript", G2L["f"]);



-- StarterGui.Trez.MainBG.Executor.MainCodeFrame
G2L["11"] = Instance.new("ScrollingFrame", G2L["e"]);
G2L["11"]["Visible"] = false;
G2L["11"]["Active"] = true;
G2L["11"]["BorderSizePixel"] = 0;
G2L["11"]["CanvasSize"] = UDim2.new(0, 0, 900, 0);
G2L["11"]["BackgroundColor3"] = Color3.fromRGB(91, 91, 91);
G2L["11"]["Name"] = [[MainCodeFrame]];
G2L["11"]["Size"] = UDim2.new(0.11097, 326, 0.01154, 164);
G2L["11"]["ScrollBarImageColor3"] = Color3.fromRGB(0, 0, 0);
G2L["11"]["Position"] = UDim2.new(0.02604, 0, 0.14163, 0);
G2L["11"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["11"]["BackgroundTransparency"] = 0.9;


-- StarterGui.Trez.MainBG.Executor.MainCodeFrame.TextBox
G2L["12"] = Instance.new("TextBox", G2L["11"]);
G2L["12"]["CursorPosition"] = -1;
G2L["12"]["TextXAlignment"] = Enum.TextXAlignment.Left;
G2L["12"]["PlaceholderColor3"] = Color3.fromRGB(179, 179, 179);
G2L["12"]["BorderSizePixel"] = 0;
G2L["12"]["TextWrapped"] = true;
G2L["12"]["TextSize"] = 14;
G2L["12"]["ShowNativeInput"] = false;
G2L["12"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
G2L["12"]["TextYAlignment"] = Enum.TextYAlignment.Top;
G2L["12"]["BackgroundColor3"] = Color3.fromRGB(34, 34, 34);
G2L["12"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["12"]["MultiLine"] = true;
G2L["12"]["ClearTextOnFocus"] = false;
G2L["12"]["PlaceholderText"] = [[print("SSP")]];
G2L["12"]["Size"] = UDim2.new(0.111, 310, 0.71, 1134);
G2L["12"]["Position"] = UDim2.new(0, 0, -0.30693, 0);
G2L["12"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["12"]["Text"] = [[]];


-- StarterGui.Trez.MainBG.Executor.MainCodeFrame.TextBox.UIPadding
G2L["13"] = Instance.new("UIPadding", G2L["12"]);
G2L["13"]["PaddingLeft"] = UDim.new(0, 25);


-- StarterGui.Trez.MainBG.Executor.MainCodeFrame.TextBox.LineCount
G2L["14"] = Instance.new("TextLabel", G2L["12"]);
G2L["14"]["TextWrapped"] = true;
G2L["14"]["BorderSizePixel"] = 0;
G2L["14"]["TextSize"] = 14;
G2L["14"]["TextYAlignment"] = Enum.TextYAlignment.Top;
G2L["14"]["BackgroundColor3"] = Color3.fromRGB(66, 66, 66);
G2L["14"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["14"]["TextColor3"] = Color3.fromRGB(196, 196, 196);
G2L["14"]["BackgroundTransparency"] = 0.2;
G2L["14"]["Size"] = UDim2.new(-0.899, 310, 0.996, 602);
G2L["14"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["14"]["Text"] = [[1]];
G2L["14"]["Name"] = [[LineCount]];
G2L["14"]["Position"] = UDim2.new(-0.07677, 0, 0, 0);


-- StarterGui.Trez.MainBG.Executor.MainCodeFrame.TextBox.LocalScript
G2L["15"] = Instance.new("LocalScript", G2L["12"]);



-- StarterGui.Trez.MainBG.Executor.MainCodeFrame.TextBox.LocalScript
G2L["16"] = Instance.new("LocalScript", G2L["12"]);



-- StarterGui.Trez.MainBG.Executor.MainCodeFrame.UIListLayout
G2L["17"] = Instance.new("UIListLayout", G2L["11"]);
G2L["17"]["SortOrder"] = Enum.SortOrder.LayoutOrder;


-- StarterGui.Trez.MainBG.Executor.Execute
G2L["18"] = Instance.new("TextButton", G2L["e"]);
G2L["18"]["BorderSizePixel"] = 0;
G2L["18"]["TextSize"] = 14;
G2L["18"]["TextColor3"] = Color3.fromRGB(166, 166, 166);
G2L["18"]["BackgroundColor3"] = Color3.fromRGB(60, 60, 60);
G2L["18"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["18"]["Size"] = UDim2.new(-0.00597, 182, 0.00009, 20);
G2L["18"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["18"]["Text"] = [[Execute]];
G2L["18"]["Name"] = [[Execute]];
G2L["18"]["Visible"] = false;
G2L["18"]["Position"] = UDim2.new(0.02604, 0, 0.88492, 0);


-- StarterGui.Trez.MainBG.Executor.Execute.LocalScript
G2L["19"] = Instance.new("LocalScript", G2L["18"]);



-- StarterGui.Trez.MainBG.Loading
G2L["1a"] = Instance.new("ImageLabel", G2L["2"]);
G2L["1a"]["BorderSizePixel"] = 0;
G2L["1a"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
-- [ERROR] cannot convert ImageContent, please report to "https://github.com/uniquadev/GuiToLuaConverter/issues"
G2L["1a"]["ImageColor3"] = Color3.fromRGB(114, 114, 114);
G2L["1a"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
G2L["1a"]["Image"] = [[rbxassetid://80990588449079]];
G2L["1a"]["Size"] = UDim2.new(0, 100, 0, 100);
G2L["1a"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["1a"]["BackgroundTransparency"] = 1;
G2L["1a"]["Name"] = [[Loading]];
G2L["1a"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);


-- StarterGui.Trez.MainBG.Loading.LocalScript
G2L["1b"] = Instance.new("LocalScript", G2L["1a"]);



-- StarterGui.Trez.MainBG.LoadCount
G2L["1c"] = Instance.new("TextLabel", G2L["2"]);
G2L["1c"]["TextWrapped"] = true;
G2L["1c"]["BorderSizePixel"] = 0;
G2L["1c"]["TextSize"] = 28;
G2L["1c"]["TextScaled"] = true;
G2L["1c"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["1c"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["1c"]["TextColor3"] = Color3.fromRGB(105, 105, 105);
G2L["1c"]["BackgroundTransparency"] = 1;
G2L["1c"]["Size"] = UDim2.new(0, 200, -0.08, 50);
G2L["1c"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["1c"]["Name"] = [[LoadCount]];
G2L["1c"]["Position"] = UDim2.new(0.23958, 0, 0.76245, 0);


-- StarterGui.Trez.MainBG.Error
G2L["1d"] = Instance.new("ImageLabel", G2L["2"]);
G2L["1d"]["BorderSizePixel"] = 0;
G2L["1d"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
-- [ERROR] cannot convert ImageContent, please report to "https://github.com/uniquadev/GuiToLuaConverter/issues"
G2L["1d"]["ImageColor3"] = Color3.fromRGB(114, 114, 114);
G2L["1d"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
G2L["1d"]["Image"] = [[rbxassetid://10480493542]];
G2L["1d"]["Size"] = UDim2.new(0, 100, 0, 100);
G2L["1d"]["Visible"] = false;
G2L["1d"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["1d"]["BackgroundTransparency"] = 1;
G2L["1d"]["Name"] = [[Error]];
G2L["1d"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);


-- StarterGui.Trez.MainBG.MainAPI
G2L["1e"] = Instance.new("StringValue", G2L["2"]);
G2L["1e"]["Name"] = [[MainAPI]];


-- StarterGui.Trez.MainBG.TopBar.Toggle
local function C_7()
local script = G2L["7"];
	local children = script.Parent.Parent:GetDescendants()
	local Error = script.Parent.Parent.Error
	local loadingimage = script.Parent.Parent.Loading
	local saytext = script.Parent.Parent.LoadCount
	local foundAPI = false
	
	for i = 1, #children do
		wait(0.3)
		saytext.Text = 'Fetching '..i..'/'..#children
		local v2 = children[i]
		if v2.Name == 'MainAPI' then
			foundAPI = true
			break
		end
	end
	
	if foundAPI then
		loadingimage.Visible = false
		saytext.Visible = false
	
		local Frames = script.Parent.Parent
		local Closed = '90'
		local Opens = '-90'
		local Trigger = script.Parent.Close
		local UltimateTrigger = script.Parent.UltimateClose
		local Closeds = false
	
		local function Close(Frame:Frame)
			for i,v in pairs(Frame:GetDescendants()) do
				if v:IsA("ScrollingFrame") then
					v.Visible = false
				end
				if v:IsA("TextButton") then
					if v.Name == "Close" then
						v.Visible = true
					else
						v.Visible = false
					end
				end
			end
			Frame:TweenSize(UDim2.new(0, 384,0, 26))
			Trigger.Rotation = Opens
			Closeds = true
		end
	
		local function Open(Frame:Frame)
			Frame:TweenSize(UDim2.new(0, 384,0, 233))
			Frame:TweenPosition(UDim2.new(0.502, 0,0.5, 0))
			wait(1)
			for i,v in pairs(Frame:GetDescendants()) do
				if v:IsA("ScrollingFrame") then
					v.Visible = true
				end
				if v:IsA("TextButton") then
					v.Visible = true
				end
			end
			Trigger.Rotation = Closed
			Closeds = false
		end
		Open(Frames)
	
		Trigger.MouseButton1Click:Connect(function()
			if Closeds == false then
				Close(Frames)
			else
				Open(Frames)
			end
		end)
	
		UltimateTrigger.MouseButton1Click:Connect(function()
			Close(Frames)
			wait(0.9)
			Frames.Visible = false
			game.StarterGui:SetCore("SendNotification", {
				Title = "Settings";
				Text = "Project Trez has been closed if you want to re open it please execute Copied Code on your executor";
				Icon = "rbxassetid://224102590";
				Duration = 5; 
			})
			SetClipoard("getgenv().Vpi = true")
			if getgenv().Vpi == true then
				Frames.Visible = true
				Open(Frames)
			else
				return
			end
		end)
	else
		Error.Visible = true
		loadingimage.Visible = false
		saytext.Text = "Cant Find API! (please Use Original Source or reload this script!)"
	end
	
	
	
end;
task.spawn(C_7);
-- StarterGui.Trez.MainBG.UIDrag
local function C_d()
local script = G2L["d"];
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
task.spawn(C_d);
-- StarterGui.Trez.MainBG.Executor.Clear.LocalScript
local function C_10()
local script = G2L["10"];
	script.Parent.MouseButton1Click:Connect(function()
		getgenv().Code.Text = ""
	end)
end;
task.spawn(C_10);
-- StarterGui.Trez.MainBG.Executor.MainCodeFrame.TextBox.LocalScript
local function C_15()
local script = G2L["15"];
	local codebox = script.Parent
	local linecount = script.Parent.LineCount
	codebox:GetPropertyChangedSignal("Text"):Connect(function()
		local line = codebox.Text:split('\n')
		linecount.Text = ""
		for i = 1, #line do
			linecount.Text = linecount.Text .. i .. "\n"
		end
	end)
end;
task.spawn(C_15);
-- StarterGui.Trez.MainBG.Executor.MainCodeFrame.TextBox.LocalScript
local function C_16()
local script = G2L["16"];
	getgenv().Code = script.Parent
end;
task.spawn(C_16);
-- StarterGui.Trez.MainBG.Executor.Execute.LocalScript
local function C_19()
local script = G2L["19"];
	script.Parent.MouseButton1Click:Connect(function()
		pcall(function()
			loadstring(getgenv().Code.Text)()
		end)
	end)
	
end;
task.spawn(C_19);
-- StarterGui.Trez.MainBG.Loading.LocalScript
local function C_1b()
local script = G2L["1b"];
	while wait() do
		script.Parent.Rotation += 5
	end
end;
task.spawn(C_1b);

return G2L["1"], require;
