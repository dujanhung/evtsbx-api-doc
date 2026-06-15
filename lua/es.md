# <code>es</code>

represents an **Evertech Sandbox API** entry.

---

# inheritance

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

___

# minimap

┣ 🛠️ constructors<br>
┃ ┗ [`es`](#constructor_es)<br>
┣ 🛰️ virtual methods<br>
┃ ┣ [`onPlace()`](#method_virtual_onPlace)<br>
┃ ┣ [`start()`](#method_virtual_start)<br>
┃ ┣ [`update()`](#method_virtual_update)<br>
┃ ┗ [`fixedUpdate()`](#method_virtual_fixedUpdate)

___

# constructor description

## <code id="constructor_es">es</code>

```lua
es
```

```lua
return ESAPI
```

<code>getter</code>

construct **Evertech Sandbox API** instance.

___

# virtual method description

## <code id="method_virtual_onPlace">onPlace()</code>

```lua
function onPlace()

end
```

called when player place this MOD block.

## <code id="method_virtual_start">start()</code>

```lua
function start()

end
```

called when player place this MOD block, or this MOD block is loaded from world file.

## <code id="method_virtual_update">update()</code>

```lua
function update()

end
```

called during screen rendering frame iteration.

## <code id="method_virtual_fixedUpdate">fixedUpdate()</code>

```lua
function fixedUpdate()

end
```

called during physics rendering frame iteration, usually about 50 FPS.