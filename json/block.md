<h2>
MOD_block
</h2>

a MOD block data.

___

```json
"uuid|@required,@unique":"str"
```

MOD block UUID.

___

```json
"name|@required":"str"
```

MOD block name.

___

```json
"description|@required":"str"
```

MOD block description.

___

```json
"icon|@required,filepath_flag(png)":"str"
```

icon texture filepath.

___

```json
"dif|@required,filepath_flag(png)":"str"
```

albedo texture filepath.

> [!WARNING]
> this entry may be changed in the future.

___

```json
"nor|filepath_flag(png)":"str"
```

normal texture filepath.

> [!WARNING]
> this entry may be changed in the future.

___

```json
"met|filepath_flag(png)":"str"
```

metallic texture filepath.

> [!WARNING]
> this entry may be changed in the future.

___

```json
"mesh|@required,filepath_flag(obj)":"str"
```

OBJ filepath.

___

```json
"script|filepath_flag(lua)":"str"
```

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

change collider type.

look up this enum.

> [!WARNING]
> this entry may be changed in the future.

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

> [!WARNING]
> this entry may be changed in the future.

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

> [!WARNING]
> this entry may be changed in the future.

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

> [!WARNING]
> this entry may be changed in the future.

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

> [!WARNING]
> this entry may be changed in the future.

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

> [!WARNING]
> this entry may be changed in the future.

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