<h2>
MOD_block_connection
</h2>

represents a MOD block's connection point.

<table><thread><tr><td>

```json
"type|@required,enum(SignalReceiver,SignalSender,SignalReceiverSender)":"str"
```

connection point's type.

see this enum.

</td></tr></thread><tbody><tr><td>

```json
"color|@required,hex_flag(tag,no-alpha)":"str"
```

connection point's color.

</td></tr></tbody><thread><tr><td>

```json
"connectionsLimit|@required,range_flag(unsigned)":"int"
```

connection point's connection limit.

</td></tr></thread><tbody><tr><td>

```json
"relativePosition|@required":"dict"
```

connection point's relative position.

</td></tr></tbody></table>