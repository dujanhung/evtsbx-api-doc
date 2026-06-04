<h2>
MOD_header
</h2>

the "Evertech Sandbox" MOD header in JSON.

>[!IMPORTANT]
>"Evertech Sandbox" support `PNG` and `JPG` files. other files would fire an error.

___

```json
"name|@required":"str"
```

MOD name.

___

```json
"description|@required":"str"
```

MOD description.

___

```json
"author|@required,remap_flag(author)":"int"
```

MOD author name.

> [!NOTE]
> the value is restricted to a remap file.
>
> to assign your name, please visit a repo.

___

```json
"version"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

MOD version.

___

```json
"preview"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

MOD preview image filepath.

___

```json
"simpleblocks"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>Array[MOD_block]</code>
</td></tr></table>

a list of MOD blocks.