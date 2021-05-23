# Welcome to Hive Documentation

Client:
```lua
QBCore = nil
Citizen.CreateThread(function() 
	while QBCore == nil do
		TriggerEvent('QBCore:GetObject', function(obj) QBCore = obj end)
		Citizen.Wait(0)
	end
end)
```

Server:
```perl
QBCore = nil
TriggerEvent('QBCore:GetObject', function(obj) QBCore = obj end)
```