getgenv().rejoin = game:GetService("CoreGui").RobloxPromptGui.promptOverlay.ChildAdded:Connect(function(child)
    if child.Name == 'ErrorPrompt' and child:FindFirstChild('MessageArea') and child.MessageArea:FindFirstChild("ErrorFrame") then
        game:GetService("TeleportService"):Teleport(game.PlaceId)
    end
end)



s = Instance.new("Sound",Workspace)
        s.Pitch = 1
        s.Volume = 1000
        s.SoundId = "rbxassetid://9577148759"
        s.Looped = false
        s.PlayOnRemove = false
        s:Play()
        
if game:GetService("Players").LocalPlayer.PlayerGui:FindFirstChild("Ticket") then
    game:GetService("Players").LocalPlayer.PlayerGui:FindFirstChild("Ticket"):Destroy()
    end

local DiscordLib =
    loadstring(game:HttpGet "https://pastebin.com/raw/pjQ6yNJK")()

local win = DiscordLib:Window("CorlHub | Premium  ")

local serv = win:Server("Main", "")

local A = serv:Channel("Player")

local B = serv:Channel("Teleport  (Bike Requests)")

local C = serv:Channel("Combat")

local D = serv:Channel("Anti")

local F = serv:Channel("Fun & Troll")

A:Button(
    "Fly",
    function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/fk7/main/README.md"))()
    end
)

A:Button(
    "Fly Bypass (Bike Requests)",
    function()
        local plr = game:GetService("Players").LocalPlayer
        local pos = game.Players.LocalPlayer.Character.HumanoidRootPart.Position
        local roundedPos = math.round(pos.X) .. ", " .. math.round(pos.Y) .. ", " .. math.round(pos.Z)
        
        function bypass()
          if game.Players.LocalPlayer.Character.Humanoid.Sit ~= true then
              rconsoleclear()
            rconsolewarn("Please be seated in any vehicle to inititate Bypass. \n - You can also sit in the passenger seat!")
          end
            
          if game.Players.LocalPlayer.Character.Humanoid.Sit ~= false then
            workspace[plr.Name .. "'s Car"]:MoveTo(roundedPos)
            workspace[plr.Name .. "'s Car"].DriveSeat:Sit(plr.Character.Humanoid)
         end
        end
        
        bypass()
        rconsoleclear()
        rconsolewarn("Successful! \n -If anything bugs out after you stop flying type '/respawn'")
    end
)

    A:Button(
    "Walk Speed Bypass",
    function()
        local plr = game.Players.LocalPlayer
            local char = plr.Character
        
            char.Humanoid.WalkSpeed = 40
    end
)

A:Button(
    "Skip loading Screen",
    function()
        local LP = game:GetService("Players").LocalPlayer
if LP.PlayerGui:FindFirstChild("Menu") then
LP.PlayerGui:FindFirstChild("Menu"):Destroy()
end

if LP.PlayerGui:FindFirstChild("Agreement") then
LP.PlayerGui:FindFirstChild("Agreement"):Destroy()
end

LP.PlayerGui.Stats.Enabled = true
LP.PlayerGui.twitter.Enabled = false

workspace.CurrentCamera.CameraType = "Custom"
local char = LP.Character or LP.CharacterAdded:Wait()
workspace.CurrentCamera.CameraSubject = char:WaitForChild("Humanoid")
end
)

A:Button(
    "Infinite Stamina",
    function()
     while true do 
                    wait(0)
                    game.Players.LocalPlayer.Valuestats.Stamina.Value = 100
                end   
    end
)

A:Button(
    "Infinite Hunger",
    function()
       while true do 
                    wait(0)
                    game.Players.LocalPlayer.Valuestats.Hunger.Value = 100
                end  
    end
)

A:Button(
    "Infinite Karma",
    function()
         while true do
                    wait(1)
                    game.Players.LocalPlayer.Valuestats.Karma.Value = 999999
                end
    end
)

A:Button(
    "Infinite Skittles",
    function()
         while wait() do
                    game:GetService("Players").LocalPlayer.PlayerGui.Run.Value.Value = true
                    game.Players.LocalPlayer.Character.Resistance.Value = true
                    game:GetService("Workspace").LocalPlayer.Resistance = true
                end
    end
)

A:Button(
    "Removes Karma Alert",
    function()
  while true do
                    wait(1)
                    game.ReplicatedStorage.KarmaAlert:Destroy()
            end
    end
)

A:Button(
    "Removes Traffic City Noises",
    function()
 while true do
                    wait(1)
                    game.SoundService["Traffic City Noises"]:Destroy()
        end
    end
)

