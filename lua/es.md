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
ESAPI es            getter
nil   onPlace()     virtual
nil   start()       virtual
nil   update()      virtual
nil   fixedUpdate() virtual
```

___

# constructor description

<table><tr><td>

```lua
es
```

```lua
return ESAPI
```

<code>getter</code>

construct **Evertech Sandbox API** instance.

</td></tr></table>

___

# virtual method description

<table><thread><tr><td>

```lua
function onPlace()->nil:
 
end
```

called when player place this MOD block.

</td></tr></thread><tbody><tr><td>

```lua
function start()->nil:
 
end
```

called when player place this MOD block, or this MOD block is loaded from world file.

</td></tr></tbody><thread><tr><td>

```lua
function update()->nil:
 
end
```

called during screen rendering frame iteration.

</td></tr></thread><tbody><tr><td>

```lua
function fixedUpdate()->nil:
 
end
```

called during physics rendering frame iteration, usually about 50 FPS.

</td></tr></tbody></table>