=== "Client"
    ``` lua
    TriggerEvent('chat:addMessage', {
        template = '<div class="chat-message system"><b>SYSTEM</b>: Test Chat Message!</div>',
        args = { message }
    })
    ```

=== "Server"
    ```lua
    TriggerClientEvent('chat:addMessage', source, {
        template = '<div class="chat-message success"><b>SUCCESS</b>: Test Chat Message!</div>',
        args = { message }
    })
    ```

####COLORS
<ul>
    <li style= "width: 20px; height: 20px; border: none; border-radius: 50%; background-color: rgb(47, 92, 115);"> <code style="margin-left: 30px; word-break: normal;">advert</code> </li>
    <li style= "width: 20px; height: 20px; border: none; border-radius: 50%; background-color: rgb(184, 41, 41);"> <code style="margin-left: 30px; word-break: normal;">server</code> </li>
    <li style= "width: 20px; height: 20px; border: none; border-radius: 50%; background-color: rgb(67, 57, 111);"> <code style="margin-left: 30px; word-break: normal;">system</code> </li>
    <li style= "width: 20px; height: 20px; border: none; border-radius: 50%; background-color: rgb(224, 50, 50);"> <code style="margin-left: 30px; word-break: normal;">emergency</code> </li>
    <li style= "width: 20px; height: 20px; border: none; border-radius: 50%; background-color: rgb(112, 25, 25);"> <code style="margin-left: 30px; word-break: normal;">nonemergency</code> </li>
    <li style= "width: 20px; height: 20px; border: none; border-radius: 50%; background-color: rgb(77, 189, 77);"> <code style="margin-left: 30px; word-break: normal;">success</code> </li>
    <li style= "width: 20px; height: 20px; border: none; border-radius: 50%; background-color: rgb(201, 130, 38);"> <code style="margin-left: 30px; word-break: normal;">number</code> </li>
    <li style= "width: 20px; height: 20px; border: none; border-radius: 50%; background-color: rgb(38, 81, 201);"> <code style="margin-left: 30px; word-break: normal;">jail</code> </li>
</ul>