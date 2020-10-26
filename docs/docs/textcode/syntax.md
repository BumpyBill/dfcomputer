## Text Code Syntax

### Commands

Every command gets its own line. Commands with no arguments are just the name of the command alone on a line. Commands with arguments have parentheses after the command name that contain all arguments separated by commas. Do not use spaces. If a line starts with something that is not a command name, it will be considered a comment. Here are some examples:
```
setReg([0001],{3})
setReg([0010],{5})
This is a comment!
addRaw
print([0011])
end
```


### Argument Types

Arguments must be expressed with delimiters denoting the type of argument they are. Registers must use [] (`[0001]`), binary numbers must use <> (`<1001010010011011>`), and integers must use {} ('{4}').
