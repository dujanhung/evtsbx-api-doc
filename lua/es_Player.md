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

>[!NOTE]
>unless otherwise noted, "Evertech Sandbox" use XYZ convention.

>[!IMPORTANT]
>"Evertech Sandbox" API don't support multiplayer, due to security reasons.

>[!IMPORTANT]
>"Evertech Sandbox" API don't support any methods that could change player skin, force changes to player inventory, force player to enter or exit the seat, toggle jetpack, force player to crouch, force player to jump.

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
<code>{float,float,float}</code>
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

the player position in world coordinate.

>[!TIP]
>this one is useful for player teleportation, and player movement recorder.

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
<code>{float,float,float}</code>
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

the player camera position in world coordinate, including seat's camera.

>[!TIP]
>this one is used for player tool blocks to follow player's camera, even though if player is crouching, or sitting in the seat.

>[!TIP]
>to calculate player's up direction, use this one together with `es.Player.Position` .

>[!CAUTION]
>don't always rely on this one to calculate player's up direction, because it would become incorrect if player was sitting in the seat and enable orbit mode.

___

```lua
es.Player.Rotation
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
<code>es.Quaternion.Euler(float,float,float)</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
default
</td><td>
|
</td><td>
<code>es.Quaternion.Euler(0.0,0.0,0.0)</code>
</td></tr></table>

the player rotation in world coordinate.

>[!TIP]
>this one is used for MOD seat, to replace the built-in seat blocks.

>[!CAUTION]
>don't use this one to force "drunk" player, as it would cause health risks.

___

```lua
es.Player.CameraRotation
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
<code>es.Quaternion.Euler(float,float,float)</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
default
</td><td>
|
</td><td>
<code>es.Quaternion.Euler(0.0,0.0,0.0)</code>
</td></tr></table>

the player camera rotation in world coordinate, including seat's camera.

>[!TIP]
>this one is used for player recorder.

>[!CAUTION]
>don't use this one to force "drunk" player, as it would cause health risks.

___

```lua
es.Player.CameraDirection
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
<code>{float,float,float}</code>
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

the player camera direction in world coordinate, including seat's camera.
