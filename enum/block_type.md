<h2>
<code>es.MultiBlock.Type</code> enum
</h2>

a full list of block types from "Evertech Sandbox" in Lua.

>[!NOTE]
>unless otherwise noted, the word "paintable" means `es.MultiBlock.Paint()` would works.

>[!CAUTION]
>when using `es.CreateMultiBlock()` , don't create blocks that goes outside <b><a>the list of default unlocked items</a></b>, because it's listed as <i>illegal</i> acts of shoplifting or ADs prevention.

___

```lua
"SimpleModBlock"
```

a regular MOD block.

___

```lua
"WheelModBlock"
```

a wheel MOD block, 3x1.

___

```lua
"SizableWheelModBlock"
```

a sizable wheel MOD block, default size 3x1.

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. you should edit it manually in `info.JSON` .

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
"PipeLine"
```

a straight pipe.

___

```lua
"PipeBend"
```

a bend pipe.

___

```lua
"PipeArc"
```

an arc pipe.

___

```lua
"PipeTee"
```

a tee pipe.

___

```lua
"PipeFour"
```

a four-ways pipe.

___

```lua
"PipeSix"
```

a six-ways pipe.

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

>[!IMPORTANT]
>this block can't be painted with `es.MultiBlock.Paint()` . only player could paint it.

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

a paintable huge wheel block, 7x3.

___

```lua
"MonsterWheel"
```

a paintable monster wheel block, 7x4.

>[!IMPORTANT]
>this block can't be painted with `es.MultiBlock.Paint()` . only player could paint it.

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
"RubberDuck"
```

a decorative yellow rubber duck.

this block could float on water.

___

```lua
"GreenRubberDuck"
```

a decorative green rubber duck.

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

a paintable driver's seat block.

>[!IMPORTANT]
>this block can't be interacted with MOD, because there are no API entry about it. only player could interact with it.

___

```lua
"PassengerSeat"
```

a paintable passenger's seat block.

>[!IMPORTANT]
>this block can't be interacted with MOD, because there are no API entry about it. only player could interact with it.

___

```lua
"Suspension"
```

a paintable spring coil block.

>[!CAUTION]
>this block shouldn't be created with `es.CreateMultiBlock()` , because it would become unbreakable.

>[!CAUTION]
>in old versions, don't detach the group of 3 of this block at a same time, because it would cause crash.

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. only player could edit it.

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

a paintable piston block.

the body, and rod could be painted independently.

>[!IMPORTANT]
>the rod can't be painted with `es.MultiBlock.Paint()` . only player could paint it.

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. only player could edit it.

___

```lua
"PistonSecondBase"
```

a decorative paintable coin block, being internally created by `Piston` .

this block is also called "PSB coin" .

___

```lua
"Bearing"
```

a paintable bearing block.

>[!IMPORTANT]
>this block can't be created with `es.CreateMultiBlock()` . only player could create it.

>[!IMPORTANT]
>this block can't be painted with `es.MultiBlock.Paint()` . only player could paint it.

>[!IMPORTANT]
>this block can't be reversed with MOD, because there are no API entry about it. only player could reverse it.

___

```lua
"Thruster"
```

a paintable thruster block, size 2x2 height 3.

>[!IMPORTANT]
>this block can't be painted with `es.MultiBlock.Paint()` . only player could paint it.

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. only player could edit it.

___

```lua
"Engine"
```

a paintable engine block, size 2x2 height 2.

this block could spin the bearing.

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. only player could edit it.

___

```lua
"Controller"
```

a bearing controller block, size 1x2 height 1.

this block could set up bearing rotation sequences, change speed, and use loop mode.

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. only player could edit it.

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

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. only player could edit it.

___

```lua
"MortarMarine"
```

a marine mortar block.

this block could destroy other blocks.

the projectile could float on water.

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. only player could edit it.

___

```lua
"PotatoGun"
```

a potato gun block.

this block could destroy 2 block ( `GlassBlock` and `WoodenBlock` ) , and trigger the `Switch` and `Button` .

