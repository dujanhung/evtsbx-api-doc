<h2>
MOD_block
</h2>

```json
{
 "uuid":"random_uuid",
 "name":"new MOD block",
 "description":"sample text",
 "icon":"icon.png",
 "dif":"dif.png",
 "nor":"nor.png",
 "met":"met.png",
 "mesh":"mesh.obj",
 "script":"script.lua",
 "collider":"sizable_wheel",
 "normScale":1,
 "smoothness":0.5,
 "scale":1,
 "colliderOptions":{
  "MOD_collider_option"
 },
 "meshOption":{
  "MOD_mesh_option"
 },
 "connections":[
  "MOD_connection"
 ]
}
```

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

>[!IMPORTANT]
>this value must be unique among others from inside the `info.json` and other MOD.

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
