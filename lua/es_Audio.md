<h2>
<code>es.Audio</code>
</h2>

<table><tr><td>
expands
</td><td>
|
</td><td>
<code>es</code>
</td></tr></table>

a helper class to play audio files.

>[!IMPORTANT]
>"Evertech Sandbox" only support `WAV` file. other files would fire an error.

>[!TIP]
>if the file's source don't have `WAV` output, use file converter apps to convert them to `WAV` file.

>[!IMPORTANT]
>only one audio file could be played at the same block at the same time. trying to play the new one while the old one is still playing, would result in suddenly playing the new one instead.

>[!TIP]
>to play multiple audio files at a same time, you should create more blocks whose scripts are pointing to different audio files.

>[!WARNING]
>don't make the audio length too short. otherwise, lag would occur upon playing it.

___

<h2>
method description
</h2>

```lua
es.PlaySound(path)
/*

  -> void

  mandatory

  name  | path
  ------+-------------------
  type  | str
  ------+-------------------
  range | filepath_flag(wav)

*/
```

play a `WAV` file.

___

```lua
es.SetSoundVolume(volume)
/*

  -> void

  mandatory

  name  | volume
  ------+-------------------
  type  | float
  ------+-------------------
  range | range_flag(linear)

*/
```

change sound volume.

___

```lua
es.SetSoundLoop(value)
```

<table><tr><td>
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
default
</td><td>
|
</td><td>
<code>false</code>
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

change loop mode.