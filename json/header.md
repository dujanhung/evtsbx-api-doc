<h2>
MOD_header
</h2>

```json
{
 "name":"new MOD"
 "description":"sample text"
 "author":"user"
 "version":"1.0"
 "preview":"image.png"
 "simpleblocks":[
  "MOD_block"
 ]
}
```

the "Evertech Sandbox" MOD header in JSON.

>[!IMPORTANT]
>"Evertech Sandbox" support `PNG` and `JPG` files. other files would fire an error.

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