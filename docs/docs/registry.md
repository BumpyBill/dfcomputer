## Registry

The syntax for the setReg OPCODE is:
```
00000010<# reg1 #><# reg2 #>
```
This sets the value of `reg1` to the value of `reg2`. 
For example, `0000001010001111` will set the the register `1000` to the value of `1111`.


The register `0111` is the code var. It is set with the command `0000010000000011`. That commmand will not read the following line of code as a command; it will instead set the register `0111` to the value of the line.
```
0000010000000011
1010101010101010
```
This sets the value of `0111` to `1010101010101010`. To set the value of a register other than `0111`, use the setReg command described above and use `0111` as `reg2`.


If `reg1` in the setReg command is equal to `0000`, this works as a jump command.
```
0000010000000011
0000000000000000
0000001000000111
```
This sets the current line to 0, so afer executing the jump command, the computer will start reading from the first line.
