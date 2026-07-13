<h2>
<code>es.MultiBlock.Sign</code>
</h2>

stores and renders arbitrary text contents.

___

<h2>
constructor
</h2>

```lua
es.MultiBlock.Sign
```

get instance.

<table><tr><td>
behavior
</td><td>
<code>getter</code>
</td></tr><tr><td>
type
</td><td>
<code>evertech_SIGNAPI</code>
</td></tr></table>

___

<h2>
property description
</h2>

<codeblock lang="lua">
es.MultiBlock.Sign.Text
</codeblock>

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
>this variable is commonly used for MOD - player interface, and ASCII art generator.

>[!WARNING]
>at some updates until now, `Sign` text's font is changed, and the vertical spacing is increased. so, some ASCII arts would be broken, and renders incorrectly on the `Sign` .

>[!CAUTION]
>don't use `<quad>` , because it would breaks rendering, and cause lag.

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

>[!NOTE]
>in old versions, `Sign` text color could change alpha value. however, at some updates until now, it's removed to deal with `<quad>` bug.

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