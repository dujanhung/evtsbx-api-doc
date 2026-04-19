<h2>
<code>es.MultiBlock.Sign</code>
</h2>

<table><tr><td>
inherit
</td><td>
|
</td><td>
<code>es.MultiBlock</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
<code>es.MultiBlock.Type</code> specific
</td><td>
|
</td><td>
<code>Sign</code>
</td></tr></table>

a `Sign` block.

___

<h2>
constructor
</h2>

```lua
es.MultiBlock.Sign
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>getter</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
type
</td><td>
|
</td><td>
<code>SIGNAPI</code>
</td></tr></table>

get `Sign` instance.

___

<h2>
property description
</h2>

```lua
es.MultiBlock.Sign.Text
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>getter</code>
<br>
<code>setter</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
type
</td><td>
|
</td><td>
<code>String</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
default
</td><td>
|
</td><td>
<code>" "</code>
</td></tr></table>

`Sign` text.

>[!TIP]
>this one is used for MOD text input, and MOD screen.

>[!NOTE]
>at some updates until now, `Sign` text's font is changed, and the vertical spacing is increased. so, some ASCII arts would be broken, and displays incorrectly on the `Sign` .

___

```lua
es.MultiBlock.Sign.TextColor
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>getter</code>
<br>
<code>setter</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
type
</td><td>
|
</td><td>
<code>{float,float,float}</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
default
</td><td>
|
</td><td>
<code>{0.32,0.32,0.32}</code>
</td></tr></table>

`Sign` text color, use RGB linear color.

___

```lua
es.MultiBlock.Sign.BackgroundColor
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>getter</code>
<br>
<code>setter</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
type
</td><td>
|
</td><td>
<code>{float,float,float}</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
default
</td><td>
|
</td><td>
<code>{0.86,0.86,0.86}</code>
</td></tr></table>

`Sign` background color, use RGB linear color.