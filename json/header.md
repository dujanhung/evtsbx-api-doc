<h2>
MOD_header
</h2>

```json
{
 "name|@required":"str",
 "description|@required":"str",
 "author|@required":"str",
 "version|@required":"str",
 "preview|@required,external_file(png)":"str",
 "simpleblocks|@required,list_flag(allow_multiple)":[
  "MOD_block"
 ]
}
```

the "Evertech Sandbox" MOD header in JSON.

>[!IMPORTANT]
>"Evertech Sandbox" support `PNG` and `JPG` files. other files would fire an error.

___

```json
"name|@required"
```

MOD name.

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

MOD description.

___

```json
"author"
```

<table><tr><td>
value type
</td><td>
|
</td><td>
<code>String</code>
</td></tr></table>

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