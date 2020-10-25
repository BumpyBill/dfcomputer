## ALU

The syntax for the ALU OPCODE is:

```
00000001<# method #>
```

### OPCODE

If `method` is equal to `00000000`, it will set the value of registry `0011` to the sum of `0001` and `0010`
If `method` is equal to `00000001`, it will set the value of registry `0011` to the difference of `0001` and `0010`

### Registries

- 0011: Output
- 0001: ALU1
- 0010: ALU2
