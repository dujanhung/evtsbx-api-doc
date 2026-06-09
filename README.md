# evtsbx-api-doc

a full **Evertech Sandbox API** documentation in MD files.

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
<br>
<code>child2</code>
<br>
<code>child3</code>
</td></tr></tbody></table>

### minimap

```lua
variant property1 getter setter
variant method1() virtual required
```

### property description

<table><tr><td>

```lua
property1
```

```lua
return variant
```

<code>getter</code><code>setter</code>

Lua property description.

</td></tr></table>

### method description

<table><tr><td>

```lua
method1(v)
```

```lua
return nil
```

<table><thread><tr><td>
name
</td><td>
<code>
v
</code>
</td></tr></thread><tbody><tr><td>
type
</td><td>
<code>
float
</code>
</td></tr></tbody><thread><tr><td>
range
</td><td>
<code>
0<=x<=1
</code>
</td></tr></thread></table>

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