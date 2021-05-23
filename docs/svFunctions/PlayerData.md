```lua
QBCore.Functions.GetPlayer(source)
```

Loads the players Data

Player Data consists of:

| Data | Description |
| ----------- | ----------- |
| PlayerData.money | Returns a table of the players money (cash, bank & crypto) |
| PlayerData.job | Returns a table of the player job (name, label, payment, onduty) |
| PlayerData.position | Returns the players saved position |
| PlayerData.metadata | Returns a table of the players Metadata (hunger, thirst, licenses, commandbindings, fingerprint etc.) |
| PlayerData.charinfo | Returns a table of the player Character Data (cid, nationality, First & Last name, Phone#, DOB, AccountID & Gender) |
| PlayerData.citizenid | Returns the characters Citizen ID |
| PlayerData.steam | Returns the players Steam ID |
| PlayerData.license | Returns the players R* License |
| PlayerData.name | Returns the players name (This just calls GetPlayerName()) |
| PlayerData.cid | Returns the players CID (Should use PlayerData.citizenid as this is always 1) |

Player Functions:

| Function | Description |
| ----------- | ----------- |
| PlayerData.Functions.SetJob(job) | Sets the players job |
| PlayerData.Functions.SetJobDuty(onDuty) | Sets the player to being on/off duty |
| PlayerData.Functions.AddJobReputation(amount) | Adds players job reputation |
| PlayerData.Functions.SetMetaData(meta, val) | Sets specified metadata to the given value |
| PlayerData.Functions.AddMoney(moneytype, amount, reason) | Adds money to the player |
| PlayerData.Functions.RemoveMoney(moneytype, amount, reason) | Removes money from the player |
| PlayerData.Functions.SetMoney(moneytype, amount, reason) | Sets players money |
| PlayerData.Functions.AddItem(item, amount, slot, info) | Adds Item to players inventory [slot and info are optional] |
| PlayerData.Functions.RemoveItem(item, amount, slot) | Removes Item from players inventory [slot is optional] |
| PlayerData.Functions.SetInventory(items) | Sets the inventory of a player |
| PlayerData.Functions.ClearInventory() | Clears the inventory of a player |
| PlayerData.Functions.GetItemByName(item) | Gets the given items data |
| PlayerData.Functions.GetItemBySlot(slot) | Gets the item from the given slot |
| PlayerData.Functions.Save() | Saves the players data |