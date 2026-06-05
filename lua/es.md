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
function onPlace()->nil:
 
end
```

<code>virtual</code>

called when player place this MOD block.

___

```lua
function start()->nil:
 
end
```

<code>virtual</code>

called when player place this MOD block, or this MOD block is loaded from world file.

___

```lua
function update()->nil:
 
end
```

<code>virtual</code>

called via screen rendering frame iteration.

___

```lua
function fixedUpdate()->nil:
 
end
```

<code>virtual</code>

called during physics rendering frame iteration, usually about 50 FPS.