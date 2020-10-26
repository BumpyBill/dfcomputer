## Alu Commands

### What is the Alu?

The ALU (Arithmetic and Logic Unit) is the part of the computer that does math. It has three registers: `0001`, `0010`, and `0011`. `0001` is the first input (sometimes called ALU1), `0010` is the second input (likewise called ALU2), and `0011` is the output (ALUOut). To carry out an operation, the registers `0001` and `0010` must be set to the operands of the operation to be performed, and then an ALU operation must be called, which will set `0011` to the result.


### How to use the Alu

Most of the inner workings of the ALU are taken care of by the three argument commands `add([<# reg1 #>],[<# reg2 #>],[<# reg3 #>])` and `sub([<# reg1 #>],[<# reg2 #>],[<# reg3 #>])`. These will take the value in `reg1` and `reg2`, perform the operation, and store the result in `reg3`. If `reg3` is left out resulting in a two argument command, the output will sit in ALUOut (`0011`).

If you want to make an efficient program (more speed and fewer binary code lines), you may want to access the ALU functions independently. `addRaw` and `subRaw` will simply perform their respective operation on `0001` and `0010` and store it in `0011`. The ALU registers can be accessed with `setReg()`. A shorthand for storing ALU operands is `prepAlu([<# reg1 #>],[<# reg2 #>])`. This sets ALU1 to reg1 and ALU2 to reg2. However, some commands (like `if!()`) use ALU functions within them, so letting the values sit in the ALU registers while other code is running isn't always an option.
