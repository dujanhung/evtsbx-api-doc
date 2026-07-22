# block local transformations

changes block local transformations.

if a valid command is entered into `es.MultiBlock.Sign.Text` (directly or via API), the entered `Sign` block would:

- find a block under it
- change block local transformations

after the command is successfully done for once, the entered `Sign` block would cache target block's GUID internally, to continue working in next time.

# <a id="minimap"/> minimap

╠╦ [move](#move)<br>
┃┣╾ [x](#move_x)<br>
┃┣╾ [y](#move_y)<br>
┃┗╾ [z](#move_z)<br>
╠╦ [spin](#spin)<br>
┃┣╾ [x](#spin_x)<br>
┃┣╾ [y](#spin_y)<br>
┃┗╾ [z](#spin_z)

# <a id="move"/> move

```txt
move x y z
```

move block, relative to itself with `Sign` axises.

block's position unit is `0.5 per block`.

> [!WARNING]
> **this command could cause memory overflow**.
>
> if you see `Sign` texts with 20 digits, such as:
>
> ```txt
> move 12345678901234567890 12345678901234567890 12345678901234567890
> ```
>
> you must leave immedicately.

[⛖](#minimap)

## <a id="move_x"/> x

move block along `Sign` forward axis.

[⛖](#minimap)

## <a id="move_y"/> y

move block along `Sign` upward axis.

[⛖](#minimap)

## <a id="move_z"/> z

move block along `Sign` left axis.

[⛖](#minimap)

# <a id="spin"/> spin

```txt
spin x y z
```

spin block, relative to itself with `Sign` axises.

rotation unit is in degrees.

[⛖](#minimap)

## <a id="spin_x"/> x

spin block along `Sign` forward axis.

[⛖](#minimap)

## <a id="spin_y"/> y

spin block along `Sign` upward axis.

[⛖](#minimap)

## <a id="spin_z"/> z

spin block along `Sign` left axis.

[⛖](#minimap)
