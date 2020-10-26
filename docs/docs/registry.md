## Registry

The syntax for the registry OPCODE is:

```
00000010<# reg1 #><# reg2 #>
```

If `reg1` is equal to `0000`, this works as a jump command.

```
0000010000000011
0000000000000000
0000001000000111
```

This sets the current line to 0, so afer executing the jump command, the computer will start reading from the first line.
