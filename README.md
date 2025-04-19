local 10101918 = game:GetService("MarketplaceService")
local 10101918 = game:GetService("Players")
local 10101918 = Players.LocalPlayer

-- ID do Gamepass ou Developer Product que você quer vender
local itemId = 10101918 -- Substitua pelo ID correto
local isGamepass = true -- true para Gamepass, false para Developer Product

script.Parent.MouseButton1Click:Connect(function()
    if isGamepass then
        MarketplaceService:PromptGamePassPurchase(player, itemId)
    else
        MarketplaceService:PromptProductPurchase(player, itemId)
    end
end)
