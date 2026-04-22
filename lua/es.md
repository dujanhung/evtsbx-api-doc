<h2>
<code>es</code>
</h2>

<table><tr><td>
inherit
</td><td>
|
</td><td>
<code>userdata</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
inherited by
</td><td>
|
</td><td>
<code>es.Player</code>
<br>
<code>es.MultiBlock</code>
<br>
<code>es.Quaternion</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
expanded by
</td><td>
|
</td><td>
<code>es.GUI</code>
<br>
<code>es.Sensor</code>
<br>
<code>es.IO</code>
<br>
<code>es.Audio</code>
<br>
<code>es.Material</code>
<br>
<code>es.Time</code>
</td></tr></table>

represents **Evertech Sandbox Lua API**.

___

<h2>
constructor
</h2>

```lua
es
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
<code>ESAPI</code>
</td></tr></table>

access to "Evertech Sandbox" instance.

___

<h2>
virtual method description
</h2>

```lua
function onPlace()
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>virtual</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
return type
</td><td>
|
</td><td>
<code>void</code>
</td></tr></table>

called when player place this MOD block.

___

```lua
function start()
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>virtual</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
return type
</td><td>
|
</td><td>
<code>void</code>
</td></tr></table>

called when player place this MOD block, or this MOD block is loaded from world file.

___

```lua
function update()
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>virtual</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
return type
</td><td>
|
</td><td>
<code>void</code>
</td></tr></table>

called via screen rendering frame iteration.

___

```lua
function fixedUpdate()
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>virtual</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
return type
</td><td>
|
</td><td>
<code>void</code>
</td></tr></table>

called via physics rendering frame iteration, usually about 50 FPS.