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
>"Evertech Sandbox" don't support multiple buttons, pinned button, set button transform and set button color.

>[!TIP]
>to interact with the "place" button, you should use another MOD block whose script use `es.TryGetMultiBlock()` , `es.MultiBlock.ModBlock.send()` and `es.MultiBlock.DestroyFast()` .

___

<h2>
function description
</h2>

```lua
es.enableButton(value)
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
"center button" visibility
</td></tr></table>

change "center button" visibility.

this button is only shown if player look at the MOD block.

>[!TIP]
>to pin the button, add more scripts to move the MOD block itself to in front of player's crosshair.

___

```lua
es.setButtonText(volume)
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
es.setButtonIcon(value)
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