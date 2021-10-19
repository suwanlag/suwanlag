game:GetService("StarterGui"):SetCore("SendNotification", {
  Title = "ShellXHubV2 v1.0.3",
  Text = "thank for using ShellXhubV2"
})
wait(1)
game:GetService("StarterGui"):SetCore("SendNotification", {
  Title = "ShellXHubV2 v1.0.3",
  Text = "PlsWait10Second"
})
wait(10)
local Venyx = loadstring(game:HttpGet("https://raw.githubusercontent.com/Stefanuk12/Venyx-UI-Library/main/source2.lua"))()
local UI = Venyx.new({
    title = "Shell X Hub V2 - 1.0.3"
})

-- // Themes
local Themes =  {
    Background = Color3.fromRGB(24, 24, 24),
    Glow = Color3.fromRGB(0, 0, 0),
    Accent = Color3.fromRGB(10, 10, 10),
    LightContrast = Color3.fromRGB(20, 20, 20),
    DarkContrast = Color3.fromRGB(14, 14, 14),  
    TextColor = Color3.fromRGB(255, 255, 255)
}

-- // Test Page
local Test = UI:addPage({
    title = "Main",
    icon = 5012544693
})

-- // Sections for Test Page
local SectionA = Test:addSection({
    title = "MainAutofarm"
})
local SectionB = Test:addSection({
    title = "CommingSoon.."
})

-- // Section A UI Elements
SectionA:addToggle({
    title = "AutoFarmBeta2",
    callback = function(value)
        loadstring(game:HttpGet("https://raw.githubusercontent.com/suwanlag/AutoFarm/main/README.md"))()
    end
})

-- // Section D UI Elements
local Test = UI:addPage({
    title = "Teleport",
    icon = 5012544693
})

local SectionD = Test:addSection({
    title = "Teleport"
})

SectionD:addButton({
    title = "Ctrl + Click = TP",
    callback = function()
        local Plr = game:GetService("Players").LocalPlayer
local Mouse = Plr:GetMouse()
 
Mouse.Button1Down:connect(
    function()
        if not game:GetService("UserInputService"):IsKeyDown(Enum.KeyCode.LeftControl) then
            return
        end
        if not Mouse.Target then
            return
        end
        Plr.Character:MoveTo(Mouse.Hit.p)
    end
)
    end
})

SectionD:addButton({
    title = "Starterland",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(946.396484, 16.5166149, 1428.54102, -0.0332927071, -4.42573764e-08, 0.999445617, -4.84113132e-11, 1, 4.42803092e-08, -0.999445617, 1.42582701e-09, -0.0332927071)
    end
})

SectionD:addButton({
    title = "MiddleTown",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-698.071655, 7.85224533, 1559.16711, 0.971976697, 3.74573865e-08, 0.235077143, -4.1371532e-08, 1, 1.17186092e-08, -0.235077143, -2.11157172e-08, 0.971976697)
    end
})

SectionD:addButton({
    title = "Jungle",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1324.81079, 11.8530645, 492.504089, -0.950561523, 0, -0.310536355, 0, 1, 0, 0.310536355, 0, -0.950561523)
    end
})

SectionD:addButton({
    title = "Desert",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(909.186157, 6.5132513, 4380.58252, -0.979714632, -1.68406054e-08, 0.2003977, -9.15892709e-11, 1, 8.35881551e-08, -0.2003977, 8.18741839e-08, -0.979714632)
    end
})

SectionD:addButton({
    title = "Snowisland",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1390.01794, 87.272789, -1347.60876, -0.199600711, -3.93440693e-08, -0.979877293, 1.92018632e-08, 1, -4.40634516e-08, 0.979877293, -2.76105663e-08, -0.199600711)
    end
})

SectionD:addButton({
    title = "Marineford",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4818.64404, 20.6519604, 4371.78076, 0.853140891, 0, -0.521680713, 0, 1, 0, 0.521680713, 0, 0.853140891)
    end
})

SectionD:addButton({
    title = "Skypiea1",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4695.72168, 845.277161, -1849.30481, 0.942552745, 0, 0.33405903, 0, 1, 0, -0.33405903, 0, 0.942552745)
    end
})

SectionD:addButton({
    title = "Skypiea2",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-7887.83545, 5545.49316, -380.958527, -0.000477724156, -6.86372985e-08, -0.999999881, 5.76642201e-08, 1, -6.86648534e-08, 0.999999881, -5.76970152e-08, -0.000477724156)
    end
})

SectionD:addButton({
    title = "Prison",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5009.61572, 3.65196347, 739.075989, -0.00479308004, 9.31296569e-08, 0.999988496, 5.43943734e-08, 1, -9.28700103e-08, -0.999988496, 5.39486145e-08, -0.00479308004)
    end
})

SectionD:addButton({
    title = "Colosseum",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1477.56165, 7.38933945, -2937.54102, 0.748681664, -4.16919406e-08, 0.662929654, -1.05962474e-08, 1, 7.4857347e-08, -0.662929654, -6.30688533e-08, 0.748681664)
    end
})

SectionD:addButton({
    title = "Magma Village",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-5254.56592, 8.59067631, 8451.16797, -0.356155008, 7.88511798e-08, 0.934427261, 7.19219528e-08, 1, -5.69715759e-08, -0.934427261, 4.69150905e-08, -0.356155008)
    end
})

SectionD:addButton({
    title = "Fishman island",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(61352.3828, 18.8707905, 1502.90942, -0.999073625, 2.99610892e-09, -0.043031659, 3.08991832e-09, 1, -2.11348894e-09, 0.043031659, -2.24449526e-09, -0.999073625)
    end
})

SectionD:addButton({
    title = "Fountain city",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5072.36914, 4.50129032, 4158.08545, 0.574859381, 0, 0.818252444, 0, 1, 0, -0.818252623, 0, 0.57485944)
    end
})
-- // Section F UI Elements
local Test = UI:addPage({
    title = "Players",
    icon = 5012544693
})

local SectionD = Test:addSection({
    title = "Players"
})

SectionD:addButton({
    title = "OpenTeleportPlayers",
    callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/KnamzuVk"))()
    end
})

