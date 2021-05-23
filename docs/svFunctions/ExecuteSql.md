```lua
HVCore.Functions.ExecuteSql(wait, query, cb)
```

| Argument | Description | Required |
| ----------- | ----------- | ----------- |
| @wait | If the thread waits for the query to complete before returning | true |
| @query | The SQL query to run | true |
| @cb | Callback Function | true |

Executes and SQL query

Example:
```lua
HVCore.Functions.ExecuteSql(true, "SELECT * FROM table WHERE column = '" .. columnSpecific .. "'", function(result)
		print(result)
    end)
```