<h2>
MOD_block_connection
</h2>

represents MOD block's connection point.

___

```json
"type|@required,enum(SignalReceiver,SignalSender,SignalReceiverSender)":"str"
```

connection point's type.

see this enum.

___

```json
"color|@required,hex_flag(tag,no-alpha)":"str"
```

connection point's color.

___

```json
"connectionsLimit|@required,range_flag(unsigned)":"int"
```

connection point's connection limit.

___

```json
"relativePosition|@required":"dict"
```

connection point's relative position.