SectionD:addButton({
    title = "Spectage",
    callback = function()
        --Made by N3xul
local runDummyScript = function(f,scri)
local oldenv = getfenv(f)
local newenv = setmetatable({}, {
__index = function(_, k)
if k:lower() == 'script' then
return scri
else
return oldenv[k]
end
end
})
setfenv(f, newenv)
ypcall(function() f() end)
end
cors = {}
mas = Instance.new("Model",game:GetService("Lighting")) 
mas.Name = "CompiledModel"
o1 = Instance.new("ScreenGui")
o2 = Instance.new("Frame")
o3 = Instance.new("TextButton")
o4 = Instance.new("TextButton")
o5 = Instance.new("TextLabel")
o6 = Instance.new("ImageButton")
o7 = Instance.new("LocalScript")
o1.Name = "SpectateGui"
o1.Parent = mas
o2.Name = "Bar"
o2.Parent = o1
o2.Position = UDim2.new(-1,-100,0.87999999523163,-50)
o2.Size = UDim2.new(0,200,0,50)
o2.Position = UDim2.new(-1,-100,0.87999999523163,-50)
o2.BackgroundColor3 = Color3.new(0, 0, 0)
o2.BackgroundTransparency = 0.20000000298023
o2.BorderSizePixel = 5
o3.Name = "Previous"
o3.Parent = o2
o3.Size = UDim2.new(0.25,0,1,0)
o3.Text = "<"
o3.BackgroundColor3 = Color3.new(0.52549, 0.52549, 0.52549)
o3.BorderColor3 = Color3.new(0.509804, 0.796079, 1)
o3.BorderSizePixel = 0
o3.Font = Enum.Font.SourceSans
o3.FontSize = Enum.FontSize.Size48
o3.TextColor3 = Color3.new(1, 1, 1)
o4.Name = "Next"
o4.Parent = o2
o4.Position = UDim2.new(1,0,0,0)
o4.Size = UDim2.new(-0.25,0,1,0)
o4.Text = ">"
o4.Position = UDim2.new(1,0,0,0)
o4.BackgroundColor3 = Color3.new(0.52549, 0.52549, 0.52549)
o4.BorderColor3 = Color3.new(0.509804, 0.796079, 1)
o4.BorderSizePixel = 0
o4.Font = Enum.Font.SourceSans
o4.FontSize = Enum.FontSize.Size48
o4.TextColor3 = Color3.new(1, 1, 1)
o5.Name = "Title"
o5.Parent = o2
o5.Position = UDim2.new(0.27500000596046,0,0,0)
o5.Size = UDim2.new(0.44999998807907,0,1,0)
o5.Text = ""
o5.Position = UDim2.new(0.27500000596046,0,0,0)
o5.BackgroundColor3 = Color3.new(1, 1, 1)
o5.BackgroundTransparency = 1
o5.Font = Enum.Font.SourceSans
o5.FontSize = Enum.FontSize.Size14
o5.TextColor3 = Color3.new(1, 1, 1)
o5.TextScaled = true
o5.TextWrapped = true
o6.Name = "Button"
o6.Parent = o1
o6.Position = UDim2.new(0,0,0.5,-25)
o6.Size = UDim2.new(0,50,0,50)
o6.Position = UDim2.new(0,0,0.5,-25)
o6.BackgroundColor3 = Color3.new(1, 1, 1)
o6.BackgroundTransparency = 0.30000001192093
o6.BorderSizePixel = 5
o6.Image = "http://www.roblox.com/asset/?id=176106970"
o7.Parent = o1
table.insert(cors,coroutine.create(function()
wait()
runDummyScript(function()
-- By super10099

cam = game.Workspace.CurrentCamera

local bar = script.Parent.Bar
local title = bar.Title
local prev = bar.Previous
local nex = bar.Next
local button = script.Parent.Button

function get()
	for _,v in pairs(game.Players:GetPlayers())do
		if v.Name == title.Text then
			return(_)
		end
	end
end


local debounce = false
button.MouseButton1Click:connect(function()
	if debounce == false then debounce = true
		bar:TweenPosition(UDim2.new(.5,-100,0.88,-50),"In","Linear",1,true)
		pcall(function()
				title.Text = game.Players:GetPlayerFromCharacter(cam.CameraSubject.Parent).Name
		end)
	elseif debounce == true then debounce = false
		pcall(function() cam.CameraSubject = game.Players.LocalPlayer.Character.Humanoid end)
			bar:TweenPosition(UDim2.new(-1,-100,0.88,-50),"In","Linear",1,true)
		end
end)

prev.MouseButton1Click:connect(function()
	wait(.1)
	local players = game.Players:GetPlayers()
	local num = get()
	if not pcall(function() 
		cam.CameraSubject = players[num-1].Character.Humanoid
		end) then
		cam.CameraSubject = players[#players].Character.Humanoid
	end
pcall(function()
				title.Text = game.Players:GetPlayerFromCharacter(cam.CameraSubject.Parent).Name
		end)
end)

nex.MouseButton1Click:connect(function()
	wait(.1)
	local players = game.Players:GetPlayers()
	local num = get()
	if not pcall(function() 
		cam.CameraSubject = players[num+1].Character.Humanoid
		end) then
		cam.CameraSubject = players[1].Character.Humanoid
	end
pcall(function()
				title.Text = game.Players:GetPlayerFromCharacter(cam.CameraSubject.Parent).Name
		end)
end)


end,o7)
end))
mas.Parent = workspace
mas:MakeJoints()
local mas1 = mas:GetChildren()
for i=1,#mas1 do
	mas1[i].Parent = game:GetService("Players").LocalPlayer.PlayerGui 
	ypcall(function() mas1[i]:MakeJoints() end)
end
mas:Destroy()
for i=1,#cors do
coroutine.resume(cors[i])
end
    end
})

SectionD:addButton({
    title = "Teleport all players to me.",
    callback = function()
       local plr = game:GetService("Players").LocalPlayer
for i,v in pairs(game:GetService("Players"):GetChildren()) do
    if v.ClassName == "Player" and v.Name ~= plr.Name then
        if v.Character:FindFirstChild("HumanoidRootPart") then
            v.Character.HumanoidRootPart.CFrame = CFrame.new(plr.Character.HumanoidRootPart.Position)
        end
    end
end
    end
})

SectionD:addButton({
    title = "Aimbot Gun",
    callback = function()
        game:GetService("StarterGui"):SetCore("SendNotification", {
  Title = "AIMBOT PASS2",
  Text = "Press L.Ctrl"
})

game:GetService("StarterGui"):SetCore("SendNotification", {
  Title = "ESP NAME",
  Text = "Press L.Alt"
})


PLAYER  = game.Players.LocalPlayer
MOUSE   = PLAYER:GetMouse()
CC      = game.Workspace.CurrentCamera

ENABLED      = false
ESP_ENABLED  = false

_G.FREE_FOR_ALL = true

_G.BIND        = 50
_G.ESP_BIND    = 52
_G.CHANGE_AIM  = 'gfdkdfvdgfdgccv'

_G.AIM_AT = 'Head'

wait(1)

function GetNearestPlayerToMouse()
	local PLAYERS      = {}
	local PLAYER_HOLD  = {}
	local DISTANCES    = {}
	for i, v in pairs(game.Players:GetPlayers()) do
		if v ~= PLAYER then
			table.insert(PLAYERS, v)
		end
	end
	for i, v in pairs(PLAYERS) do
		if _G.FREE_FOR_ALL == false then
			if v and (v.Character) ~= nil and v.TeamColor ~= PLAYER.TeamColor then
				local AIM = v.Character:FindFirstChild(_G.AIM_AT)
				if AIM ~= nil then
					local DISTANCE                 = (AIM.Position - game.Workspace.CurrentCamera.CoordinateFrame.p).magnitude
					local RAY                      = Ray.new(game.Workspace.CurrentCamera.CoordinateFrame.p, (MOUSE.Hit.p - CC.CoordinateFrame.p).unit * DISTANCE)
					local HIT,POS                  = game.Workspace:FindPartOnRay(RAY, game.Workspace)
					local DIFF                     = math.floor((POS - AIM.Position).magnitude)
					PLAYER_HOLD[v.Name .. i]       = {}
					PLAYER_HOLD[v.Name .. i].dist  = DISTANCE
					PLAYER_HOLD[v.Name .. i].plr   = v
					PLAYER_HOLD[v.Name .. i].diff  = DIFF
					table.insert(DISTANCES, DIFF)
				end
			end
		elseif _G.FREE_FOR_ALL == true then
			local AIM = v.Character:FindFirstChild(_G.AIM_AT)
			if AIM ~= nil then
				local DISTANCE                 = (AIM.Position - game.Workspace.CurrentCamera.CoordinateFrame.p).magnitude
				local RAY                      = Ray.new(game.Workspace.CurrentCamera.CoordinateFrame.p, (MOUSE.Hit.p - CC.CoordinateFrame.p).unit * DISTANCE)
				local HIT,POS                  = game.Workspace:FindPartOnRay(RAY, game.Workspace)
				local DIFF                     = math.floor((POS - AIM.Position).magnitude)
				PLAYER_HOLD[v.Name .. i]       = {}
				PLAYER_HOLD[v.Name .. i].dist  = DISTANCE
				PLAYER_HOLD[v.Name .. i].plr   = v
				PLAYER_HOLD[v.Name .. i].diff  = DIFF
				table.insert(DISTANCES, DIFF)
			end
		end
	end
	
	if unpack(DISTANCES) == nil then
		return false
	end
	
	local L_DISTANCE = math.floor(math.min(unpack(DISTANCES)))
	if L_DISTANCE > 20 then
		return false
	end
	
	for i, v in pairs(PLAYER_HOLD) do
		if v.diff == L_DISTANCE then
			return v.plr
		end
	end
	return false
end

GUI_MAIN                           = Instance.new('ScreenGui', game.CoreGui)
GUI_TARGET                         = Instance.new('TextLabel', GUI_MAIN)
GUI_AIM_AT                         = Instance.new('TextLabel', GUI_MAIN)

GUI_MAIN.Name                      = 'AIMBOT'

GUI_TARGET.Size                    = UDim2.new(0,200,0,30)
GUI_TARGET.BackgroundTransparency  = 0.5
GUI_TARGET.BackgroundColor         = BrickColor.new('Fossil')
GUI_TARGET.BorderSizePixel         = 0
GUI_TARGET.Position                = UDim2.new(0.5,-100,0,0)
GUI_TARGET.Text                    = 'AIMBOT : OFF'
GUI_TARGET.TextColor3              = Color3.new(1,1,1)
GUI_TARGET.TextStrokeTransparency  = 1
GUI_TARGET.TextWrapped             = true
GUI_TARGET.FontSize                = 'Size24'
GUI_TARGET.Font                    = 'SourceSansBold'

GUI_AIM_AT.Size                    = UDim2.new(0,200,0,20)
GUI_AIM_AT.BackgroundTransparency  = 0.5
GUI_AIM_AT.BackgroundColor         = BrickColor.new('Fossil')
GUI_AIM_AT.BorderSizePixel         = 0
GUI_AIM_AT.Position                = UDim2.new(0.5,-100,0,30)
GUI_AIM_AT.Text                    = 'AIMING : HEAD'
GUI_AIM_AT.TextColor3              = Color3.new(1,1,1)
GUI_AIM_AT.TextStrokeTransparency  = 1
GUI_AIM_AT.TextWrapped             = true
GUI_AIM_AT.FontSize                = 'Size18'
GUI_AIM_AT.Font                    = 'SourceSansBold'

local TRACK = false

function CREATE(BASE, TEAM)
	local ESP_MAIN                   = Instance.new('BillboardGui', PLAYER.PlayerGui)
	local ESP_DOT                    = Instance.new('Frame', ESP_MAIN)
	local ESP_NAME                   = Instance.new('TextLabel', ESP_MAIN)
	
	ESP_MAIN.Name                    = 'ESP'
	ESP_MAIN.Adornee                 = BASE
	ESP_MAIN.AlwaysOnTop             = true
	ESP_MAIN.ExtentsOffset           = Vector3.new(0, 1, 0)
	ESP_MAIN.Size                    = UDim2.new(0, 5, 0, 5)
	
	ESP_DOT.Name                     = 'DOT'
	ESP_DOT.BackgroundColor          = BrickColor.new('Bright red')
	ESP_DOT.BackgroundTransparency   = 0.3
	ESP_DOT.BorderSizePixel          = 0
	ESP_DOT.Position                 = UDim2.new(-0.5, 0, -0.5, 0)
	ESP_DOT.Size                     = UDim2.new(2, 0, 2, 0)
	ESP_DOT.Visible                  = true
	ESP_DOT.ZIndex                   = 10
	
	ESP_NAME.Name                    = 'NAME'
	ESP_NAME.BackgroundColor3        = Color3.new(255, 255, 255)
	ESP_NAME.BackgroundTransparency  = 1
	ESP_NAME.BorderSizePixel         = 0
	ESP_NAME.Position                = UDim2.new(0, 0, 0, -40)
	ESP_NAME.Size                    = UDim2.new(1, 0, 10, 0)
	ESP_NAME.Visible                 = true
	ESP_NAME.ZIndex                  = 10
	ESP_NAME.Font                    = 'ArialBold'
	ESP_NAME.FontSize                = 'Size14'
	ESP_NAME.Text                    = BASE.Parent.Name:upper()
	ESP_NAME.TextColor               = BrickColor.new('Bright red')
end

function CLEAR()
	for _,v in pairs(PLAYER.PlayerGui:children()) do
		if v.Name == 'ESP' and v:IsA('BillboardGui') then
			v:Destroy()
		end
	end
end

function FIND()
	CLEAR()
	TRACK = true
	spawn(function()
		while wait() do
			if TRACK then
				CLEAR()
				for i,v in pairs(game.Players:GetChildren()) do
					if v.Character and v.Character:FindFirstChild('Head') then
						if _G.FREE_FOR_ALL == false then
							if v.TeamColor ~= PLAYER.TeamColor then
								if v.Character:FindFirstChild('Head') then
									CREATE(v.Character.Head, true)
								end
							end
						else
							if v.Character:FindFirstChild('Head') then
								CREATE(v.Character.Head, true)
							end
						end
					end
				end
			end
		end
		wait(1)
	end)
end

MOUSE.KeyDown:connect(function(KEY)
	KEY = KEY:lower():byte()
	if KEY == _G.BIND then
		ENABLED = true
	end
end)

MOUSE.KeyUp:connect(function(KEY)
	KEY = KEY:lower():byte()
	if KEY == _G.BIND then
		ENABLED = false
	end
end)

MOUSE.KeyDown:connect(function(KEY)
	KEY = KEY:lower():byte()
	if KEY == _G.ESP_BIND then
		if ESP_ENABLED == false then
			FIND()
			ESP_ENABLED = true
			print('ESP : ON')
		elseif ESP_ENABLED == true then
			wait()
			CLEAR()
			TRACK = false
			ESP_ENABLED = false
			print('ESP : OFF')
		end
	end
end)

MOUSE.KeyDown:connect(function(KEY)
	if KEY == _G.CHANGE_AIM then
		if _G.AIM_AT == 'Head' then
			_G.AIM_AT = 'Torso'
			GUI_AIM_AT.Text = 'AIMING : TORSO'
		elseif _G.AIM_AT == 'Torso' then
			_G.AIM_AT = 'Head'
			GUI_AIM_AT.Text = 'AIMING : HEAD'
		end
	end
end)

game:GetService('RunService').RenderStepped:connect(function()
	if ENABLED then
		local TARGET = GetNearestPlayerToMouse()
		if (TARGET ~= false) then
			local AIM = TARGET.Character:FindFirstChild(_G.AIM_AT)
			if AIM then
				CC.CoordinateFrame = CFrame.new(CC.CoordinateFrame.p, AIM.CFrame.p)
			end
			GUI_TARGET.Text = 'AIMBOT : '.. TARGET.Name:sub(1, 5)
		else
			GUI_TARGET.Text = 'AIMBOT : OFF'
		end
	end
end)

repeat
	wait()
	if ESP_ENABLED == true then
		FIND()
	end
until ESP_ENABLED == false
    end
})

SectionD:addButton({
    title = "BountyFarmAndOpenAutoClick",
    callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/Lr8Enx7Z"))()
    end
})

local Test = UI:addPage({
    title = "Game",
    icon = 5012544693
})

local SectionD = Test:addSection({
    title = "Graphics"
})

SectionD:addButton({
    title = "RTXMODE",
    callback = function()
        getgenv().mode = "Summer" -- Choose from Summer and Autumn




local a = game.Lighting
a.Ambient = Color3.fromRGB(33, 33, 33)
a.Brightness = 6.67
a.ColorShift_Bottom = Color3.fromRGB(0, 0, 0)
a.ColorShift_Top = Color3.fromRGB(255, 247, 237)
a.EnvironmentDiffuseScale = 0.105
a.EnvironmentSpecularScale = 0.522
a.GlobalShadows = true
a.OutdoorAmbient = Color3.fromRGB(51, 54, 67)
a.ShadowSoftness = 0.04
a.GeographicLatitude = -15.525
a.ExposureCompensation = 0.75
local b = Instance.new("BloomEffect", a)
b.Enabled = true
b.Intensity = 0.04
b.Size = 1900
b.Threshold = 0.915
local c = Instance.new("ColorCorrectionEffect", a)
c.Brightness = 0.176
c.Contrast = 0.39
c.Enabled = true
c.Saturation = 0.2
c.TintColor = Color3.fromRGB(217, 145, 57)
if getgenv().mode == "Summer" then
   c.TintColor = Color3.fromRGB(255, 220, 148)
elseif getgenv().mode == "Autumn" then
   c.TintColor = Color3.fromRGB(217, 145, 57)
else
   warn("No mode selected!")
   print("Please select a mode")
   b:Destroy()
   c:Destroy()
end
local d = Instance.new("DepthOfFieldEffect", a)
d.Enabled = true
d.FarIntensity = 0.077
d.FocusDistance = 21.54
d.InFocusRadius = 20.77
d.NearIntensity = 0.277
local e = Instance.new("ColorCorrectionEffect", a)
e.Brightness = 0
e.Contrast = -0.07
e.Saturation = 0
e.Enabled = true
e.TintColor = Color3.fromRGB(255, 247, 239)
local e2 = Instance.new("ColorCorrectionEffect", a)
e2.Brightness = 0.2
e2.Contrast = 0.45
e2.Saturation = -0.1
e2.Enabled = true
e2.TintColor = Color3.fromRGB(255, 255, 255)
local s = Instance.new("SunRaysEffect", a)
s.Enabled = true
s.Intensity = 0.01
s.Spread = 0.146

print("RTX Graphics loaded \n created by Rawget#0001")
    end
})

SectionD:addButton({
    title = "BetterMODE",
    callback = function()
        local g = game 
local w = g.Workspace
local l = g.Lighting
local t = w.Terrain
local sr = Instance.new("SunRaysEffect",l)
sr.Intensity = 0.075
sr.Spread = 0.01
local df = Instance.new("DepthOfFieldEffect",l)
df.FarIntensity = 0.01
l.GlobalShadows = true
l.Brightness = 0.7
l.ClockTime = 13.5
l.GeographicLatitude = 45
l.TimeOfDay = 16
sethiddenproperty(l,"Technology",4)
sethiddenproperty(l,"ShadowSoftness",1)
sethiddenproperty(t,"Decoration",true)
    end
})

SectionD:addButton({
    title = "EnhancedMODE",
    callback = function()
        -- Script made by Harryboharps
-- Shoutout to Claude

bloom = Instance.new("BloomEffect",game.Lighting) -- BLOOM Properties
bloom.Intensity = 1
bloom.Size = 56
bloom.Threshold = 0.5

blur = Instance.new("BlurEffect",game.Lighting) -- BLUR Properties
blur.Size = 5

color = Instance.new("ColorCorrectionEffect",game.Ligting) -- COLORCORRECTION Properties
color.TintColor = Color3.fromRGB(216,216,216)

rays = Instance.new("SunRaysEffect",game.Lighting) -- SUNRAYS Properties
rays.Intensity = 0.25
rays.Spread = 1

print("Shoutout to my cousin ben.")
    end
})



local SectionD = Test:addSection({
    title = "ESP"
})

SectionD:addButton({
    title = "Players Esp",
    callback = function()
        -- by slice
local MainParent = game.workspace.Terrain or nil
local LineFrame = Instance.new("ScreenGui",MainParent)
LineFrame.Name = "Lines"
LineFrame.Enabled = false
ToggleKey = Enum.KeyCode.F1
local Spotted = {};
local CharacterMotors = {}
CharacterMotors.GetMotors = function(char)
	local Motors = {}
		for i,v in pairs(char:GetDescendants()) do
			if v:IsA("Motor6D") then
				if v.Part0 and v.Part1 then--and v.Part0.Name ~= "HumanoidRootPart" and v.Part1.Name ~= "HumanoidRootPart" then
					table.insert(Motors,{v.Part0,v.Part1})
				end
			end
		end
	table.insert(Motors,{char:FindFirstChild("Head") or char.PrimaryPart,"Camera"})
	CharacterMotors[char] = Motors
	return CharacterMotors[char]
end
		
lerp = function(a, b, t)
	return a + (b - a) * t
end

local ESP = {Characters = {}}
ESP.Visible = true
ESP.Init = function(char,plr)
	--if (game:GetService("Players").LocalPlayer.Team == nil or plr.Team ~= game:GetService("Players").LocalPlayer.Team) then
		char.DescendantAdded:Connect(function()
			CharacterMotors.GetMotors(char)
		end)
		
		local BillboardUi = Instance.new("BillboardGui")
		BillboardUi.AlwaysOnTop = true
		BillboardUi.Size = UDim2.new(3,60,1,30)
		BillboardUi.StudsOffsetWorldSpace = Vector3.new(0,-4.5,0)
		BillboardUi.Adornee = char:WaitForChild("HumanoidRootPart")
		
		local PlayerName = Instance.new("TextLabel",BillboardUi)
		PlayerName.BackgroundTransparency = 1
		PlayerName.TextColor3 = (game:GetService("Players"):GetPlayerFromCharacter(char)).TeamColor.Color
		PlayerName.Size = UDim2.new(1,0,.3,0)
		PlayerName.ZIndex = 2
		PlayerName.Text = char.Name
		PlayerName.TextScaled = true
		PlayerName.TextStrokeTransparency = .25
		PlayerName.Font = Enum.Font.GothamBold
		PlayerName.TextStrokeColor3 = Color3.fromRGB(33, 33, 33)
		
		local Distance = PlayerName:Clone()
		Distance.Parent = BillboardUi
		Distance.Font = Enum.Font.Gotham
		Distance.TextColor3 = Color3.new(1,1,1)
		Distance.Position = UDim2.new(0,0,.3,0)
		
		local Health = PlayerName:Clone()
		Health.Parent = BillboardUi
		Health.Font = Enum.Font.Gotham
		Health.Position = UDim2.new(0,0,.6,0)
		
		ESP.Characters[char] = {PlayerName,Distance,Health,BillboardUi}
	--end
end
ESP.Render = function()
	
	for i,v in pairs(ESP.Characters) do
		pcall(function()
			local shrink = ((((game.Workspace.CurrentCamera.CFrame.p) - i.HumanoidRootPart.Position).Magnitude)/1500)+1
			v[2].Text = math.floor(((game.Workspace.CurrentCamera.CFrame.p) - i.HumanoidRootPart.Position).Magnitude+.5)
			v[3].Text = math.floor(i.Humanoid.Health).."/"..i.Humanoid.MaxHealth.." - "..math.floor(((i.Humanoid.Health/i.Humanoid.MaxHealth)*100)+.5).."%"
			v[3].TextColor3 = Color3.fromHSV((i.Humanoid.Health/i.Humanoid.MaxHealth) * (80/255),1,1)
			if not Spotted[i] then
				--v[1].TextTransparency = lerp(v[1].TextTransparency,.6,0.05)
			else
				--v[1].TextTransparency = lerp(v[1].TextTransparency,0,0.1)
			end
			v[1].TextColor3 = (game:GetService("Players"):GetPlayerFromCharacter(i)).TeamColor.Color
			--v[1].TextStrokeTransparency = 1-((1-v[1].TextTransparency)/2)
			--v[2].TextTransparency = v[1].TextTransparency
			--v[2].TextStrokeTransparency = v[1].TextStrokeTransparency
			--v[3].TextTransparency = v[1].TextTransparency
			--v[3].TextStrokeTransparency = v[1].TextStrokeTransparency
			v[4].Size = UDim2.new(3,60/shrink,1,30/shrink)
			v[1].Visible = ESP.Visible
			v[2].Visible = ESP.Visible
			v[3].Visible = ESP.Visible
			v[4].Parent = MainParent
			
		end)
	end
	
end

local Perspective = {}
Perspective.CalculatePoint = function(position,cam)
	local vector, onScreen = cam:WorldToScreenPoint(position)
	return Vector2.new(vector.X, vector.Y),vector.Z,onScreen
end

local Draw = {UsedLines = {}}
Draw.Line = function(a,b,line,width)
	if a and b then	
		local lerp = a:Lerp(b,.5)
		local Magnitude = (a-b).Magnitude
		line.AnchorPoint = Vector2.new(0.5,.5)
		line.Position = UDim2.new(lerp.X/game.Workspace.CurrentCamera.ViewportSize.X,0,(lerp.Y/(game.Workspace.CurrentCamera.ViewportSize.Y-36)),36/2)
		line.Size = UDim2.new(Magnitude/line.Parent.AbsoluteSize.X,0,0,width)
		line.Rotation = math.deg(math.atan2(a.y - b.y, a.x - b.x))
	else
		line:Destroy()
	end
end


Draw.Character = function(player,lines,cam)
	local Motors = CharacterMotors[player]
	if not Motors then
		Motors = CharacterMotors.GetMotors(player)
	end

	for i,v in pairs(Motors) do
		if v[1] and v[2] then
			local FoundLine = nil
			for i,v in pairs(lines:GetChildren()) do
				if Draw.UsedLines[v] == nil then
					Draw.UsedLines[v] = true
					FoundLine = v
					break
				end
			end
			local a2d,az,screen = Perspective.CalculatePoint(v[1].Position,cam)
			local b2d,bz,screen2
			local v2pos = v[2].Position
			Spotted[player] = false
			if v[2] == "Camera" then
				local ray = Ray.new(v[1].Position, (cam.CFrame.p - v[1].Position).unit * (cam.CFrame.p - v[1].Position).Magnitude)
				local part, position = workspace:FindPartOnRayWithIgnoreList(ray, {game:GetService("Players").LocalPlayer.Character,player}, false, true)
				if part then
					screen = false
					screen2 = false
				else
					Spotted[player] = true
					b2d,bz,screen2 = Vector2.new(cam.ViewportSize.x/2, cam.ViewportSize.y),0,true	
					screen = true
				end
				v2pos = v[1].Position
			else
				b2d,bz,screen2 = Perspective.CalculatePoint(v[2].Position,cam)	
			end
			if screen and screen2 and (v[1].Position-v2pos).Magnitude <= 5 then
				if not FoundLine then
					FoundLine = Instance.new("Frame")
					FoundLine.BackgroundColor3 = Color3.new(1,1,1)
					FoundLine.BackgroundTransparency = .25
					FoundLine.BorderSizePixel = 0
					FoundLine.Parent = lines	
					Draw.UsedLines[FoundLine] = true
				end
				if screen then
					Draw.Line(a2d,b2d,FoundLine,1)
				else
					Draw.Line(b2d,a2d,FoundLine,1)
				end
			elseif FoundLine then
				FoundLine:Destroy()
			end
		end
	end
end

Draw.ResetLines = function(lines)
	for i,v in pairs(lines:GetChildren()) do
		if Draw.UsedLines[v] == nil then
			v:Destroy()
		end
	end
	Draw.UsedLines = {}
end

local AddPlayer = function(plr)
	coroutine.resume(coroutine.create(function()
		if plr ~= game:GetService("Players").LocalPlayer  then
			if plr.Character then
				ESP.Init(plr.Character,plr)
			end
			plr.CharacterAdded:Connect(function(cha)
				ESP.Init(cha,plr)
			end)
		end
	end))
end

for i,v in pairs(game:GetService("Players"):GetChildren()) do
	AddPlayer(v)
end
game:GetService("Players").PlayerAdded:Connect(function(v)
	AddPlayer(v)
end)
game:GetService("UserInputService").InputBegan:connect(function(inputObject)
	if inputObject.KeyCode == ToggleKey then
		ESP.Visible = not ESP.Visible
	end
end)
game:GetService("RunService").RenderStepped:Connect(function()
	ESP.Render()
	for i,v in pairs(game:GetService("Players"):GetChildren()) do
		if v.Character and v ~= game:GetService("Players").LocalPlayer and (game:GetService("Players").LocalPlayer.Team == nil or v.Team ~= game:GetService("Players").LocalPlayer.Team) then
			if v.Character.PrimaryPart and (v.Character.PrimaryPart.Position - game.Workspace.CurrentCamera.CFrame.Position).Magnitude <= 200 then
				Draw.Character(v.Character,LineFrame,game.Workspace.CurrentCamera)
			end
		end
	end
	Draw.ResetLines(LineFrame)
end)
    end
})


local SectionD = Test:addSection({
    title = "Npcteleport"
})

SectionD:addButton({
    title = "Blackleg",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-987.23175, 13.7520361, 3989.80298, -0.272060424, -7.10997128e-09, -0.962280095, -8.50117921e-10, 1, -7.14832105e-09, 0.962280095, -1.12672338e-09, -0.272060424)
    end
})