A:Button(
    "Remove Damage Blood",
    function()
wait(1)
                    game.Players.LocalPlayer.PlayerGui.Dmg:Destroy()
    end
)

B:Button(
    "Bring Car",
    function()
         local plr = game:GetService("Players").LocalPlayer
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait(.1)
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)

    end
)

B:Button(
    "Apartment Bypass",
    function()
         game.ReplicatedStorage.Places:Clone().Parent = game.Workspace
    end
)

B:Textbox(
    "Teleport To Player",
    "Put Player Name Here",
    true,
    function(text)
        for i, v in pairs(game.Players:GetChildren()) do
            if (string.sub(string.lower(v.Name), 1, string.len(text))) == string.lower(text) then
                text = v.Name
            end
        end
        local plr = game.Players.LocalPlayer
        local ooooooof = text
        local plr1 = game.Players.LocalPlayer.Character
        local plr2 = game.Workspace:FindFirstChild(ooooooof)
        plr1.HumanoidRootPart.CFrame = plr2.HumanoidRootPart.CFrame * CFrame.new(0,2,0)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Apartment 1",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-176.541977, -457.964905, -69.6778412, 0.0172199383, -7.30185334e-08, 0.999851704, -1.86776674e-08, 1, 7.33510319e-08, -0.999851704, -1.99379979e-08, 0.0172199383)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Apartment 2",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-175.904221, -457.964905, -493.479797, 0.0789805874, -2.37789219e-08, 0.99687618, -4.13485459e-08, 1, 2.71294027e-08, -0.99687618, -4.33620748e-08, 0.0789805874)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Apartment 3",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-0.532082677, -457.913483, -112.602715, -0.000539803877, -4.52883206e-08, -0.999999881, 6.60640032e-09, 1, -4.52918947e-08, 0.999999881, -6.63084831e-09, -0.000539803877)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Sports Direct",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-195.589691, -463.662384, 92.2535934, 0.238895774, 2.38148239e-08, 0.971045196, 3.21983293e-08, 1, -3.24463443e-08, -0.971045196, 3.90173298e-08, 0.238895774)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Tescos",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(983.751831, -446.635803, 103.678848, -0.381174803, -9.88733646e-08, -0.924502969, -2.49378118e-08, 1, -9.66656728e-08, 0.924502969, -1.37914373e-08, -0.381174803)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Urbans",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(282, 4.45790863, -157, 1, 6.64652404e-08, -1.07617515e-13, -6.64652404e-08, 1, 7.81934428e-09, 1.08137234e-13, -7.81934428e-09, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Bandos",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-20, 4.4000082, -24, 1, 9.46803347e-09, -1.61477362e-14, -9.46803347e-09, 1, -1.32429419e-08, 1.60223516e-14, 1.32429419e-08, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Barbers",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-21, 4.40000916, 102, 1, -3.14583648e-09, -1.63019792e-14, 3.14583648e-09, 1, 4.40034809e-09, 1.62881369e-14, -4.40034809e-09, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Hair Salon",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-21.0000038, 4.40000916, 120.000015, 1, 3.68644564e-08, -1.16391732e-13, -3.68644564e-08, 1, -5.15691454e-08, 1.14490665e-13, 5.15691454e-08, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Muruna Restaurant",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-21, 4.40000916, 209, 1, 3.79887801e-08, -2.18802942e-14, -3.79887801e-08, 1, -5.31432249e-08, 1.98614488e-14, 5.31432249e-08, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Quiz Clothing",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-20, 4.45790815, -52.0000076, 1, -2.40221443e-09, -2.3818412e-13, 2.40221443e-09, 1, 3.36058181e-09, 2.38176042e-13, -3.36058181e-09, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Car Dealership",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-93.9999847, 4.15790749, 542, 1, -1.20612453e-08, -2.38422726e-13, 1.20612453e-08, 1, 1.68743792e-08, 2.38219221e-13, -1.68743792e-08, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Petrol Station",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-391, 4.27190638, 326.000061, 1, -4.65898431e-08, -3.57836346e-13, 4.65898431e-08, 1, 6.51843592e-08, 3.54799415e-13, -6.51843592e-08, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Police Station",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-207, 6, -211, 1, 0, 0, 0, 1, 0, 0, 0, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Banks Boxing",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-190, 4.40000916, 168, 1, -9.0672172e-09, 2.15987354e-14, 9.0672172e-09, 1, -5.94992215e-08, -2.10592431e-14, 5.94992215e-08, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Night Club",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-21, 4.40000916, 182, 1, -5.01537478e-08, -6.47372331e-15, 5.01537478e-08, 1, -5.58382318e-09, 6.75377316e-15, 5.58382318e-09, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Ultimate Drip",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(479.154602, -395.400482, -91.1273499, 0.216078922, 1.49673074e-08, 0.976375878, -1.26980304e-09, 1, -1.50484354e-08, -0.976375878, 2.01184469e-09, 0.216078922)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "School",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-351, 5.93800926, -39, 1, 8.71055903e-08, 5.51441827e-14, -8.71055903e-08, 1, 9.69893588e-09, -5.4299352e-14, -9.69893588e-09, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "New London",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(612.033203, -400.384491, -106.705254, -0.0193231795, -7.59797825e-09, 0.999813318, 1.18716381e-09, 1, 7.62234187e-09, -0.999813318, 1.33423006e-09, -0.0193231795)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "Face Lift",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(281, 4.45790815, -188, 1, -6.91100155e-09, 2.24737441e-14, 6.91100155e-09, 1, -7.69573294e-10, -2.24684248e-14, 7.69573294e-10, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "OO Block",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-359, 4.53488302, -185, 1, -1.25941853e-08, 1.20608318e-14, 1.25941853e-08, 1, -1.76135628e-09, -1.20386489e-14, 1.76135628e-09, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)

B:Button(
    "K33 Block",
    function()
local plr = game.Players.LocalPlayer
        local workspace = game.Workspace
        plr.Character.HumanoidRootPart.CFrame = CFrame.new(-78, 7.00918674, 163, 1, 6.13948075e-08, 1.15661519e-14, -6.13948075e-08, 1, 8.58640181e-09, -1.10389908e-14, -8.58640181e-09, 1)
        game:GetService("Workspace")[plr.Name.."'s Car"]:MoveTo(game.Players.LocalPlayer.Character.HumanoidRootPart.Position)
        task.wait()
        game:GetService("Workspace")[plr.Name.."'s Car"].DriveSeat:sit(plr.Character.Humanoid)
        task.wait()
        game:GetService("ReplicatedStorage").DoorService:FireServer("HOP",workspace:FindFirstChild(plr.Name .. "'s Car"))
    end
)




C:Textbox(
    "Kick Player Fist",
    "Put Player Name Here",
    true,
    function(text)
    for i,v in pairs(game.Players:GetChildren()) do
            if (string.sub(string.lower(v.Name),1,string.len(text))) == string.lower(text) then
            text = v.Name
            end
            end
            -- main scirpt under
            if not game.Players.LocalPlayer.Character:FindFirstChild("Fist") then
               game.Players.LocalPlayer.Backpack.Fist.Parent = game.Players.LocalPlayer.Character
            end

            
            local alive = true
            local name = text
            local kid = game.Players.LocalPlayer.Character
            local kiddie = game.Players[name].Character
            local startpos1 = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
            
            local plr = game:GetService("Players").LocalPlayer
            local char = plr.Character
            --tp bypass 
            for Loop = 1, 10 do
                local args = {
                    [1] = "Apartments"
                }
                game:GetService("ReplicatedStorage").DoorService:FireServer(unpack(args))
                task.wait(0.025)
                char.HumanoidRootPart.CFrame = CFrame.new(-99, 4, -115)
            end
            -- end
            task.wait(1)
            char.HumanoidRootPart.CFrame = startpos1
            
            local ohInstance1 = game.Players[name].Character.Humanoid
            local ohNil2 = nil
            local ohNumber3 = 1
            local ohInstance4 = game.Players[name].Character.Head
            local ohBoolean5 = true
            local ohVector36 = Vector3.new()
            local ohBoolean7 = false
            while alive do
                task.wait(0.05)
            game.Players.LocalPlayer.Character.Fist.LocalScript.Script.e:FireServer(ohInstance1, ohNil2, ohNumber3, ohInstance4, ohBoolean5, ohVector36, ohBoolean7)
            kid.HumanoidRootPart.CFrame = kiddie.HumanoidRootPart.CFrame
    
            if game.Players[name].Character.Humanoid.Health <= 25 or alive == false then
               local args = {
                   [1] = game:GetService("Players")[name]
               }
               game:GetService("ReplicatedStorage").CarryingServer:FireServer(unpack(args))
            
            repeat
               task.wait(0.2)
               --tp bypass
            local plr = game:GetService("Players").LocalPlayer
            local char = plr.Character
            for Loop = 1, 10 do
                local args = {
                    [1] = "Apartments"
                }
                game:GetService("ReplicatedStorage").DoorService:FireServer(unpack(args))
                task.wait(0.025)
                char.HumanoidRootPart.CFrame = CFrame.new(-99, 4, -115)
            end
            -- end
            task.wait(1)
            char.HumanoidRootPart.CFrame = CFrame.new(-2740.23071, -184.292358, -2930.51563, -0.684846103, 0.106422901, -0.720874488, 1.90580485e-09, 0.989277601, 0.146047324, 0.728687763, 0.100019939, -0.677502871) -- Place to TP
                local args = {
       [1] = game:GetService("Players")[name]
   }
   game:GetService("ReplicatedStorage").CarryingServer:FireServer(unpack(args))
               task.wait(0.9)
               game:GetService('Players').LocalPlayer.Character.HumanoidRootPart.CFrame = startpos1
               task.wait(0.2)
               game:GetService('Players').LocalPlayer.Character.HumanoidRootPart.CFrame = startpos1
               task.wait(.2)
               until not game.Players:FindFirstChild(name)
            end
        end
    end
)

C:Textbox(
    "Kill Player Fist",
    "Put Player Name Here",
    true,
    function(text)
       for i, v in pairs(game.Players:GetChildren()) do
            if (string.sub(string.lower(v.Name), 1, string.len(text))) == string.lower(text) then
                text = v.Name
            end
        end
        local Target = text
        local dead

        if not game.Players.LocalPlayer.Backpack:FindFirstChild("Fist") then
            return notify("No fists found!", 10)
        end

        if not game.Players.LocalPlayer.Character:FindFirstChild("Fist") then
            game.Players.LocalPlayer.Backpack.Fist.Parent = game.Players.LocalPlayer.Character
        end

        if game.Players[Target].Character.Humanoid.Health >= 1 then
            dead = false
        end

        if game.Players[Target].Character.Humanoid.Health <= 1 then
            dead = true
        end

        local ohInstance1 = game.Players[Target].Character.Humanoid
        local ohNil2 = nil
        local ohNumber3 = 0
        local ohInstance4 = game.Players.LocalPlayer.Character.Head
        local ohBoolean5 = true
        local ohVector36 = game.Players[Target].Character.HumanoidRootPart.Position
        local ohBoolean7 = false

        while dead ~= true do
            task.wait(.04)
            game.Players.LocalPlayer.Character.Fist.LocalScript.Script.e:FireServer(
                ohInstance1,
                ohNil2,
                ohNumber3,
                ohInstance4,
                ohBoolean5,
                ohVector36,
                ohBoolean7
            )
        end
    end
)

C:Button(
    "HitBox",
    function()
 loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/dedefe/main/README.md"))()
    end
)

C:Button(
    "ESP",
    function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/fwfveef/main/README.md"))()
    end
    )
    
    C:Button(
    "Chat SPY",
    function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/defefef/main/README.md"))()
        end
    )

 C:Button(
    "Pick Up Tools",
    function()
        local g = game.Workspace.tools
    while task.wait() do
        for fk, fl in pairs((g:GetChildren())) do
            if fl:IsA("Tool") then
                if fl:IsA("Tool") and fl.Name == "Phone" or fl.Name == "Crate" then
                else
                    game:GetService("Players").LocalPlayer.Character.Humanoid:EquipTool(fl)
                
                end
            end
        end
    end
        end
    )

 C:Button(
    "Quick Buy Food",
    function()
       loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/sasasas/main/README.md"))()  
        end
    )

 C:Button(
    "Infinite Ammo",
    function()
       for i, v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do 
                if v:IsA("Tool") and v:FindFirstChild("Stats") then
                    task.spawn(function()
                        while task.wait(5) do
                            if v.Stats.ClipSize.Value ~= v.Stats.ClipSize.Original.Value then
                                v.Stats.ClipSize.Value = math.huge
                                v.Stats.ClipSize.Original.Value = math.huge
                            end
                         end
                    end)
                end
            end 
        end
    )
    
    C:Button(
    "One tap",
    function()
        local meleeRemote = game:GetService("ReplicatedStorage").GunRemotes.Impact;
        local OldNameCall = nil
        OldNameCall = hookmetamethod(game, "__namecall", function(Self, ...)
            local Args = {...}
            local NamecallMethod = getnamecallmethod()

            if not checkcaller() and Self == meleeRemote and NamecallMethod == "FireServer" then
                for i=1, 15, 1 do
                    OldNameCall(Self,...);
                end        
            end

            return OldNameCall(Self, ...)
        end)
        end
    )

    
    
     D:Button(
    "Anti AFK",
    function()
       loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/dfefefe/main/README.md"))()
        end
    )
    
    D:Button(
    "Anti Camera Bob",
    function()
       loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/sfegrgr/main/README.md"))()
        end
    )
    
    D:Button(
    "Anti Ragdoll",
    function()
       game:GetService("ReplicatedStorage").Modules.RagdollHandler:Destroy()
        game.ReplicatedStorage.RemoteEvents.SetPlayerRagdolled:Destroy()
        game.Workspace.Ragdoller:Destroy()
        
        while task.wait(1) do 
        if game.Players.LocalPlayer.Character:FindFirstChild("Ragdolled") then
            game.Players.LocalPlayer.Character:FindFirstChild("Ragdolled"):Destroy()
        end 
        end
        end
    )
    
    D:Button(
    "Anti Blur",
    function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/sdfe3/main/README.md"))()
        end
    )
    
     D:Button(
    "Anti Combat Log",
    function()
       game:GetService("Players").LocalPlayer.PlayerGui.Stats.CLog:Destroy()
        end
    )


    
    F:Button(
    "BoomBox",
    function()
         _G.boomboxb = game:GetObjects('rbxassetid://740618400')[1]
                    _G.boomboxb.Parent = game:GetService'Players'.LocalPlayer.Backpack
                    loadstring(_G.boomboxb.Client.Source)() 
                    loadstring(_G.boomboxb.Server.Source)()
    end
    )
    
     F:Button(
    "No Face",
    function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/wqqqq/main/README.md"))()
    end
    )
    
     F:Button(
    "No Head",
    function()
         loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/fdqqqqq/main/README.md"))()
    end
    )
    
     F:Button(
    "bald",
    function()
        for i,v in next, game:GetService('Players').LocalPlayer.Character:GetChildren() do
                    if v:IsA('Accessory') then
                        v:Destroy()
                    end
            end
    end
    )
    
     F:Button(
    "No Legs",
    function()
      loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/eqqqqq/main/README.md"))()  
    end
    )
    
    F:Button(
    "No Arms",
    function()
        game:GetService("Players").LocalPlayer.Character.RightUpperArm:Destroy()
           game:GetService("Players").LocalPlayer.Character.RightLowerArm:Destroy()
           game:GetService("Players").LocalPlayer.Character.LeftUpperArm:Destroy()
           game:GetService("Players").LocalPlayer.Character.LeftLowerArm:Destroy()
    end
    )
    
    F:Button(
    "No Name",
    function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/wwdghjhgfds/main/README.md"))()
    end
    )
    
    F:Button(
    "Fire Hands",
    function()
        Fire.Parent = game.Players.LocalPlayer.Character.RightHand
    Fire.Heat = 5
    Fire.Size = 2
    end
    )
    
    F:Button(
    "Kill Your Self",
    function()
       game.Players.LocalPlayer.Character.Humanoid.Health = 0 
    end
    )
    
     F:Button(
    "Join Low Server",
    function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/WspNas/fgf/main/README.md"))()
    end
    )
    
     F:Button(
    "Loud Sound",
    function()
        local args = {
            [1] = workspace:FindFirstChild(game.Players.LocalPlayer.Name .. "'s Car")
        }
        
        game:GetService("ReplicatedStorage").TireSmoke:FireServer(unpack(args))
        
        local args = {
            [1] = game.Workspace[game.Players.LocalPlayer.Name .. "'s Car"],
            [2] = 1000,
            [3] = 1000,
            [4] = false,
            [5] = 1000,
            [6] = 1000,
            [7] = 0,
            [8] = 1000,
            [9] = false
        }
        
        game:GetService("ReplicatedStorage").CarSound:FireServer(unpack(args))
    end
    )
    
     F:Button(
    "Ghost Drive A Fucking Car",
    function()
        local plr = game.Players.LocalPlayer

-- / function
local function SelfDrive()
    if game:GetService("Workspace")[plr.Name.."'s Car"] then
    game:GetService("Workspace")[plr.Name.."'s Car"]["A-Chassis Tune"]:Clone().Parent = game.Players.LocalPlayer.Character
    else
        rconsoleprint("Failed to find car!")
    end
end

SelfDrive()
    end
    )
    
     F:Button(
        "Call all",
function()
    local function callAll( )
        for i,v in pairs(Players:GetPlayers( )) do
            if v ~= LocalPlayer then
    
                local args = {
                    [1] = v,
                    [2] = "Starting"
                };        
    
                game:GetService("ReplicatedStorage").Call:FireServer(unpack(args));
    
                print("called " .. v.Name);
            end;
        end;
    end;
    callAll()
end
     )  
