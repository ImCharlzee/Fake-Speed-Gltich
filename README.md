local words = {
    'ur bad',
    'ez',
    'im not locking ur just bad',
    'get better',
    'clown',
    'ez',
    'how did u miss that many shots',
    'I can write a whole book about how bad you are',
    'dog',
    'kid',
    'aim kid',
    'where is your aim?',
    'if you had money I would reccomend buying a coach',
    'Sonned',
    'you can get star.... in a 10yrs 😂',
    '😂😂😂😂',
    'Mad',
    '1v1... jk your too bad you will lose',
    'Go Get A level 0 exploiter',
    'Get A Flame Next Time You Will Need it 😂',
    'You Be Looking Like 🙃This🙃 when I air Shoot you',
    'You want Flame? Wont even Help You',
    'Wanna try Rpg Lol go spend 50k money for ammo U wont Hit me.',
    'Seed',
    'dog',
    'imagine',
    'cat eve aim bro',
    'I wanna see you try.',
    'lol',
    'ur christmas list should have aim on it ',
}
local player = game.Players.LocalPlayer
local keybind = 'e'

local event = game.ReplicatedStorage.DefaultChatSystemChatEvents.SayMessageRequest

player:GetMouse().KeyDown:connect(function(key)
    if key == keybind then
        event:FireServer(words[math.random(#words)], "All")
    end
end)
