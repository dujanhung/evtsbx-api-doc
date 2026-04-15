<h2>
<code>es.Player</code>
</h2>

<table><tr><td>
inherit
</td><td>
|
</td><td>
<code>es</code>
</td></tr></table>

an "Evertech Sandbox" player.

>[!IMPORTANT]
>"Evertech Sandbox" API don't support multiplayer, due to security reasons.

>[!IMPORTANT]
>"Evertech Sandbox" API don't support any methods that could change player skin, force changes to player inventory, force player to enter or exit the seat, toggle jetpack.

___

<h2>
property description
</h2>

```lua
es.Player.Position
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>getter</code>
<br>
<code>setter</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
type
</td><td>
|
</td><td>
<code>Array(float)</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
default
</td><td>
|
</td><td>
<code>{0.0,0.0,0.0}</code>
</td></tr></table>

the player position in world coordinate. use XYZ convention.

>
>

>[!CAUTION]
>don't teleport the player too far away. otherwise, player would get stuck in the black void.

___

```lua
es.Player.CameraPosition
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>getter</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
type
</td><td>
|
</td><td>
<code>Array(float)</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
default
</td><td>
|
</td><td>
<code>{0.0,0.0,0.0}</code>
</td></tr></table>

the player camera position in world coordinate, including seat's camera. use XYZ convention.

>[!TIP]
>by default, player camera position would have an offset of 4 blocks upwards, which would be useful to detect if player were entering the seat in orbit mode.