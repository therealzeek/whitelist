local WhitelistedUserIds = {
    ["243805732"] = true, --
    ["2233820804"] = true,
    ["5367063377"] = true,
    ["2502514909"] = true,
    ["4442411184"] = true
}

local Player = game.Players.LocalPlayer

local function isWhitelisted(player)
    local userId = tostring(player.UserId)
    return WhitelistedUserIds[userId] == true
end

if isWhitelisted(Player) then
loadstring(game:HttpGet("loadstring(game:HttpGet("https://raw.githubusercontent.com/therealzeek/Nara.cc/main/script1.lua", true))()", true))()
else
    print("You are not whitelisted")
end
