## setReg

The setReg command can be used in three ways.


Firstly, it can be used to set one register to the value of another.
```
setReg([<# reg1 #>],[<# reg2 #>])
```
The value of `reg1` will be set to the value of `reg2`.


Secondly, setReg can be used to set a register to a binary value.
```
setReg([<# reg #>],<# binary #>)
```
`reg` will be set to the binary number.


Thirdly, setReg can set a register to an integer. This will be translated to binary when compiled, so it's simply for convenience of the programmer.
```
setReg([<# reg #>],{# integer #})
```
`reg` will be set to the binary translation of `integer`.