player could hold this block as a handheld weapon.

>[!NOTE]
>in multiplayer, when edit mode is disabled, player <i>can't</i> use this item.

>[!CAUTION]
>don't spam too many "potato" projectiles. otherwise, connection points would stop working.

___

```lua
"HeadLight"
```

a paintable headlight block.

___

```lua
"LightFrame"
```

a paintable double light block.

only the light beam is paintable, not the body.

>[!IMPORTANT]
>the light beam can't be painted with `es.MultiBlock.Paint()` . only player could paint it.

___

```lua
"Sign"
```

a sign block (size 1x3 height 1), could read, write and store texts.

>[!CAUTION]
>don't use `<quad>` , because it would cause lag.

___

```lua
"Switch"
```

a paintable switch block.

___

```lua
"Button"
```

a paintable button block.

>[!IMPORTANT]
>this block can't be interacted with MOD, because there are no API entry about it. player or `PotatoGun` projectile could interact with it.

___

```lua
"Timer"
```

a timer block.

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. only player could edit it.

___

```lua
"AND"
```

an AND gate.

___

```lua
"OR"
```

an OR gate.

___

```lua
"XOR"
```

a XOR gate.

___

```lua
"NAND"
```

a NAND gate.

___

```lua
"NOR"
```

a NOR gate.

___

```lua
"NXOR"
```

a NXOR gate.

___

```lua
"XORFeedback"
```

a XOR gate with feedback.

___

```lua
"Camera"
```

a camera block.

>[!CAUTION]
>in old versions, don't create too many of this blocks, because it would cause lag.

___

```lua
"TV"
```

a TV block.

___

```lua
"OldTV"
```

an old TV block, size 2x2 height 2.

___

```lua
"Shield"
```

a paintable block (size 4x4 height 1) that could generate a big cyan virtual shield.

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. only player could edit it.

___

```lua
"SpeechBlock"
```

a paintable block that could do TTS.

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. only player could edit it.

___

```lua
"VK1_A_Jet"
```

a paintable jet thruster block, size 1x3 height 2.

this block is also called "A24 block"

>[!IMPORTANT]
>this block can't be edited with MOD, because there are no API entry about it. only player could edit it.

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

a paintable 6-lights stroble lights block, size 1x6 height 1.

the body and all 6 lights could be painted independently.

>[!IMPORTANT]
>the light can't be painted with `es.MultiBlock.Paint()` . only player could paint it.

___

```lua
"SciFiCab"
```

a decorative paintable sci-fi cab block.

the glass and body could be painted independently.

>[!IMPORTANT]
>the glass can't be painted with `es.MultiBlock.Paint()` . only player could paint it.

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

___

```lua
"Toilet"
```

a toilet block, could open and close.

>[!IMPORTANT]
>this block can't be interacted with MOD, because there are no API entry about it. only player could interact with it.

___

```lua
"Tile"
```

a small decorative paintable square tile block.

>[!IMPORTANT]
>this block can't be created with `es.CreateMultiBlock()` . only player could create it.

>[!IMPORTANT]
>this block can't be painted with `es.MultiBlock.Paint()` . only player could paint it.

___

```lua
"CubeTile"
```

a small decorative paintable cube tile block.

>[!IMPORTANT]
>this block can't be created with `es.CreateMultiBlock()` . only player could create it.

>[!IMPORTANT]
>this block can't be painted with `es.MultiBlock.Paint()` . only player could paint it.

___

```lua
"TriangleTile"
```

a small decorative paintable triangle tile block.

>[!IMPORTANT]
>this block can't be created with `es.CreateMultiBlock()` . only player could create it.

>[!IMPORTANT]
>this block can't be painted with `es.MultiBlock.Paint()` . only player could paint it.

___

```lua
"Antenna"
```

a small decorative paintable antenna block, could react to movement.

>[!IMPORTANT]
>this block can't be created with `es.CreateMultiBlock()` . only player could create it.

>[!IMPORTANT]
>this block can't be painted with `es.MultiBlock.Paint()` . only player could paint it.