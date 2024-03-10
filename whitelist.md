-- Define the list of whitelisted user IDs
local WhitelistedUserIds = {
    ["243805732"] = true,
    ["2233820804"] = true,
    ["5367063377"] = true,
    ["2502514909"] = true,
    ["4999596731"] = true,
    ["1833432678"] = true,
    ["5087780867"] = true,
    ["4964439299"] = true,
    ["1281241466"] = true,
    ["390527725"] = true,
    ["3576792553"] = true,
    ["4212790915"] = true
    -- Add more user IDs as needed
}

-- Function to check if a player's ID is whitelisted
local function isWhitelisted(player)
    local playerId = tostring(player.UserId)
    return WhitelistedUserIds[playerId] == true
end

-- Check if the player's ID is whitelisted
local player = game.Players.LocalPlayer
if player and player:IsA("Player") and isWhitelisted(player) then
    loadstring(game:HttpGet("https://raw.githubusercontent.com/therealzeek/Nara.cc/main/script1.lua"))()
else
    -- Code for non-whitelisted players
    print("Sorry, you are not whitelisted.")
    -- You can kick or restrict access for non-whitelisted players here
end
