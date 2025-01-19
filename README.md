local Player = game.Players.LocalPlayer

local Whitelisted = {
    "El_belicorp",
    "dustsans40404",
    "AnotherUsername"
}

-- Check if the player's name is in the whitelist
if table.find(Whitelisted, Player.Name) then

else
    Player:Kick("Not whitelisted")
end

local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "Liberty Heights NYC🗽",
   Icon = 0, -- Icon in Topbar. Can use Lucide Icons (string) or Roblox Image (number). 0 to use no icon (default).
   LoadingTitle = "Liberty Heights NYC🗽",
   LoadingSubtitle = "",
   Theme = "Ocean", -- Check https://docs.sirius.menu/rayfield/configuration/themes

   DisableRayfieldPrompts = false,
   DisableBuildWarnings = false, -- Prevents Rayfield from warning when the script has a version mismatch with the interface

   ConfigurationSaving = {
      Enabled = true,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "Big Hub"
   },

   Discord = {
      Enabled = false, -- Prompt the user to join your Discord server if their executor supports it
      Invite = "noinvitelink", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },

   KeySystem = false, -- Set this to true to use our key system
   KeySettings = {
      Title = "Key System",
      Subtitle = "Key System",
      Note = "Wrong Key", -- Use this to tell the user how to get a key
      FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {""} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local Tab = Window:CreateTab("Spawners", 4483362458) -- Title, Image

local Section = Tab:CreateSection("Gun Spawners")

local Button = Tab:CreateButton({
    Name = "Glock .45",
    Callback = function()
        local args = {
            [1] = "Glock .45",
    
        }    game:GetService("ReplicatedStorage").Remotes.GiveGun:FireServer(unpack(args)) 
    end,
 })

 local Button = Tab:CreateButton({
    Name = "Beretta M9",
    Callback = function()
        local args = {
            [1] = "Beretta M9",
    
        }    game:GetService("ReplicatedStorage").Remotes.GiveGun:FireServer(unpack(args)) 
    end,
 })

 local Button = Tab:CreateButton({
    Name = "Smith & Wesson M&P",
    Callback = function()
        local args = {
            [1] = "Smith & Wesson M&P",
    
        }    game:GetService("ReplicatedStorage").Remotes.GiveGun:FireServer(unpack(args)) 
    end,
 })


 local Button = Tab:CreateButton({
    Name = "Taurus G3C",
    Callback = function()
        local args = {
            [1] = "Taurus G3C",
    
        }    game:GetService("ReplicatedStorage").Remotes.GiveGun:FireServer(unpack(args)) 
    end,
 })


 local Button = Tab:CreateButton({
    Name = "Hi-Point C-9",
    Callback = function()
        local args = {
            [1] = "Hi-Point C-9",
    
        }    game:GetService("ReplicatedStorage").Remotes.GiveGun:FireServer(unpack(args)) 
    end,
 })

 local Button = Tab:CreateButton({
    Name = "Taurus .380 ACP",
    Callback = function()
        local args = {
            [1] = "Taurus .380 ACP",
    
        }    game:GetService("ReplicatedStorage").Remotes.GiveGun:FireServer(unpack(args)) 
    end,
 })


local Section = Tab:CreateSection("Ammo Spawners")


local Button = Tab:CreateButton({
    Name = "9mm",
    Callback = function()
        local args = {
            [1] = "9mm",
    
        }    game:GetService("ReplicatedStorage").Remotes.GiveGun:FireServer(unpack(args)) 
    end,
 })

 local Button = Tab:CreateButton({
    Name = "7.62 x 39mm",
    Callback = function()
        local args = {
            [1] = "7.62 x 39mm",
    
        }    game:GetService("ReplicatedStorage").Remotes.GiveGun:FireServer(unpack(args)) 
    end,
 })

 local Button = Tab:CreateButton({
    Name = ".380 ACP",
    Callback = function()
        local args = {
            [1] = ".380 ACP",
    
        }    game:GetService("ReplicatedStorage").Remotes.GiveGun:FireServer(unpack(args)) 
    end,
 })
 --------------------------------------------------------------------------------------------------

 local Sigma = Window:CreateTab("Teleports", 4483362458) -- Title, Image

 local Section = Sigma:CreateSection("Disable Anti Cheat")

 local Button = Sigma:CreateButton({
    Name = "Disable Anti Cheat",
    Callback = function()
        local YourRoot = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
        --warn(YourRoot.CFrame)
        --local LocationToTP = workspace["El_belicorp"].HumanoidRootPart.CFrame
        local LocationToTP2 = CFrame.new(-479, -181, -555)
        YourRoot.CFrame = LocationToTP2
    end,
 })

 local Section = Sigma:CreateSection("Teleports")

 local Button = Sigma:CreateButton({
    Name = "Mask Shop",
    Callback = function()
        local YourRoot = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
        --warn(YourRoot.CFrame)
        --local LocationToTP = workspace["El_belicorp"].HumanoidRootPart.CFrame
        local LocationToTP2 = CFrame.new(-640, -58, 885)
        YourRoot.CFrame = LocationToTP2
    end,
 })


 local Button = Sigma:CreateButton({
    Name = "Deli",
    Callback = function()
        local YourRoot = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
        --warn(YourRoot.CFrame)
        --local LocationToTP = workspace["El_belicorp"].HumanoidRootPart.CFrame
        local LocationToTP2 = CFrame.new(-400, -67, 764)
        YourRoot.CFrame = LocationToTP2
    end,
 })

 local Button = Sigma:CreateButton({
    Name = "Bike Shop",
    Callback = function()
        local YourRoot = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
        --warn(YourRoot.CFrame)
        --local LocationToTP = workspace["El_belicorp"].HumanoidRootPart.CFrame
        local LocationToTP2 = CFrame.new(-609, -49, -209)
        YourRoot.CFrame = LocationToTP2
    end,
 })



 local Button = Sigma:CreateButton({
    Name = "Harlem Clothing Shop",
    Callback = function()
        local YourRoot = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
        --warn(YourRoot.CFrame)
        --local LocationToTP = workspace["El_belicorp"].HumanoidRootPart.CFrame
        local LocationToTP2 = CFrame.new(-437, -117, 362)
        YourRoot.CFrame = LocationToTP2
    end,
 })


 local Button = Sigma:CreateButton({
    Name = "Shoe Shop",
    Callback = function()
        local YourRoot = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
        --warn(YourRoot.CFrame)
        --local LocationToTP = workspace["El_belicorp"].HumanoidRootPart.CFrame
        local LocationToTP2 = CFrame.new(155, -50, 279)
        YourRoot.CFrame = LocationToTP2
    end,
 })


 local Button = Sigma:CreateButton({
    Name = "Exotic Shop",
    Callback = function()
        local YourRoot = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
        --warn(YourRoot.CFrame)
        --local LocationToTP = workspace["El_belicorp"].HumanoidRootPart.CFrame
        local LocationToTP2 = CFrame.new(-302, -65, 358)
        YourRoot.CFrame = LocationToTP2
    end,
 })

 

 local Sigmas = Window:CreateTab("Player", 4483362458) -- Title, Image

 local Section = Sigmas:CreateSection("Misc")

 local Slider = Sigmas:CreateSlider({
    Name = "WalkSpeed",
    Range = {0, 100},
    Increment = 1,
    Suffix = "Speed",
    CurrentValue = 0,
    Flag = "Slider1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
    Callback = function(Value)
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = (Value)
    end,
 })

 local Slider = Sigmas:CreateSlider({
    Name = "JumpPower",
    Range = {0, 100},
    Increment = 1,
    Suffix = "Speed",
    CurrentValue = 0,
    Flag = "Slider1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
    Callback = function(Value)
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = (Value)
    end,
 })


 local Slider = Sigmas:CreateSlider({
    Name = "Level",
    Range = {0, 100},
    Increment = 1,
    Suffix = "Level",
    CurrentValue = 0,
    Flag = "Slider1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
    Callback = function(Value)
        game.Players.LocalPlayer.PlayerData.Level.Value = (Value)
    end,
 })

 

 local Section = Sigmas:CreateSection("Spectate")


 local Players = game:GetService("Players")
local playerNames = {}
local selectedPlayer = nil
local camera = workspace.CurrentCamera

-- Collect all player names
for _, player in ipairs(Players:GetPlayers()) do
    table.insert(playerNames, player.Name)
end

local Dropdown = Sigmas:CreateDropdown({
   Name = "Player List",
   Options = playerNames, -- Set the player names as options
   CurrentOption = {playerNames[1]}, -- Set the first player as the current option
   MultipleOptions = false,
   Flag = "Dropdown1",
   Callback = function(Options)
       selectedPlayer = Players:FindFirstChild(Options[1]) -- Store the selected player
       print("Selected player: " .. Options[1])
   end,
})

-- Update the dropdown whenever a new player joins
Players.PlayerAdded:Connect(function(player)
    table.insert(playerNames, player.Name)
    Dropdown:UpdateOptions(playerNames) -- Updates the dropdown options
end)

-- Remove a player from the dropdown if they leave
Players.PlayerRemoving:Connect(function(player)
    for i, name in ipairs(playerNames) do
        if name == player.Name then
            table.remove(playerNames, i)
            break
        end
    end
    Dropdown:UpdateOptions(playerNames) -- Updates the dropdown options
end)

-- Button to view the selected player
local Button = Sigmas:CreateButton({
   Name = "View Player",
   Callback = function()
       if selectedPlayer and selectedPlayer.Character then
           -- Set the camera's subject to the selected player's humanoid
           camera.CameraSubject = selectedPlayer.Character:FindFirstChild("Humanoid")
           print("Now viewing: " .. selectedPlayer.Name)
       else
           print("No player selected or player does not have a character")
       end
   end,
})

-- Button to unview (reset camera back to the player)
local UnviewButton = Sigmas:CreateButton({
   Name = "Unview Player",
   Callback = function()
       -- Set the camera back to the local player's humanoid
       local localPlayer = Players.LocalPlayer
       if localPlayer and localPlayer.Character then
           camera.CameraSubject = localPlayer.Character:FindFirstChild("Humanoid")
           print("Camera reset to local player")
       else
           print("Local player does not have a character")
       end
   end,
})

local Button = Sigmas:CreateButton({
    Name = "Teleport",
    Callback = function()
        if selectedPlayer and selectedPlayer.Character then
            -- Get the LocalPlayer's HumanoidRootPart
            local YourRoot = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
            warn(YourRoot.CFrame)
        
            -- Get the selected player's HumanoidRootPart
            local selectedPlayerRoot = selectedPlayer.Character:FindFirstChild("HumanoidRootPart")
        
            if selectedPlayerRoot then
                -- Get the CFrame of the selected player's HumanoidRootPart
                local LocationToTP = selectedPlayerRoot.CFrame
                YourRoot.CFrame = LocationToTP -- Teleport the LocalPlayer to the selected player's location
            else
                warn("Selected player does not have a HumanoidRootPart.")
            end
        else
            warn("No selected player or the selected player does not have a character.")
        end
        
    end,
 })


 local Shoot = Window:CreateTab("Combat", 4483362458) -- Title, Image

 local Section = Shoot:CreateSection("HitBox")


 local Players = game:GetService("Players")
 local RunService = game:GetService("RunService")
 local LocalPlayer = Players.LocalPlayer
 local originalSizes = {} -- Store original head sizes for all players
 local hitboxEnabled = false
 
 -- Function to scale the head hitbox
 local function scaleHeadHitbox(player, scale)
     if player.Character and player.Character:FindFirstChild("Head") then
         local head = player.Character.Head
         if not originalSizes[player] then
             originalSizes[player] = head.Size -- Save original size if not already saved
         end
         head.Size = originalSizes[player] * scale -- Scale the head
         head.CanCollide = false -- Disable collision for fairness
     end
 end
 
 -- Function to reset the head hitbox to its original size
 local function resetHeadHitbox(player)
     if player.Character and player.Character:FindFirstChild("Head") then
         local head = player.Character.Head
         if originalSizes[player] then
             head.Size = originalSizes[player] -- Reset to original size
         end
     end
 end
 
 -- Toggle the hitbox scaling on or off
 local function toggleHitbox(state)
     hitboxEnabled = state
     if not hitboxEnabled then
         -- Reset hitboxes when disabled
         for _, player in pairs(Players:GetPlayers()) do
             if player ~= LocalPlayer then
                 resetHeadHitbox(player)
             end
         end
     else
         -- Apply hitbox scaling when enabled
         for _, player in pairs(Players:GetPlayers()) do
             if player ~= LocalPlayer then
                 scaleHeadHitbox(player, 2) -- Scale once, no need to repeatedly do this
             end
         end
     end
 end
 
 -- Function to handle when a player's character spawns
 local function onCharacterSpawned(player)
     if hitboxEnabled then
         local head = player.Character:WaitForChild("Head", 10) -- Wait for head to load
         if head then
             scaleHeadHitbox(player, 2) -- Apply the scaling only once when character is loaded
         end
     end
 end
 
 -- Handle new players and respawns
 local function onPlayerAdded(player)
     if player.Character then
         onCharacterSpawned(player) -- Scale immediately if the character already exists
     end
 
     -- Connect character respawn events
     player.CharacterAdded:Connect(function()
         onCharacterSpawned(player)
     end)
 end
 
 -- Connect to existing players
 for _, player in pairs(Players:GetPlayers()) do
     if player ~= LocalPlayer then
         onPlayerAdded(player)
     end
 end
 
 -- Connect to new players joining the game
 Players.PlayerAdded:Connect(function(player)
     if player ~= LocalPlayer then
         onPlayerAdded(player)
     end
 end)
 
 -- Reset hitbox when players leave
 Players.PlayerRemoving:Connect(function(player)
     resetHeadHitbox(player)
 end)
 
 -- GUI toggle button for hitbox scaling
 local Toggle = Shoot:CreateToggle({
     Name = "HitBox",
     CurrentValue = false,
     Flag = "Toggle1", -- A flag is the identifier for the configuration file
     Callback = function(state)
         toggleHitbox(state)
     end,
 })




 



 
