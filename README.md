lua

local player = game.Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")


function AutoGol()
    while true do
        wait(1)
        print("Gol marcado!")
    end
end


function StaminaInfinita()
    while true do
        wait(0.1)
        player.Stamina.Value = math.huge
    end
end


function InfiniteFluxo()
    while true do
        wait(0.1)
        print("Fluxo ativado!")
    end
end


print("Escolha uma opção:")
print("1. Auto Gol")
print("2. Stamina Infinita")
print("3. Infinite Fluxo")

local choice = io.read()

if choice == "1" then
    AutoGol()
elseif choice == "2" then
    StaminaInfinita()
elseif choice == "3" then
    InfiniteFluxo()
else
    print("Opção inválida!")
end
