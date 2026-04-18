<h2>
<code>es.MultiBlock.Type</code> enum
</h2>

>[!CAUTION]
>when using `es.CreateMultiBlock()` , don't create blocks that goes outside <b><a>the list of default unlocked items</a></b>, because it's listed as <i>illegal</i> act of shoplifting or ADs prevention.

___

```lua
"Cube"
```

a paintable cube block.

___

```lua
"Edge"
```

a paintable edge block.

___

```lua
"Corner"
```

a paintable corner block.

___

```lua
"Inner"
```

a paintable inner block.

___

```lua
"GlassBlock"
```

a paintable glass block.

___

```lua
"WoodenBlock"
```

a wooden block.

this block could float on water, and be destroyed by potato gun projectile.

___

```lua
"MetalBlock"
```

a metal block.

___

```lua
"StoneBlock"
```

a stone block.

___

```lua
"GoldenBlock"
```

a golden block.

___

```lua
"GoldenEdge"
```

a golden edge block.

___

```lua
"GoldenCorner"
```

a golden corner block.

___

```lua
"GoldenInner"
```

a golden inner block.

___

```lua
"Barrel"
```

a barrel block.

this block could float on water.

___

```lua
"DriverSeat"
```

a driver seat block.

___

```lua
"PassengerSeat"
```

a passenger seat block.

___

```lua
"Suspension"
```

a spring coil block.

>[!CAUTION]
>this block shouldn't be created with `es.CreateMultiBlock()` , because it would become unbreakable.

___

```lua
"SuspensionSecondBase"
```

a decorative paintable coin block, being internally created by `Suspension` .

this block is also called "SSB coin" .

___

```lua
"Piston"
```

a piston block.

___

```lua
"PistonSecondBase"
```

a decorative paintable coin block, being internally created by `Piston` .

this block is also called "PSB coin" .

___

```lua
"Cannon"
```

a cannon block.

this block could destroy other blocks.

___

```lua
"Mortar"
```

a mortar block.

this block could destroy other blocks.

___

```lua
"PotatoGun"
```

a potato gun block.

this block could destroy 2 block ( `GlassBlock` and `WoodenBlock` ) , and trigger the `Switch` and `Button` .

___

```lua
"Camera"
```

a camera block.

___

```lua
"TV"
```

a TV block.

___

```lua
"Shield"
```

a block that could generate a big cyan virtual shield.

___

```lua
"SpeechBlock"
```

a block that could do TTS.

___

```lua
"VK1_A_Jet"
```

a jet thruster block.

this block is also called "A24 block"

___

```lua
"Beacon"
```

a police beacon block, always rotate clockwise.

this block is also called "CW block"

___

```lua
"StrobleLights"
```

a stroble lights block.

the body and all 6 lights could be painted independently.

___

```lua
"SciFiCab"
```

a decorative sci-fi cab block.

the glass and body could be painted independently.

___

```lua
"GlassCab1"
```

a decorative paintable glass cab block, looks like sunglasses.

___

```lua
"GlassCab2"
```

a decorative paintable glass cab block, looks like jet's cab.

___

```lua
"GlassCab3"
```

a decorative paintable glass cab block, looks like crane's cab.