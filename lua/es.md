<h2>
<code>es</code>
</h2>

<table><thread><tr><td>
inherit
</td><td>
<code>userdata</code>
</td></tr></thread><tbody><tr><td>
inherited by
</td><td>
<code>es.Player</code>
<br>
<code>es.MultiBlock</code>
<br>
<code>es.Quaternion</code>
</td></tr></tbody></table>

represents **Evertech Sandbox API**.

___

<h2>
constructor
</h2>

```lua
es
```

```lua
return ESAPI
```

<code>getter</code>

represents **Evertech Sandbox API** instance.

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