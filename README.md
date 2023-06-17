# GrowLauncher-Docs
GrowLauncher is a Modded Growtopia Game

# Functions 

* [SendPacket](#SendPacket)
* [LogToConsole](#LogToConsole)
* [Sleep](#Sleep)
* [FindItemID](#FindItemID)
* [FindPath](#FindPath)
* [Error](#Error)
* [GetLocal](#GetLocal)
* [GetTiles](#GetTiles)
* [GetTile](#GetTile)
* [GetInventory](#GetInventory)

# SendPacket
To Send a Packet to Growtopia server
```lua
SendPacket(2, "action|input\ntext|Hello !")
```

# LogToConsole
To Print String into Growtopia Console
```lua
LogToConsole("This is Console Message")
```

# Sleep
To add cooldown in your script
```lua
Sleep(1000)
-- 1 sec
```

# FindItemID
To get item id by name
```lua
FindItemID("Dirt")
```

# FindPath
Auto teleport to other position
```lua
FindPath(20, 21)
```
# Error
To add fake error message
```lua
error("This is error message")
```
# GetLocal
Local Player
```lua
-- List Struct:
local GetLocal = {
posX,
posY,
netID,
name,
userID,
country,
punchID,
guildflag,
isLeft,
posXenc,
posYenc,
sizeX,
sizeY,
sizeXenc,
sizeYenc,
waterSpeed
}

-- Example
GetLocal().name
```

# GetTiles
To get all tiles in the World
```lua
-- Note:
-- tiles.fg = foreground
-- tiles.bg = background
for _, tiles in pairs(GetTiles()) do
if tiles.fg == 2 then
LogToConsole("Many Dirt!")
end
end
```

# GetTile
To Get Tile Data
```lua
GetTile(23, 25)
```

# GetInventory
```lua
-- List Struct:
local GetInventory = {
id,
amount
}

-- Example:
for _, inv in pairs(GetInventory()) do
if inv.id == 2 then
LogToConsole("You have "..inv.amount "dirt!")
end
end
```
