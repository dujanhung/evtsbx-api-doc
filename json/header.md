<h2>
MOD_header
</h2>

represents **Evertech Sandbox MOD** header.

<table><thread><tr><td>

```json
"name|@required":"str"
```

MOD name.

</td></tr></thread><tbody><tr><td>

```json
"description|@required":"str"
```

MOD description.

</td></tr></tbody><thread><tr><td>

```json
"author|@required":"str"
```

MOD author name.

</td></tr></thread><tbody><tr><td>

```json
"version|@required":"str"
```

MOD version.

</td></tr></tbody><thread><tr><td>

```json
"preview|@required,filepath_flag(png)":"str"
```

MOD preview image filepath.

</td></tr></thread><tbody><tr><td>

```json
"simpleblocks|@required,list_flag(allow_multiple)":"list"
```

a list of MOD blocks.

</td></tr></tbody></table>