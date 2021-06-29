```lua
local Player = HVCore.Functions.GetPlayerData()
```

Loads the players Data

Player Data consists of:

| Data | Description |
| ----------- | ----------- |
| Player.PlayerData.money | Returns a table of the players money (cash, bank & crypto) |
| Player.PlayerData.job | Returns a table of the player job (name, label, onduty, currentRank, rankPayment, rankLabel) |
| Player.PlayerData.position | Returns the players saved position |
| Player.PlayerData.metadata | Returns a table of the players Metadata (hunger, thirst, licenses, commandbindings, fingerprint etc.) |
| Player.PlayerData.charinfo | Returns a table of the player Character Data (cid, nationality, First & Last name, Phone#, DOB, AccountID & Gender) |
| Player.PlayerData.citizenid | Returns the characters Citizen ID |
| Player.PlayerData.steam | Returns the players Steam ID |
| Player.PlayerData.license | Returns the players R* License |
| Player.PlayerData.name | Returns the players name (This just calls GetPlayerName()) |
| Player.PlayerData.cid | Returns the players CID (Should use Player.PlayerData.citizenid as this is always 1) |

Player Functions:

| Function | Description |
| ----------- | ----------- |
| Player.Functions.SetJob(job) | Sets the players job |
| Player.Functions.SetJobDuty(onDuty) | Sets the player to being on/off duty |
| Player.Functions.AddJobReputation(amount) | Adds players job reputation |
| Player.Functions.SetMetaData(meta, val) | Sets specified metadata to the given value |
| Player.Functions.AddMoney(moneytype, amount, reason) | Adds money to the player |
| Player.Functions.RemoveMoney(moneytype, amount, reason) | Removes money from the player |
| Player.Functions.SetMoney(moneytype, amount, reason) | Sets players money |
| Player.Functions.AddItem(item, amount, slot, info) | Adds Item to players inventory [slot and info are optional] |
| Player.Functions.RemoveItem(item, amount, slot) | Removes Item from players inventory [slot is optional] |
| Player.Functions.SetInventory(items) | Sets the inventory of a player |
| Player.Functions.ClearInventory() | Clears the inventory of a player |
| Player.Functions.GetItemByName(item) | Gets the given items data |
| Player.Functions.GetItemBySlot(slot) | Gets the item from the given slot |
| Player.Functions.Save() | Saves the players data |