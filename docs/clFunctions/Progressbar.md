```lua
HVCore.Functions.Progressbar(name, label, duration, useWhileDead, canCancel, disableControls, animation, prop, propTwo, onFinish, onCancel)
```


| Argument | Description | Type | Required |
| ----------- | ----------- | ----------- | ----------- |
| @name | Name (think this is used to keep track of what progressbar it is) | String | true |
| @label | The text shown on the progressbar | String | true |
| @duration | The time is takes to complete the progress bar | Int | true |
| @useWhileDead | Whether or not the progbar can start while the player is dead | Bool | true |
| @canCancel | Whether or not the player can cancel the progbar | Bool | true |
| @disableControls | The controls that should be disabled when the progbar is active | table | true |
| @animation | The animation that plays while the progbar is active | table | true |
| @prop | A prop that displays while the progbar is active | table | true |
| @propTwo | A 2nd prop that displays while the progbar is active | table | true |
| @onFinish | A function that is called when the progbar is completed successfully | function | true |
| @onCancel | A function that is called when the progbar is failed/canceled | function | false |

Starts a progress bar

#Example
-
```lua
    HVCore.Functions.Progressbar("prog_bar", "Doing Progress..", 5000, false, true, {}, {}, {}, {}, function() -- // Done
        print("Progress Bar Finished!")
    end, function() -- // Cancel
        print("Progress Bar Canceled")
    end)
```

Disable Movement Types
----
- disableMouse
- disableMovement
- disableCarMovement
- disableCombat