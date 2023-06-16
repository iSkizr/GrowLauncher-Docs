# GrowLauncher-Docs
GrowLauncher is a Modded Growtopia Game

# Functions 

* [SendPacket](#SendPacket)
* [LogToConsole](#LogToConsole)
* [Sleep](#Sleep)
* [FindItemID](#FindItemID)
* [FindPath](#FindPath)

# SendPacket
To Send a Packet to Growtopia server
```lua
SendPacket(2, "action|input\ntext|Hello !")
```

# LogToConsole
To Print String into Growtopia Console
```lua
LogToConsole("Growtopia")
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
