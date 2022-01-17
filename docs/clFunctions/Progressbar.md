```lua
TriggerEvent("HiveHud:StartProg", duration, color, useWhileDead, canCancel, disabledControls, animation, cb
```


| Argument | Description | Type | Required |
| ----------- | ----------- | ----------- | ----------- |
| @duration | The time is takes to complete the progress bar | Int | true |
| @color | Color of the progress bar (Can be Hex or Name) Defaults to lime green | string | false |
| @useWhileDead | Whether or not the progbar can start while the player is dead | Bool | true |
| @canCancel | Whether or not the player can cancel the progbar | Bool | true |
| @disabledControls | The controls that should be disabled when the progbar is active | table | true |
| @animation | The animation that plays while the progbar is active | table | true |
| @cb | The function that is called when the progress bar is complete or canceled | function | true |

Starts a progress bar

#Example
```lua
TriggerEvent("HiveHud:StartProg", 3000, nil, false, true, { 
    mouse = false, move = false, car = false, combat = true -- // true = disabled
}, {
    dict = "timetable@ron@ig_4_smoking_meth", anim = "chefiscookingup", flag = 16
}, function(success)
    if not success then return end
    print("You smoked Meth!")
end)
```

!!! note "Disable Movement Types"
    - [mouse] - Disable Camera Movement
    - [move] - Disables Player Movement
    - [car] - Disabled Car Movement
    - [combat] - Disabled Combat Controls