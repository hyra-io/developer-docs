---
description: >-
  A simple API wrapper module script to allow you to interact with the API more
  easily.
---

# Roblox Module

Here's an example script on the implementation of the Roblox Module.

```lua
local Ranking = require(4754168383) -- Require the module
local Token = "TOKEN" -- Replace TOKEN with your Token

local Callback = Ranking.SetRank(Token, PLAYER-USER_ID, GROUPID, RANKID)
if Callback.Success == true then
    -- Ranking Succeeded
else
    -- Ranking failed
end
```

Simply edit the **`Token`**variable to be your token and use your own Player User ID, Group ID and Rank ID when invoking the command.

For each reference in a singular script, you only need line 4 and below, as the top two lines are used to initiate the system.

Though the require\(\) module is open source, we don't advise using your own version, as you may lose out on updates and functionality may stop at any point.

