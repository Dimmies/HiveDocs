```lua
TriggerClientEvent('HVCore:Notify', source, text, notifType)
```

| Argument | Description | Required |
| ----------- | ----------- | ----------- |
| @source | Player Source | true |
| @text | Text displayed on the notification | true |
| @notifType | Type of the notification [primary, error or success] | false (Defaults to Primary)

Sends a notification to the specified player