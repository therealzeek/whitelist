local WhitelistedUserIds = {
    ["243805732"] = true, --
    ["2233820804"] = true,
    ["3297713064"] = true,
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
loadstring(game:HttpGet("https://raw.githubusercontent.com/therealzeek/Nara.cc/main/script.md", true))()
else
    print("You are not whitelisted")
end
