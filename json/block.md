<h2>
MOD_block
</h2>

a MOD block data.

___

```json
"uuid"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

MOD block UUID.

>[!CAUTION]
>this value must be unique among others from inside the `info.json` and from other MODs. otherwise, the conflict would happen.

___

```json
"name"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

MOD block name.

___

```json
"description"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

MOD block description.

___

```json
"icon"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

icon texture filepath.

___

```json
"dif"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table

albedo texture filepath.

___

```json
"nor"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

normal texture filepath.

___

```json
"met"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

metallic texture filepath.

___

```json
"mesh"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

3D mesh filepath.

___

```json
"script"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

Lua script filepath.

___

```json
"collider"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

collider. look up this enum.

___

```json
"normScale"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>float</code>
</td></tr></table>

normal texture repeate scale.

___

```json
"smoothness"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>float</code>
</td></tr></table>

metallic texture smoothness.

___

```json
"scale"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>float</code>
</td></tr></table>

3D mesh scale.

___

```json
"colliderOptions"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>MOD_collider_option</code>
</td></tr></table>

`SizableWheelModBlock` collider options.

___

```json
"meshOptions"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>MOD_mesh_option</code>
</td></tr></table>

`SizableWheelModBlock` mesh options.

___

```json
"connections"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>MOD_connection</code>
</td></tr></table>

connection.