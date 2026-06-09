# evtsbx-api-doc

a full **Evertech Sandbox API documentation** in MD files.

<table><tr><td>

<img src="https://github.com/dujanhung/evtsbx-gallery/blob/main/meme/famous.jpg"/>

<sup>
how users see MOD authors in multiplayer
</sup>

</td></tr></table>

___

# features

## fancy `<table>` tags

improve readability.

## functionable

works in **Evertech Sandbox** out-of-the-box.

___

# example doc entry

## JSON

### enum description

<table><tr><td>

```json
"a"
```

JSON enum description

</td></tr></table>

### entry description

<table><tr><td>

```json
"name|flag1,flag2,...":"variant"
```

JSON entry description

</td></tr></table>

## Lua

### inheritance

<table><thread><tr><td>
inherit
</td><td>
<code>parent1</code>
</td></tr></thread><tbody><tr><td>
inherited by
</td><td>
<code>child1</code>
</td></tr></tbody></table>

### minimap

<table><thread><tr><td>
name
</td><td>
variant type
</td><td>
flag
</td></tr></thread><tbody><tr><td>
<code>
property1
</code>
</td><td>
<code>
number
</code>
</td><td>
<code>
getter
</code>
<br>
<code>
setter
</code>
</td></tr></tbody><thread><tr><td>
<code>
method1()
</code>
</td><td>
<code>
nil
</code>
</td><td>
<code>
virtual
</code>
<br>
<code>
required
</code>
</td></tr></thread></table>

### property description

<table><tr><td>

```json
"property1":{
 "type":"number",
 "flag":"getter,setter"
}
```

```lua
property1
```

Lua property description.

</td></tr></table>

### method description

<table><tr><td>

```json
"method1":{
 "type":"nil",
 "mandatory":[
  {
   "v":{
    "type":"number",
    "range":"0<=x<=1"
   }
  }
 ]
}
```

```lua
method1(v)
```

Lua method description.

</td></tr></table>

___

# usage

___

# credits

<table><thread><tr><td>
resource
</td><td>
description
</td></tr></thread><tbody><tr><td>
<a href="https://vitsum.com/evertech/docs/#/en-US/">
Evertech Sandbox API doc
</a>
</td><td>
depends on official API documentation
</td></tr></tbody></table>