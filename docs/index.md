# Welcome to Hive Documentation

Client:
```lua
HVCore = nil
Citizen.CreateThread(function() 
	while HVCore == nil do
		TriggerEvent('HVCore:GetObject', function(obj) HVCore = obj end)
		Citizen.Wait(0)
	end
end)
```

Server:
```lua
HVCore = nil
TriggerEvent('HVCore:GetObject', function(obj) HVCore = obj end)
```