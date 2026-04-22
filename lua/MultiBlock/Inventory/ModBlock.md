<h2>
<code>es.MultiBlock.ModBlock</code>
</h2>

<table><tr><td>
inherit
</td><td>
|
</td><td>
<code>es.MultiBlock</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
<code>es.MultiBlock.Type</code> specific
</td><td>
|
</td><td>
<code>SimpleModBlock</code>
<br>
<code>WheelModBlock</code>
<br>
<code>SizableWheelModBlock</code>
</td></tr></table>

represents a MOD block from **Evertech Sandbox Lua API**.

this block could send message to other blocks.

___

<h2>
constructor
</h2>

```lua
es.MultiBlock.ModBlock
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
<code>MODBLOCKAPI</code>
</td></tr></table>

get MOD block's instance.

___

<h2>
virtual method description
</h2>

```lua
function message(msg)
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

<table><tr><td>
mandatory
</td><td>
|
</td><td>
<code>msg</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
type
</td><td>
|
</td><td>
<code>Variant</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
description
</td><td>
|
</td><td>
message content
</td></tr></table>

called when another MOD block use `es.MultiBlock.ModBlock.send()` at this block.

___

<h2>
method description
</h2>

```lua
es.MultiBlock.ModBlock.send(msg)
```

<table><tr><td>
return type
</td><td>
|
</td><td>
<code>void</code>
</td></tr></table>

<table><tr><td>
mandatory
</td><td>
|
</td><td>
<code>msg</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
type
</td><td>
|
</td><td>
<code>Variant</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
description
</td><td>
|
</td><td>
message content
</td></tr></table>

send message to another MOD block.