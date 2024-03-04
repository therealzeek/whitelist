local WhitelistedUserIds = {
    ["243805732"] = true,
    ["2233820804"] = true,
    ["5367063377"] = true,
    ["2502514909"] = true,
    ["4999596731"] = true
}

local function isWhitelisted(player)
    local playerId = tostring(player.UserId)
    return WhitelistedUserIds[playerId] == true
end

if isWhitelisted(Player) then
    loadstring(game:HttpGet("https://raw.githubusercontent.com/therealzeek/whitelist/main/whitelist.md"))()
else
    print("You are not whitelisted")
end
