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
"collider|enum(wheel,sizable_wheel)":"str"
```

change collider type.

look up this enum.

> [!WARNING]
> this entry may be changed in the future.

___

```json
"normScale|range_flag(exp)":"float"
```

normal texture repeat scale.

> [!WARNING]
> this entry may be changed in the future.

___

```json
"smoothness|range_flag(linear)":"float"
```

metallic texture smoothness.

> [!WARNING]
> this entry may be changed in the future.

___

```json
"scale|range_flag(exp)":"float"
```

OBJ scale.

> [!WARNING]
> this entry may be changed in the future.

___

```json
"colliderOptions|need(collider.value==collider.enum.slot(2))":"dict"
```

`SizableWheelModBlock` collider options.

> [!WARNING]
> this entry may be changed in the future.

___

```json
"meshOptions|need(collider.value==collider.enum.slot(2))":"dict"
```

`SizableWheelModBlock` mesh options.

> [!WARNING]
> this entry may be changed in the future.

___

```json
"connections|array_flag(allow_multiple)":"list"
```

a list of connection points.