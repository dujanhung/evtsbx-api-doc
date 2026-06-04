<h2>
MOD_header
</h2>

the "Evertech Sandbox" MOD header in JSON.

>[!IMPORTANT]
>"Evertech Sandbox" support `PNG` and `JPG` files. other files would fire an error.

___

```json
"name|@required,external_content(inline_txt)":"str"
```

MOD name.

___

```json
"description|@required,external_content(multiline_txt)":"str"
```

MOD description.

___

```json
"author|@required,external_content(inline_txt)":"str"
```

MOD author name.

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