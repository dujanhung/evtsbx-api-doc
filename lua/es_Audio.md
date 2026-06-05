# <code>es.Audio</code>

a helper class to play audio files.

> [!TIP]
> if the file's source don't have `WAV` output, use file converter apps to convert them to `WAV` file.

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
return nil
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
```

```lua
return nil
```

<table><thread><tr><td>
name
</td><td>
<code>
volume
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
range_flag(linear)
</code>
</td></tr></thread></table>

change sound volume.

</td></tr></tbody><thread><tr><td>

```lua
es.SetSoundLoop(v)
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
bool
</code>
</td></tr></tbody></table>

change loop mode.

</td></tr></thread></table>