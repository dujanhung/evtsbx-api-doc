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

___

<h2>
property description
</h2>

```lua
es.TimeScale
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
<code>float</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
default
</td><td>
|
</td><td>
<code>1.0</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
range
</td><td>
|
</td><td>
more than <code>0.0</code>
</td></tr></table>

change time scale.

>[!IMPORTANT]
>time scale could be reset via pause menu, and upon world file reload.

___

```lua
es.DeltaTime
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
<code>float</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
range
</td><td>
|
</td><td>
more than <code>0.0</code>
</td></tr></table>

the time between screen rendering frames.

___

```lua
es.FixedDeltaTime
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
<code>float</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
range
</td><td>
|
</td><td>
more than <code>0.0</code>
</td></tr></table>

the time between physics rendering frames. usually about <code>0.02</code> .