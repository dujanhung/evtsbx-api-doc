<h2>
<code>es.GUI</code>
</h2>

<table><tr><td>
inherit
</td><td>
|
</td><td>
<code>es</code>
</td></tr></table>

a helper class to interact with GUI.

>[!IMPORTANT]
>"Evertech Sandbox" support `PNG` and `JPG` files. other files would fire an error.

>[!TIP]
>if the file's source don't have such outputs, use file converter apps to convert them.

>[!IMPORTANT]
>only one button could be shown at the same block at the same time.

>[!TIP]
>to interact with multiple buttons, you should use another MOD block whose script use `es.TryGetMultiBlock()` and `es.MultiBlock.ModBlock.send()` , which is equivalent to using the "place" button.

___

<h2>
property description
</h2>

```lua
es.PlaySound(path)
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>protected</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
return type
</td><td>
|
</td><td>
<code>void</code>
</td></tr></table>

<table><tr><td>
mandatory
</td><td>
|
</td><td>
<code>path</code>
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
description
</td><td>
|
</td><td>
<code>WAV</code> filepath
</td></tr></table>

play a `WAV` file from `path` .

___

```lua
es.SetSoundVolume(volume)
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>protected</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
return type
</td><td>
|
</td><td>
<code>void</code>
</td></tr></table>

<table><tr><td>
mandatory
</td><td>
|
</td><td>
<code>volume</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
type
</td><td>
|
</td><td>
<code>float</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
description
</td><td>
|
</td><td>
sound volume.
</td></tr></table>

change sound volume at runtime.

___

```lua
es.SetSoundLoop(value)
```

<table><tr><td>
behavior
</td><td>
|
</td><td>
<code>protected</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
return type
</td><td>
|
</td><td>
<code>void</code>
</td></tr></table>

<table><tr><td>
mandatory
</td><td>
|
</td><td>
<code>value</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
type
</td><td>
|
</td><td>
<code>bool</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
description
</td><td>
|
</td><td>
loop mode
</td></tr></table>

change loop mode at runtime.