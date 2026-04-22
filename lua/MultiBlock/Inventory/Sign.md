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

represents a <code>Sign</code> block from the **Evertech Sandbox Lua API**.

this block stores and renders arbitrary text content inside the game world.

<h3>
🛡️ security notice
</h3>

the text renderer does **not perform validation or sanitization**, so developers must ensure content safety manually when reading or writing sign data.

loading sign data from untrusted sources may expose the runtime to:

- remote code execution,
- memory exhaustion (OOM) via oversized text buffers,
- excessive `<quad>` tag rendering,
- excessive unicode characters rendering.

**only load sign data from trusted save files or verified multiplayer environments**.

<h3>
☢️ runtime stability notice
</h3>

editing large sign contents directly in-game is not recommended.

observed risks include:

- interruption during editing caused by ADs,
- external apps switching triggered by ADs,
- application restart during long editing sessions.

**these interruptions may result in lost or corrupted sign data**.

<h3>
💡 recommended workflow
</h3>

for safer sign content editing:

- prepare text externally before inserting it into the block,
- paste content from clipboard instead of typing in-game,
- temporarily disable internet connectivity,
- test large sign datasets on devices with sufficient RAM (16 GB recommended),

when manipulating large or formatted sign content, prefer MOD environments.

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