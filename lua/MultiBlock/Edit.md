<h2>
<code>es.MultiBlock.Modify</code>
</h2>

<table><tr><td>
expands
</td><td>
|
</td><td>
<code>es</code>
</td></tr></table>

a helper class to modify blocks.

___

<h2>
method description
</h2>

```lua
es.CreateMultiblock(blockType,root,relPos,relRot,modUuid)
```

<table><tr><td>
return type
</td><td>
|
</td><td>
<code>es.MultiBlock</code>
</td></tr></table>

<table><tr><td>
mandatory
</td><td>
|
</td><td>
<code>blockType</code>
</td><td>
<code>root</code>
</td><td>
<code>relPos</code>
</td><td>
<code>relRot</code>
</td><td>
<code>modUuid</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td><td>
</td><td>
</td><td>
</td><td>
</td></tr><tr><td>
type
</td><td>
|
</td><td>
<code>String</code>
</td><td>
<code>es.MultiBlock.Root</code>
</td><td>
<code>{float,float,float}</code>
</td><td>
<code>es.Quaternion.Euler(float,float,float)</code>
</td><td>
<code>String</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td><td>
</td><td>
</td><td>
</td><td>
</td></tr><tr><td>
range
</td><td>
|
</td><td>
listed in <a href="https://github.com/dujanhung/evtsbx-api-doc/blob/main/enum/block_type.md">this enum</a>
</td><td>
</td><td>
satisfy <code>Math.sqrt(x^2+y^2+z^2)>=1</code>
</td><td>
</td><td>
depends on <code>info.json</code> from every mods
</td></tr><tr><td>
</td><td>
</td><td>
</td><td>
</td><td>
</td><td>
</td><td>
</td></tr><tr><td>
range
</td><td>
|
</td><td>
</td><td>
</td><td>
</td><td>
</td><td>
</td><td>
</td></tr><tr><td>
description
</td><td>
|
</td><td>
block's type
</td><td>
block's root
</td><td>
block's relative position, use XYZ convention, use <code>0.5</code> unit
</td><td>
block's relative rotation, use XYZ convention
</td><td>
MOD block's uuid
</td></tr></table>