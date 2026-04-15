<h2>
<code>es.GUI</code>
</h2>

<table><tr><td>
expands
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
virtual function description
</h2>

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
button visibility
</td></tr></table>

change button visibility.

this button is only shown if player look at the MOD block.

>[!TIP]
>to pin the button, add more scripts to move the MOD block itself to player's crosshair, and keep distance of 5 blocks.

___

```lua
es.setButtonText(value)
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
<code>String</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
description
</td><td>
|
</td><td>
button text.
</td></tr></table>

change button text.

>[!TIP]
>texts should be short, and meaningful.

>[!IMPORTANT]
>long texts is <i>technically</i> possible. however, it would make the text smaller, which would harm readability, especially plain one.

___

```lua
es.setButtonIcon(path)
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
default
</td><td>
|
</td><td>
built-in <code>fingerprint.png</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
description
</td><td>
|
</td><td>
image file path.
</td></tr></table>

change button icon.

>[!TIP]
>icons should have the dimension of 64x64px , have less details, and meaningful.