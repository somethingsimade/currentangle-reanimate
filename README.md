# currentangle reanimate
stable currentangle reanimate with some more settings

# httpget
```lua
-- SETTINGS --
local settings = _G

settings["Use default animations"] = true
settings["Fake character transparency level"] = 0 -- 0 to disable
settings["Disable character scripts"] = true
settings["Fake character should collide"] = true
settings["Names to exclude from transparency"] = {
    --[[ example:
    ["HumanoidRootPart"] = true,
    ["Left Arm"] = true
    ]]
}
(function() if getgenv then return getgenv() else return _G end end)().fling = nil
local finished = false

task.spawn(function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/somethingsimade/currentangle-reanimate/refs/heads/main/main"))()
end)

repeat task.wait() until finished

-- USAGE: getgenv().fling(character, time, yield) if you dont have getgenv: _G.fling(character, time, yield)
-- or just fling(character, time, yield)

-- time is for how much time in seconds it will fling
-- the character

-- yield is if the fling function will yield

-- you can put your converted script under here

```

credits
This code was shared publicly by https://v3rm.net/members/presidentanvil.30546/ and/or
https://v3rm.net/members/sammyc.16754/ and no license was provided. If you would like it removed, please contact me.
