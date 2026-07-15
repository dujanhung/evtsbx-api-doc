# Sign

stores and renders arbitrary text contents.

> [!WARNING]
> **this block must only be used for testing purposes**.
>
> use it at your own (risks)[https://github.com/dujanhung/evtsbx-api-doc/blob/main/lua/MultiBlock/Inventory/Sign/risks.md].

# <a id="minimap"/> minimap

╠╦ [constructor](#constructor)<br>
┃┗╾ [1](#constructor_1)<br>
╠╦ [property](#property)<br>
┃┣╾ [Text](#property_Text)<br>
┃┣╾ [Text Color](#property_TextColor)<br>
┃┗╾ [Background Color](#property_BackgroundColor)

# <a id="constructor"/> constructor

[⛖](#minimap)

## <a id="constructor_1"/> 1

```lua
es.MultiBlock.Sign
```

get instance.

- flag : `getter`
- type : `evertech_SIGNAPI`

[⛖](#minimap)

# <a id="property"/> property

[⛖](#minimap)

## <a id="property_Text"/> Text

```lua
es.MultiBlock.Sign.Text
```

`Sign` text.

- flag : `getter` , `setter`
- type : `string`

[⛖](#minimap)

## <a id="property_TextColor"/> Text Color

```lua
es.MultiBlock.Sign.TextColor
```

`Sign` text color.

use RGB linear color.

- flag : `getter` , `setter`
- type : `{float,float,float}`
- default : `{0.32,0.32,0.32}`

[⛖](#minimap)

## <a id="property_BackgroundColor"/> Background Color

```lua
es.MultiBlock.Sign.BackgroundColor
```

`Sign` background color.

use RGB linear color.

- flag : `getter` , `setter`
- type : `{float,float,float}`
- default : `{0.86,0.86,0.86}`

[⛖](#minimap)
