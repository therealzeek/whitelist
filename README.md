local WhitelistedUserIds = {
    ["urprofileid"] = true, --
}

local Player = game.Players.LocalPlayer

local function isWhitelisted(player)
    local userId = tostring(player.UserId)
    return WhitelistedUserIds[userId] == true
end

if isWhitelisted(Player) then
loadstring(game:HttpGet("https://raw.githubusercontent.com/scripthubekitten/reddot1/main/reddot1", true))()
else
    print("You are not whitelisted")
end
