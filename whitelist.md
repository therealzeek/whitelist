local WhitelistedUserIds = {
    ["243805732"] = true, --
    ["buyer"]
}

local Player = game.Players.LocalPlayer

local function isWhitelisted(player)
    local userId = tostring(player.UserId)
    return WhitelistedUserIds[userId] == true
end

if isWhitelisted(Player) then
loadstring("https://raw.githubusercontent.com/therealzeek/aura.cc/main/README.md")()
else
    print("You are not whitelisted")
end
