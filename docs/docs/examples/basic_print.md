## Basic Print

The OPCODE for this would be:

```
0000010000000011
0101010101010101
0000001001100111
0000010000000000
```

1. `0000010000000011` Sets the next line of code to the registry `0111` (code registry)\
   `0101010101010101`
2. `0000001001100111` Copies the code from registry 0111 to registry `0110` (print registry)
3. `0000010000000000` Prints the value at registry 0110.

> Output: `0101010101010101`