SectionD:addButton({
    title = "Electro",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-5387.12012, 13.5180063, -2147.54541, 0.166960597, 1.33693021e-08, -0.985963345, 2.98132008e-08, 1, 1.86081266e-08, 0.985963345, -3.25015534e-08, 0.166960597)
    end
})

SectionD:addButton({
    title = "FishMan",
    callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(61583.3281, 18.8707886, 986.646545, -0.00245730928, -5.70202374e-08, -0.999997139, -1.9176398e-10, 1, -5.70199425e-08, 0.999997139, 5.16460208e-11, -0.00245730928)
    end
})

local SectionD = Test:addSection({
    title = "OpenBuyCombat"
})
SectionD:addButton({
    title = "Open",
    callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/faviTs7z"))()
    end
})

local SectionD = Test:addSection({
    title = "Bring"
})


SectionD:addButton({
    title = "BringChest",
    callback = function()
        local ll__SHARK_X_HUB__ll = "SHARK X HUB | MOOD#999" local ll__lIllIllIl__ll = game.Players.LocalPlayer if #ll__SHARK_X_HUB__ll == 22 then local ll__lIIlIIlllIl__ll = "SHARK X HUB NO 1" _G.ll__lIllI__ll = true local p = true local ll__lIllIlllIllIl__ll = {[1] = "SetTeam", [2] = "Pirates"} game:GetService("ReplicatedStorage").Remotes.CommF:InvokeServer(unpack(ll__lIllIlllIllIl__ll)) _G.ll__lIllIll__ll = true while _G.ll__lIllIll__ll do pcall(function() if game:GetService("Players").LocalPlayer.Data.Beli.Value >= 25000 then _G.ll__lIllI__ll = false  local ll__lIIlIIlllIl__ll = "HIW KAO WA I SUD" game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin", "Check") game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin", "Buy") end end ) wait() local ll_lIIlIIllIll_ll = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame local ll_lIIlIll_ll = game.Workspace:GetChildren() for i = 1, #ll_lIIlIll_ll do if ll_lIIlIll_ll[i].Name:lower():match("chest") then ll__lIllIl__ll = false repeat wait() if ll_lIIlIll_ll[i].Parent ~= game.Workspace then ll__lIllIl__ll = true else pcall( function()  local ll__lIIlIIlllIl__ll = "YOUR MOTHER SUCK MY DICK!" if game:GetService("Players").LocalPlayer.Data.Beli.Value >= 25000 then _G.ll__lIllI__ll = false game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin", "Check") game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin", "Buy") local ll__IlIlIIIllllIIl__ll = 0.4 function ll__lIIlIlllIllIlllIllIL__ll(ll__IllIllIIIlIl__ll) if game.Players.LocalPlayer.Backpack:FindFirstChild(ll__IllIllIIIlIl__ll) then local ll__IIIlIIllIl__ll = game.Players.LocalPlayer.Backpack:FindFirstChild(ll__IllIllIIIlIl__ll) wait(ll__IlIlIIIllllIIl__ll) game.Players.LocalPlayer.Character.Humanoid:EquipTool(ll__IIIlIIllIl__ll) end end for ll__IlIIllIIlllIl__ll,ll__IlIlIlIlIll__ll in pairs (game.Players.LocalPlayer.Backpack:GetChildren()) do if string.find(ll__IlIlIlIlIll__ll.Name,"Fruit") then local ll__IlIIIIllllIl__ll = ll__IlIlIlIlIll__ll.Name ll__lIIlIlllIllIlllIllIL__ll(ll__IlIIIIllllIl__ll) end end end end ) if _G.ll__lIllI__ll then game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = ll_lIIlIll_ll[i].CFrame end end until ll__lIllIl__ll == true end end  game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = ll_lIIlIIllIll_ll  end else  local ll__lIIlIIlllIl__ll = "YOUR MOTHER AND YOUR SISTER SUCK MY DICK!" ll__lIllIllIl__ll:kick(ll__lIIlIIlllIl__ll) end
    end
})

