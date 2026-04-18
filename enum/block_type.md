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

this block could be destroyed by potato gun projectile.
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

>[!NOTE]
>due to block units in "Evertech Sandbox" don't have custom mass, this block's mass is equal to others.

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
"NoCollisionBlock"
```

a "no collision" block.

>[!CAUTION]
>this block is hard to access via MOD, because `es.TryGetMultiBlock()` can't see it. the only one way is to access the neighbor blocks and use `es.Root` .

___

```lua
"Wheel"
```

a regular wheel block, 3x1.

___

```lua
"WheelThin"
```

a paintable thin wheel block, 3x1.

___

```lua
"BRTWheel"
```

a paintable BRT wheel block, 3x1.

___

```lua
"BigWheel"
```

a big wheel block, 5x2.

___

```lua
"HugeWheel"
```

a huge wheel block, 7x3.

___

```lua
"MonsterWheel"
```

a monster wheel block, 7x4.

___

```lua
"SoccerBall"
```

a decorative soccer ball block.

___

```lua
"Barrel"
```

a decorative barrel block.

this block could float on water.

___

```lua
"Flank"
```

a decorative flank block.

this block could fit with `RailLines` , but can't cross the `RailCross` .

___

```lua
"BeamLines"
```

a decorative straight beam block.

___

```lua
"BeamArc"
```

a decorative arc beam block.

___

```lua
"WoodenBeamLines"
```

a decorative straight beam block.

this block could float on water.

___

```lua
"WoodenBeamArc"
```

a decorative arc beam block.

this block could float on water.

___

```lua
"Ladder"
```

a decorative ladder block.

player could climb on this block.

this block could cross the `RailCross` .

>[!CAUTION]
>don't destroy this block while player is climbing on it. otherwise, player would get stuck in mid-air.

___

```lua
"RailLines"
```

a straight rail block.

___

```lua
"RailCross"
```

a crossing rail block.

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
"MortarMarine"
```

a marine mortar block.

this block could destroy other blocks.

the projectile could float on water.

___

```lua
"PotatoGun"
```

a potato gun block.

this block could destroy 2 block ( `GlassBlock` and `WoodenBlock` ) , and trigger the `Switch` and `Button` .

player could hold this block as a handheld weapon.

>[!NOTE]
>in multiplayer, when edit mode is disabled, player <i>can't</i> use this item.

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
"OldTV"
```

an old TV block.

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

>[!TIP]
>this block should be used in the "2017's coin" event, to trap the coin.