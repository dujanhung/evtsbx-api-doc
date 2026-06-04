<h2>
MOD_header
</h2>

the "Evertech Sandbox" MOD header in JSON.

>[!IMPORTANT]
>"Evertech Sandbox" support `PNG` and `JPG` files. other files would fire an error.

___

```json
"name|@required,external_content(txt,inline)":"str"
```

MOD name.

___

```json
"description|@required,external_content(txt,multiline)":"str"
```

MOD description.

___

```json
"author|@required,external_content(txt,inline)":"str"
```

MOD author name.

___

```json
"version"
```

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