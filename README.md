# currentangle reanimate
stable currentangle reanimate with some more settings

# httpget
```lua
-- SETTINGS --
local settings = _G

settings["Use default animations"] = true
settings["Fake character transparency level"] = 1 -- 0 to disable
settings["Disable character scripts"] = true

loadstring(game:HttpGet("https://raw.githubusercontent.com/somethingsimade/currentangle-reanimate/refs/heads/main/main"))()
