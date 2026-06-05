# <code>es.Audio</code>

a helper class to play audio files.

> [!IMPORTANT]
> "Evertech Sandbox" only support `WAV` file. other files would fire an error.

> [!TIP]
> if the file's source don't have `WAV` output, use file converter apps to convert them to `WAV` file.

> [!IMPORTANT]
> only one audio file could be played at the same block at the same time. trying to play the new one while the old one is still playing, would result in suddenly playing the new one instead.

> [!TIP]
> to play multiple audio files at a same time, you should create more blocks whose scripts are pointing to different audio files.

> [!WARNING]
> don't make the audio length too short. otherwise, lag would occur upon playing it.

___

# method description

<table><thread><tr><td>

```lua
es.PlaySound(path)
```

```lua
-> nil
```

<table><thread><tr><td>
name
</td><td>
<code>
path
</code>
</td></tr></thread><tbody><tr><td>
type
</td><td>
<code>
str
</code>
</td></tr></tbody><thread><tr><td>
range
</td><td>
<code>
filepath_flag(wav)
</code>
</td></tr></thread></table>

play a `WAV` file.

</td></tr></thread><tbody><tr><td>

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

</td></tr></tbody><thread><tr><td>

```lua
es.SetSoundLoop(v)
/*

  -> str

  mandatory

  name  | v
  ------+-----
  type  | bool

*/
```

change loop mode.

</td></tr></thread></table>