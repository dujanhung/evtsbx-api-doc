<h2>
<code>es.Time</code>
</h2>

<table><tr><td>
expands
</td><td>
|
</td><td>
<code>es</code>
</td></tr></table>

a helper class to get app's engine time informations.

___

<h2>
property description
</h2>

```lua
es.TimeScale
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
<code>float</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
default
</td><td>
|
</td><td>
<code>1.0</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
range
</td><td>
|
</td><td>
more than <code>0.0</code>
</td></tr></table>

change time scale.

>[!CAUTION]
>don't increase this thing more than `8.0` . otherwise, lag would occur.

>[!IMPORTANT]
>time scale could be reset via pause menu, and upon world file reload.

___

```lua
es.DeltaTime
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
<code>float</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
range
</td><td>
|
</td><td>
more than <code>0.0</code>
</td></tr></table>

the interval of screen rendering frames.

___

```lua
es.FixedDeltaTime
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
<code>float</code>
</td></tr><tr><td>
</td><td>
</td><td>
</td></tr><tr><td>
range
</td><td>
|
</td><td>
more than <code>0.0</code>
</td></tr></table>

the interval of physics rendering frames. usually about <code>0.02</code> .