local Test = UI:addPage({
    title = "DevillFruit",
    icon = 5012544693
})



local SectionD = Test:addSection({
    title = "DevillFruit"
})

SectionD:addButton({
    title = "TeleportDF",
    callback = function()
        local h = game.Players.LocalPlayer.Character.HumanoidRootPart
 
for i, v in pairs(workspace:GetChildren()) do
    if v:IsA("Tool")  then
        if v.Fruit then
              h.CFrame = v.Fruit.CFrame + Vector3.new(0,4,0)
              wait(1)
        end
    end
    if v:IsA("Model") and v.Name == "Fruit " then
      if v.Fruit then
              h.CFrame = v.Fruit.CFrame + Vector3.new(0,4,0)
              wait(1)
        end
    end
end
    end
})

local Test = UI:addPage({
    title = "Dungeon",
    icon = 5012544693
})

local SectionD = Test:addSection({
    title = "Dungeon"
})

SectionD:addButton({
    title = "Kill Aura",
    callback = function()
        print("Clicked")
    end
})

local Test = UI:addPage({
    title = "Misc",
    icon = 5012544693
})

local SectionD = Test:addSection({
    title = "Player Boost"
})


SectionD:addButton({
    title = "AutoClick F5 no F6 off",
    callback = function()
        local on
local keybind=Enum.KeyCode.F5
local keybindEnd=Enum.KeyCode.F6
local UserInputService=game:GetService("UserInputService")
local RunService=game:GetService("RunService")
local plr=game:GetService("Players").LocalPlayer
local mouse=plr:GetMouse()

local sg=Instance.new("ScreenGui",plr.PlayerGui)
local f=Instance.new("TextLabel",sg)
f.Size=UDim2.new(0,25,0,10)
f.BackgroundColor3=Color3.fromRGB(180,50,50)
f.Visible=false
f.Text="On"
f.TextSize=11

local vu = game:GetService("VirtualUser")
local function CC()
vu:CaptureController();
end 
local function CB()
local v2 = Vector2.new();
vu:ClickButton1(v2);
end

function Start(a,b)
   if a.KeyCode==keybind then
       on=true
       a=RunService.Stepped:Connect(function()
           if on then
               CC();
               CB();
               f.Visible=true
               f.Position=UDim2.new(0,mouse.X-12.5,0,mouse.Y-15)
           else
               a:Disconnect()
           end
       end)
       f.Visible=false
   end
end

function Stop(a,b)
   if a.KeyCode==keybindEnd then
       on=false
       f.Visible=false
   end
end

UserInputService.InputBegan:connect(Start)
UserInputService.InputEnded:connect(Stop)

    end
})

