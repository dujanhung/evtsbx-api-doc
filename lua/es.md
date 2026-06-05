# <code>es</code>

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

# minimap

```lua
es
function onPlace()->nil:end
function start()->nil:end
function update()->nil:end
function fixedUpdate()->nil:end
```

___

# constructor description

<table><tr><td>

```lua
es
```

<code>getter</code>

construct **Evertech Sandbox API** instance.

</td></tr></table>

___

# method description

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

called during screen rendering frame iteration.

___

```lua
function fixedUpdate()->nil:
 
end
```

<code>virtual</code>

called during physics rendering frame iteration, usually about 50 FPS.