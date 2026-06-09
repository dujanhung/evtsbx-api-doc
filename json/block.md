<h2>
MOD_block
</h2>

a MOD block's data.

<table><thread><tr><td>

```json
"uuid|@required,@unique":"str"
```

MOD block UUID.

</td></tr></thread><tbody><tr><td>

```json
"name|@required":"str"
```

MOD block name.

</td></tr></tbody><thread><tr><td>

```json
"description|@required":"str"
```

MOD block description.

</td></tr></thread><tbody><tr><td>

```json
"icon|@required,filepath_flag(png)":"str"
```

icon texture filepath.

</td></tr></tbody><thread><tr><td>

```json
"dif|@required,filepath_flag(png)":"str"
```

albedo texture filepath.

> [!WARNING]
> this entry may be changed in the future.

</td></tr></thread><tbody><tr><td>

```json
"nor|filepath_flag(png)":"str"
```

normal texture filepath.

> [!WARNING]
> this entry may be changed in the future.

</td></tr></tbody><thread><tr><td>

```json
"met|filepath_flag(png)":"str"
```

metallic texture filepath.

> [!WARNING]
> this entry may be changed in the future.

</td></tr></thread><tbody><tr><td>

```json
"mesh|@required,filepath_flag(obj)":"str"
```

OBJ filepath.

</td></tr></tbody><thread><tr><td>

```json
"script|filepath_flag(lua)":"str"
```

Lua script filepath.

</td></tr></thread><tbody><tr><td>

```json
"collider|enum(wheel,sizable_wheel)":"str"
```

change collider type.

look up this enum.

> [!WARNING]
> this entry may be changed in the future.

</td></tr></tbody><thread><tr><td>

```json
"normScale|range_flag(exp)":"float"
```

normal texture repeat scale.

> [!WARNING]
> this entry may be changed in the future.

</td></tr></thread><tbody><tr><td>

```json
"smoothness|range_flag(linear)":"float"
```

metallic texture smoothness.

> [!WARNING]
> this entry may be changed in the future.

</td></tr></tbody><thread><tr><td>

```json
"scale|range_flag(exp)":"float"
```

OBJ scale.

> [!WARNING]
> this entry may be changed in the future.

</td></tr></thread><tbody><tr><td>

```json
"colliderOptions|condition(collider.value==collider.enum.slot(2))":"dict"
```

`SizableWheelModBlock` collider options.

> [!WARNING]
> this entry may be changed in the future.

</td></tr></tbody><thread><tr><td>

```json
"meshOptions|condition(collider.value==collider.enum.slot(2))":"dict"
```

`SizableWheelModBlock` mesh options.

> [!WARNING]
> this entry may be changed in the future.

</td></tr></thread><tbody><tr><td>

```json
"connections|list_flag(allow_multiple)":"list"
```

a list of connection points.

</td></tr></tbody></table>