local SectionD = Test:addSection({
    title = "Craracter"
})

SectionD:addButton({
    title = "WalkSpeed 100",
    callback = function()
        _G.HackedWalkSpeed = 100
 
local Plrs = game:GetService("Players")
 
local MyPlr = Plrs.LocalPlayer
local MyChar = MyPlr.Character
 
if MyChar then
local Hum = MyChar.Humanoid
Hum.Changed:connect(function()
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
Hum.WalkSpeed = _G.HackedWalkSpeed
end
 
 
MyPlr.CharacterAdded:connect(function(Char)
MyChar = Char
repeat wait() until Char:FindFirstChild("Humanoid")
local Hum = Char.Humanoid
Hum.Changed:connect(function()
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
    end
})

SectionD:addButton({
    title = "WalkSpeed 200",
    callback = function()
        _G.HackedWalkSpeed = 200
 
local Plrs = game:GetService("Players")
 
local MyPlr = Plrs.LocalPlayer
local MyChar = MyPlr.Character
 
if MyChar then
local Hum = MyChar.Humanoid
Hum.Changed:connect(function()
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
Hum.WalkSpeed = _G.HackedWalkSpeed
end
 
 
MyPlr.CharacterAdded:connect(function(Char)
MyChar = Char
repeat wait() until Char:FindFirstChild("Humanoid")
local Hum = Char.Humanoid
Hum.Changed:connect(function()
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
    end
})

SectionD:addButton({
    title = "WalkSpeed 300",
    callback = function()
        _G.HackedWalkSpeed = 300
 
local Plrs = game:GetService("Players")
 
local MyPlr = Plrs.LocalPlayer
local MyChar = MyPlr.Character
 
if MyChar then
local Hum = MyChar.Humanoid
Hum.Changed:connect(function()
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
Hum.WalkSpeed = _G.HackedWalkSpeed
end
 
 
MyPlr.CharacterAdded:connect(function(Char)
MyChar = Char
repeat wait() until Char:FindFirstChild("Humanoid")
local Hum = Char.Humanoid
Hum.Changed:connect(function()
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
    end
})

SectionD:addButton({
    title = "WalkSpeedReset",
    callback = function()
        _G.HackedWalkSpeed = 50
 
local Plrs = game:GetService("Players")
 
local MyPlr = Plrs.LocalPlayer
local MyChar = MyPlr.Character
 
if MyChar then
local Hum = MyChar.Humanoid
Hum.Changed:connect(function()
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
Hum.WalkSpeed = _G.HackedWalkSpeed
end
 
 
MyPlr.CharacterAdded:connect(function(Char)
MyChar = Char
repeat wait() until Char:FindFirstChild("Humanoid")
local Hum = Char.Humanoid
Hum.Changed:connect(function()
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
Hum.WalkSpeed = _G.HackedWalkSpeed
end)
    end
})

SectionD:addButton({
    title = "JumpPower100",
    callback = function()
        local jump = 100 -- Add the amount of jump power you want here!
 
spawn(function()
while wait() do
game.Players.LocalPlayer.Character.Humanoid.JumpPower = jump
end
end)
    end
})

SectionD:addButton({
    title = "JumpPower200",
    callback = function()
        local jump = 200 -- Add the amount of jump power you want here!
 
spawn(function()
while wait() do
game.Players.LocalPlayer.Character.Humanoid.JumpPower = jump
end
end)
    end
})

SectionD:addButton({
    title = "JumpPower300",
    callback = function()
        local jump = 300 -- Add the amount of jump power you want here!
 
spawn(function()
while wait() do
game.Players.LocalPlayer.Character.Humanoid.JumpPower = jump
end
end)
    end
})

SectionD:addButton({
    title = "JumpPowerReset",
    callback = function()
        local jump = 50 -- Add the amount of jump power you want here!
 
spawn(function()
while wait() do
game.Players.LocalPlayer.Character.Humanoid.JumpPower = jump
end
end)
    end
})

SectionD:addButton({
    title = "No Clip",
    callback = function()
        local player = game.Players.LocalPlayer
local mouse = player:GetMouse()
local runservice = game:GetService("RunService")
local noclip = true
 
local msg = Instance.new("Message", player.PlayerGui)
msg.Text = "Noclip Script by 1E A Press on 'e' to noclip & 't' to destroy this message! & 'f' to turn off noclip"
 
runservice.Stepped:Connect(function()
    if noclip then
        player.Character.Humanoid:ChangeState(11)
    end
end)
 
mouse.KeyDown:Connect(function(key)
    if key == "t" then
        msg:Destroy()
    end
end)
 
mouse.KeyDown:Connect(function(key)
    if key == "e" then
        noclip = true
        player.Character.Humanoid:ChangeState(11)
    end
end)
 
mouse.KeyDown:Connect(function(key)
    if key == "f" then
        noclip = false
        player.Character.Humanoid:ChangeState(7)
    end
end)
    end
})

local SectionD = Test:addSection({
    title = "Character Misc"
})

SectionD:addButton({
    title = "Invisible",
    callback = function()
        for i,v in pairs(game:GetService("Players").LocalPlayer.Character:GetChildren()) do
	if v:IsA("Shirt") or v:IsA("Pants") or v:IsA("Hat") then
		v:Destroy()
	end
	if v:IsA("Part") or v:IsA("MeshPart") then
		v.Transparency = 1
		if v.Name == "Head" then
			if v:FindFirstChild("face") then
				v.face:Destroy()
			end
		end
	end
end
    end
})

SectionD:addButton({
    title = "Fly E To Off Have Bug",
    callback = function()
        repeat wait() 
	until game.Players.LocalPlayer and game.Players.LocalPlayer.Character and game.Players.LocalPlayer.Character:findFirstChild("HumanoidRootPart") and game.Players.LocalPlayer.Character:findFirstChild("Humanoid") 
local mouse = game.Players.LocalPlayer:GetMouse() 
repeat wait() until mouse
local plr = game.Players.LocalPlayer 
local torso = plr.Character.HumanoidRootPart 
local flying = true
local deb = true 
local ctrl = {f = 0, b = 0, l = 0, r = 0} 
local lastctrl = {f = 0, b = 0, l = 0, r = 0} 
local maxspeed = 5000
local speed = 15
 
function Fly() 
local bg = Instance.new("BodyGyro", torso) 
bg.P = 9e4 
bg.maxTorque = Vector3.new(9e9, 9e9, 9e9) 
bg.cframe = torso.CFrame 
local bv = Instance.new("BodyVelocity", torso) 
bv.velocity = Vector3.new(0,0.1,0) 
bv.maxForce = Vector3.new(9e9, 9e9, 9e9) 
repeat wait() 
plr.Character.Humanoid.PlatformStand = true 
if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then 
speed = speed+.100+(speed/maxspeed) 
if speed > maxspeed then 
speed = maxspeed 
end 
elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then 
speed = speed-1 
if speed < 5 then 
speed = 5 
end 
end 
if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r} 
elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
else 
bv.velocity = Vector3.new(0,0.1,0) 
end 
bg.cframe = game.Workspace.CurrentCamera.CoordinateFrame * CFrame.Angles(-math.rad((ctrl.f+ctrl.b)*50*speed/maxspeed),0,0) 
until not flying 
ctrl = {f = 0, b = 0, l = 0, r = 0} 
lastctrl = {f = 0, b = 0, l = 0, r = 0} 
speed = 0 
bg:Destroy() 
bv:Destroy() 
plr.Character.Humanoid.PlatformStand = false 
end 
mouse.KeyDown:connect(function(key) 
if key:lower() == "e" then 
if flying then flying = false 
else 
flying = true 
Fly() 
end 
elseif key:lower() == "w" then 
ctrl.f = 1 
elseif key:lower() == "s" then 
ctrl.b = -1 
elseif key:lower() == "a" then 
ctrl.l = -1 
elseif key:lower() == "d" then 
ctrl.r = 1 
end 
end) 
mouse.KeyUp:connect(function(key) 
if key:lower() == "w" then 
ctrl.f = 0 
elseif key:lower() == "s" then 
ctrl.b = 0 
elseif key:lower() == "a" then 
ctrl.l = 0 
elseif key:lower() == "d" then 
ctrl.r = 0 
end 
end)
Fly()
    end
})

SectionD:addButton({
    title = "Fly Speed 20",
    callback = function()
        repeat wait() 
	until game.Players.LocalPlayer and game.Players.LocalPlayer.Character and game.Players.LocalPlayer.Character:findFirstChild("HumanoidRootPart") and game.Players.LocalPlayer.Character:findFirstChild("Humanoid") 
local mouse = game.Players.LocalPlayer:GetMouse() 
repeat wait() until mouse
local plr = game.Players.LocalPlayer 
local torso = plr.Character.HumanoidRootPart 
local flying = true
local deb = true 
local ctrl = {f = 0, b = 0, l = 0, r = 0} 
local lastctrl = {f = 0, b = 0, l = 0, r = 0} 
local maxspeed = 5000 
local speed = 20 
 
function Fly() 
local bg = Instance.new("BodyGyro", torso) 
bg.P = 9e4 
bg.maxTorque = Vector3.new(9e9, 9e9, 9e9) 
bg.cframe = torso.CFrame 
local bv = Instance.new("BodyVelocity", torso) 
bv.velocity = Vector3.new(0,0.1,0) 
bv.maxForce = Vector3.new(9e9, 9e9, 9e9) 
repeat wait() 
plr.Character.Humanoid.PlatformStand = true 
if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then 
speed = speed+.5+(speed/maxspeed) 
if speed > maxspeed then 
speed = maxspeed 
end 
elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then 
speed = speed-1 
if speed < 0 then 
speed = 0 
end 
end 
if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r} 
elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
else 
bv.velocity = Vector3.new(0,0.1,0) 
end 
bg.cframe = game.Workspace.CurrentCamera.CoordinateFrame * CFrame.Angles(-math.rad((ctrl.f+ctrl.b)*50*speed/maxspeed),0,0) 
until not flying 
ctrl = {f = 0, b = 0, l = 0, r = 0} 
lastctrl = {f = 0, b = 0, l = 0, r = 0} 
speed = 0 
bg:Destroy() 
bv:Destroy() 
plr.Character.Humanoid.PlatformStand = false 
end 
mouse.KeyDown:connect(function(key) 
if key:lower() == "e" then 
if flying then flying = false 
else 
flying = true 
Fly() 
end 
elseif key:lower() == "w" then 
ctrl.f = 1 
elseif key:lower() == "s" then 
ctrl.b = -1 
elseif key:lower() == "a" then 
ctrl.l = -1 
elseif key:lower() == "d" then 
ctrl.r = 1 
end 
end) 
mouse.KeyUp:connect(function(key) 
if key:lower() == "w" then 
ctrl.f = 0 
elseif key:lower() == "s" then 
ctrl.b = 0 
elseif key:lower() == "a" then 
ctrl.l = 0 
elseif key:lower() == "d" then 
ctrl.r = 0 
end 
end)
Fly()
    end
})

SectionD:addButton({
    title = "Fly Speed 50",
    callback = function()
        repeat wait() 
	until game.Players.LocalPlayer and game.Players.LocalPlayer.Character and game.Players.LocalPlayer.Character:findFirstChild("HumanoidRootPart") and game.Players.LocalPlayer.Character:findFirstChild("Humanoid") 
local mouse = game.Players.LocalPlayer:GetMouse() 
repeat wait() until mouse
local plr = game.Players.LocalPlayer 
local torso = plr.Character.HumanoidRootPart 
local flying = true
local deb = true 
local ctrl = {f = 0, b = 0, l = 0, r = 0} 
local lastctrl = {f = 0, b = 0, l = 0, r = 0} 
local maxspeed = 5000 
local speed = 50 
 
function Fly() 
local bg = Instance.new("BodyGyro", torso) 
bg.P = 9e4 
bg.maxTorque = Vector3.new(9e9, 9e9, 9e9) 
bg.cframe = torso.CFrame 
local bv = Instance.new("BodyVelocity", torso) 
bv.velocity = Vector3.new(0,0.1,0) 
bv.maxForce = Vector3.new(9e9, 9e9, 9e9) 
repeat wait() 
plr.Character.Humanoid.PlatformStand = true 
if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then 
speed = speed+.5+(speed/maxspeed) 
if speed > maxspeed then 
speed = maxspeed 
end 
elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then 
speed = speed-1 
if speed < 0 then 
speed = 0 
end 
end 
if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r} 
elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
else 
bv.velocity = Vector3.new(0,0.1,0) 
end 
bg.cframe = game.Workspace.CurrentCamera.CoordinateFrame * CFrame.Angles(-math.rad((ctrl.f+ctrl.b)*50*speed/maxspeed),0,0) 
until not flying 
ctrl = {f = 0, b = 0, l = 0, r = 0} 
lastctrl = {f = 0, b = 0, l = 0, r = 0} 
speed = 0 
bg:Destroy() 
bv:Destroy() 
plr.Character.Humanoid.PlatformStand = false 
end 
mouse.KeyDown:connect(function(key) 
if key:lower() == "e" then 
if flying then flying = false 
else 
flying = true 
Fly() 
end 
elseif key:lower() == "w" then 
ctrl.f = 1 
elseif key:lower() == "s" then 
ctrl.b = -1 
elseif key:lower() == "a" then 
ctrl.l = -1 
elseif key:lower() == "d" then 
ctrl.r = 1 
end 
end) 
mouse.KeyUp:connect(function(key) 
if key:lower() == "w" then 
ctrl.f = 0 
elseif key:lower() == "s" then 
ctrl.b = 0 
elseif key:lower() == "a" then 
ctrl.l = 0 
elseif key:lower() == "d" then 
ctrl.r = 0 
end 
end)
Fly()
    end
})

SectionD:addButton({
    title = "Fly Speed 100",
    callback = function()
        repeat wait() 
	until game.Players.LocalPlayer and game.Players.LocalPlayer.Character and game.Players.LocalPlayer.Character:findFirstChild("HumanoidRootPart") and game.Players.LocalPlayer.Character:findFirstChild("Humanoid") 
local mouse = game.Players.LocalPlayer:GetMouse() 
repeat wait() until mouse
local plr = game.Players.LocalPlayer 
local torso = plr.Character.HumanoidRootPart 
local flying = true
local deb = true 
local ctrl = {f = 0, b = 0, l = 0, r = 0} 
local lastctrl = {f = 0, b = 0, l = 0, r = 0} 
local maxspeed = 5000 
local speed = 100 
 
function Fly() 
local bg = Instance.new("BodyGyro", torso) 
bg.P = 9e4 
bg.maxTorque = Vector3.new(9e9, 9e9, 9e9) 
bg.cframe = torso.CFrame 
local bv = Instance.new("BodyVelocity", torso) 
bv.velocity = Vector3.new(0,0.1,0) 
bv.maxForce = Vector3.new(9e9, 9e9, 9e9) 
repeat wait() 
plr.Character.Humanoid.PlatformStand = true 
if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then 
speed = speed+.5+(speed/maxspeed) 
if speed > maxspeed then 
speed = maxspeed 
end 
elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then 
speed = speed-1 
if speed < 0 then 
speed = 0 
end 
end 
if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r} 
elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
else 
bv.velocity = Vector3.new(0,0.1,0) 
end 
bg.cframe = game.Workspace.CurrentCamera.CoordinateFrame * CFrame.Angles(-math.rad((ctrl.f+ctrl.b)*50*speed/maxspeed),0,0) 
until not flying 
ctrl = {f = 0, b = 0, l = 0, r = 0} 
lastctrl = {f = 0, b = 0, l = 0, r = 0} 
speed = 0 
bg:Destroy() 
bv:Destroy() 
plr.Character.Humanoid.PlatformStand = false 
end 
mouse.KeyDown:connect(function(key) 
if key:lower() == "e" then 
if flying then flying = false 
else 
flying = true 
Fly() 
end 
elseif key:lower() == "w" then 
ctrl.f = 1 
elseif key:lower() == "s" then 
ctrl.b = -1 
elseif key:lower() == "a" then 
ctrl.l = -1 
elseif key:lower() == "d" then 
ctrl.r = 1 
end 
end) 
mouse.KeyUp:connect(function(key) 
if key:lower() == "w" then 
ctrl.f = 0 
elseif key:lower() == "s" then 
ctrl.b = 0 
elseif key:lower() == "a" then 
ctrl.l = 0 
elseif key:lower() == "d" then 
ctrl.r = 0 
end 
end)
Fly()
    end
})

SectionD:addButton({
    title = "Fly Speed 200",
    callback = function()
        repeat wait() 
	until game.Players.LocalPlayer and game.Players.LocalPlayer.Character and game.Players.LocalPlayer.Character:findFirstChild("HumanoidRootPart") and game.Players.LocalPlayer.Character:findFirstChild("Humanoid") 
local mouse = game.Players.LocalPlayer:GetMouse() 
repeat wait() until mouse
local plr = game.Players.LocalPlayer 
local torso = plr.Character.HumanoidRootPart 
local flying = true
local deb = true 
local ctrl = {f = 0, b = 0, l = 0, r = 0} 
local lastctrl = {f = 0, b = 0, l = 0, r = 0} 
local maxspeed = 5000 
local speed = 200 
 
function Fly() 
local bg = Instance.new("BodyGyro", torso) 
bg.P = 9e4 
bg.maxTorque = Vector3.new(9e9, 9e9, 9e9) 
bg.cframe = torso.CFrame 
local bv = Instance.new("BodyVelocity", torso) 
bv.velocity = Vector3.new(0,0.1,0) 
bv.maxForce = Vector3.new(9e9, 9e9, 9e9) 
repeat wait() 
plr.Character.Humanoid.PlatformStand = true 
if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then 
speed = speed+.5+(speed/maxspeed) 
if speed > maxspeed then 
speed = maxspeed 
end 
elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then 
speed = speed-1 
if speed < 0 then 
speed = 0 
end 
end 
if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r} 
elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
else 
bv.velocity = Vector3.new(0,0.1,0) 
end 
bg.cframe = game.Workspace.CurrentCamera.CoordinateFrame * CFrame.Angles(-math.rad((ctrl.f+ctrl.b)*50*speed/maxspeed),0,0) 
until not flying 
ctrl = {f = 0, b = 0, l = 0, r = 0} 
lastctrl = {f = 0, b = 0, l = 0, r = 0} 
speed = 0 
bg:Destroy() 
bv:Destroy() 
plr.Character.Humanoid.PlatformStand = false 
end 
mouse.KeyDown:connect(function(key) 
if key:lower() == "e" then 
if flying then flying = false 
else 
flying = true 
Fly() 
end 
elseif key:lower() == "w" then 
ctrl.f = 1 
elseif key:lower() == "s" then 
ctrl.b = -1 
elseif key:lower() == "a" then 
ctrl.l = -1 
elseif key:lower() == "d" then 
ctrl.r = 1 
end 
end) 
mouse.KeyUp:connect(function(key) 
if key:lower() == "w" then 
ctrl.f = 0 
elseif key:lower() == "s" then 
ctrl.b = 0 
elseif key:lower() == "a" then 
ctrl.l = 0 
elseif key:lower() == "d" then 
ctrl.r = 0 
end 
end)
Fly()
    end
})

SectionD:addButton({
    title = "Fly Speed 300",
    callback = function()
        repeat wait() 
	until game.Players.LocalPlayer and game.Players.LocalPlayer.Character and game.Players.LocalPlayer.Character:findFirstChild("HumanoidRootPart") and game.Players.LocalPlayer.Character:findFirstChild("Humanoid") 
local mouse = game.Players.LocalPlayer:GetMouse() 
repeat wait() until mouse
local plr = game.Players.LocalPlayer 
local torso = plr.Character.HumanoidRootPart 
local flying = true
local deb = true 
local ctrl = {f = 0, b = 0, l = 0, r = 0} 
local lastctrl = {f = 0, b = 0, l = 0, r = 0} 
local maxspeed = 5000 
local speed = 300 
 
function Fly() 
local bg = Instance.new("BodyGyro", torso) 
bg.P = 9e4 
bg.maxTorque = Vector3.new(9e9, 9e9, 9e9) 
bg.cframe = torso.CFrame 
local bv = Instance.new("BodyVelocity", torso) 
bv.velocity = Vector3.new(0,0.1,0) 
bv.maxForce = Vector3.new(9e9, 9e9, 9e9) 
repeat wait() 
plr.Character.Humanoid.PlatformStand = true 
if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then 
speed = speed+.5+(speed/maxspeed) 
if speed > maxspeed then 
speed = maxspeed 
end 
elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then 
speed = speed-1 
if speed < 0 then 
speed = 0 
end 
end 
if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r} 
elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then 
bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed 
else 
bv.velocity = Vector3.new(0,0.1,0) 
end 
bg.cframe = game.Workspace.CurrentCamera.CoordinateFrame * CFrame.Angles(-math.rad((ctrl.f+ctrl.b)*50*speed/maxspeed),0,0) 
until not flying 
ctrl = {f = 0, b = 0, l = 0, r = 0} 
lastctrl = {f = 0, b = 0, l = 0, r = 0} 
speed = 0 
bg:Destroy() 
bv:Destroy() 
plr.Character.Humanoid.PlatformStand = false 
end 
mouse.KeyDown:connect(function(key) 
if key:lower() == "e" then 
if flying then flying = false 
else 
flying = true 
Fly() 
end 
elseif key:lower() == "w" then 
ctrl.f = 1 
elseif key:lower() == "s" then 
ctrl.b = -1 
elseif key:lower() == "a" then 
ctrl.l = -1 
elseif key:lower() == "d" then 
ctrl.r = 1 
end 
end) 
mouse.KeyUp:connect(function(key) 
if key:lower() == "w" then 
ctrl.f = 0 
elseif key:lower() == "s" then 
ctrl.b = 0 
elseif key:lower() == "a" then 
ctrl.l = 0 
elseif key:lower() == "d" then 
ctrl.r = 0 
end 
end)
Fly()
    end
})

local SectionD = Test:addSection({
    title = "Server"
})



SectionD:addButton({
    title = "ServersHop",
    callback = function()
        --Server Hop Script cr.Magma Hub Src
          local PlaceID = 2753915549
          local AllIDs = {}
          local foundAnything = ""
          local actualHour = os.date("!*t").hour
          local Deleted = false
          --[[
          local File = pcall(function()
              AllIDs = game:GetService('HttpService'):JSONDecode(readfile("NotSameServers.json"))
          end)
          if not File then
              table.insert(AllIDs, actualHour)
              writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
          end
          ]]
          function TPReturner()
              local Site;
              if foundAnything == "" then
                  Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
              else
                  Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
              end
              local ID = ""
              if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
                  foundAnything = Site.nextPageCursor
              end
              local num = 0;
              for i,v in pairs(Site.data) do
                  local Possible = true
                  ID = tostring(v.id)
                  if tonumber(v.maxPlayers) > tonumber(v.playing) then
                      for _,Existing in pairs(AllIDs) do
                          if num ~= 0 then
                              if ID == tostring(Existing) then
                                  Possible = false
                              end
                          else
                              if tonumber(actualHour) ~= tonumber(Existing) then
                                  local delFile = pcall(function()
                                      -- delfile("NotSameServers.json")
                                      AllIDs = {}
                                      table.insert(AllIDs, actualHour)
                                  end)
                              end
                          end
                          num = num + 1
                      end
                      if Possible == true then
                          table.insert(AllIDs, ID)
                          wait()
                          pcall(function()
                              -- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
                              wait()
                              game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
                          end)
                          wait(4)
                      end
                  end
              end
          end

          function Teleport()
              while wait() do
                  pcall(function()
                      TPReturner()
                      if foundAnything ~= "" then
                          TPReturner()
                      end
                  end)
              end
          end

          Teleport()
    end
})

SectionD:addButton({
    title = "FpsBoost",
    callback = function()
        for _,v in pairs(workspace:GetDescendants()) do
if v.ClassName == "Part"
or v.ClassName == "SpawnLocation"
or v.ClassName == "WedgePart"
or v.ClassName == "Terrain"
or v.ClassName == "MeshPart" then
v.Material = "Plastic"
end
end
 
--level 2
 
for _,v in pairs(workspace:GetDescendants()) do
if v.ClassName == "Part"
or v.ClassName == "SpawnLocation"
or v.ClassName == "WedgePart"
or v.ClassName == "Terrain"
or v.ClassName == "MeshPart" then
v.Material = "Plastic"
end
end
 
for _,v in pairs(workspace:GetDescendants()) do
if v.ClassName == "Decal"
or v.ClassName == "Texture" then
v:Destroy()
end
end
 
--level 3
 
for _,v in pairs(workspace:GetDescendants()) do
if v.ClassName == "Part"
or v.ClassName == "SpawnLocation"
or v.ClassName == "WedgePart"
or v.ClassName == "Terrain"
or v.ClassName == "MeshPart" then
v.BrickColor = BrickColor.new(155, 155, 155)
v.Material = "Plastic"
end
end
 
for _,v in pairs(workspace:GetDescendants()) do
if v.ClassName == "Decal"
or v.ClassName == "Texture" then
v:Destroy()
end
end
    end
})

SectionD:addButton({
    title = "RejoinServer",
    callback = function()
        wait(1) game:GetService("TeleportService"):Teleport(2753915549, LocalPlayer)
    end
})

SectionD:addButton({
    title = "ServerCrash",
    callback = function()
        print("please wait while we attempt to crash the game")
for i=1, 68 do
  spawn(function()
      while true do
          game:service("RunService").RenderStepped:wait()
         for i=1, 64 do
                  game:service("Players"):Chat("/e i love roblox")
                  game:service("Players"):Chat("/e i love roblox")
                  game:service("Players"):Chat("/e i love roblox")
                  game:service("Players"):Chat("/e i love roblox")
                  game:service("Players"):Chat("/e i love roblox")
                  game:service("Players"):Chat("/e i love roblox")
                  game:service("Players"):Chat("/e i love roblox")
                  end
          end
  print("done?")
      end)
  end
    end
})

SectionD:addButton({
    title = "Anti AFK",
    callback = function()
        wait(0.5)local ba=Instance.new("ScreenGui")
local ca=Instance.new("TextLabel")local da=Instance.new("Frame")
local _b=Instance.new("TextLabel")local ab=Instance.new("TextLabel")ba.Parent=game.CoreGui
ba.ZIndexBehavior=Enum.ZIndexBehavior.Sibling;ca.Parent=ba;ca.Active=true
ca.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)ca.Draggable=true
ca.Position=UDim2.new(0.698610067,0,0.098096624,0)ca.Size=UDim2.new(0,304,0,52)
ca.Font=Enum.Font.SourceSansSemibold;ca.Text="Anti Afk Kick Script"ca.TextColor3=Color3.new(0,1,1)
ca.TextSize=22;da.Parent=ca
da.BackgroundColor3=Color3.new(0.196078,0.196078,0.196078)da.Position=UDim2.new(0,0,1.0192306,0)
da.Size=UDim2.new(0,304,0,107)_b.Parent=da
_b.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)_b.Position=UDim2.new(0,0,0.800455689,0)
_b.Size=UDim2.new(0,304,0,21)_b.Font=Enum.Font.Arial;_b.Text="Made by XxSwordmaster_2xX"
_b.TextColor3=Color3.new(1,1,1)_b.TextSize=20;ab.Parent=da
ab.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)ab.Position=UDim2.new(0,0,0.158377379,0)
ab.Size=UDim2.new(0,304,0,44)ab.Font=Enum.Font.ArialBold;ab.Text="Status: Script Started"
ab.TextColor3=Color3.new(1,1,1)ab.TextSize=20;local bb=game:service'VirtualUser'
game:service'Players'.LocalPlayer.Idled:connect(function()
bb:CaptureController()bb:ClickButton2(Vector2.new())
ab.Text="You went idle and ROBLOX tried to kick you but we reflected it!"wait(2)ab.Text="Script Re-Enabled"end)
    end
})


local Test = UI:addPage({
    title = "Settings",
    icon = 5012544693
})

local SectionD = Test:addSection({
    title = "Settings"
})

-- // Color Theme Customisation Page

SectionD:addKeybind({
    title = "Toggle Keybind",
    key = Enum.KeyCode.One,
    callback = function()
        print("Activated Keybind")
        UI:toggle()
    end,
    changedCallback = function(key)
        print("Changed Keybind", key)
    end
})


local Theme = UI:addPage({
    title = "Theme",
    icon = 5012544693
})

-- // Section for the Color Theme Customisation Page
local Colors = Theme:addSection({
    title = "Colors"
})

-- // Adding a color picker for each type of theme customisable
for theme, color in pairs(Themes) do
    Colors:addColorPicker({
        title = theme,
        default = color,
        callback = function(color3)
            UI:setTheme({
                theme = theme, 
                color3 = color3
            })
        end
    })
end

-- // Load
UI:SelectPage({
    page = UI.pages[1], 
    toggle = true
})
local Test = UI:addPage({
    title = "Credits",
    icon = 5012544693
})

local SectionD = Test:addSection({
    title = "Credits"
})

SectionD:addButton({
    title = "Ui Design and Components",
    callback = function()
        print("1")
    end
})

SectionD:addButton({
    title = "Veny",
    callback = function()
        print("2")
    end
})

SectionD:addButton({
    title = "Developer",
    callback = function()
        print("3")
    end
})

SectionD:addButton({
    title = "1 EA",
    callback = function()
        print("4")
    end
})

SectionD:addButton({
    title = "Credits",
    callback = function()
        print("5")
    end
})

SectionD:addButton({
    title = "1 EA",
    callback = function()
        print("6")
    end
})
