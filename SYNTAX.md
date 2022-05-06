# Laturon syntax manual
Here is an explanation of what the syntax within the Laturon programming language is, and how it can be used, to construct your very own Laturon projects.

## Arithmetic operators
|Operator|Action|
|-|-|
|+|Addition|
|-|Subtraction|
|*|Multiplication|
|/|Division|
|%|Modulos|

## Relational and logical operators
|Operation|Action|
|-|-|
|>|Greater than|
|>=|Greater than or equal to|
|<|Less than|
|<=|Less than or equal to|
|==|Equal to|
|!=|Not equal to|
|&&|And|
|\|\||Or|
|!|Not|

## Statements
|Statement|Action|
|-|-|
|if|Content within scope is run if an equation equates to true|
|else|Content within scope is only run when preceding if equates to false|
|while|Content within scope will repeatedly run if equation equates to true|

## Functions
|Function|Action|
|-|-|
|print|Outputs value|
|input|Returns a string from user input|
|str|Converts value to string|
|int|Converts value to integer|
|float|Converts value to float|
|bool|Converts value to bool|
|len|Returns length of string|
|type|Returns the type of variable|

### Function definitions
To declare a function the `function` keyword must come before the name of the function, and after the name of the function all parameters (if any) must be situated within a `(` and a `)`. An example function definition is as follows:
```
function example(parameter) {
	print(parameter)
}
```
This example function accepts a single parameter, which will be outputted to the user.

### Function calls
To call a function you must state the name of the function followed by the parameters passed to the function within a `(` and a `)`. An example call of the function created within [Function definitions](#function-definitions), is as follows:
```
example("Hello, World!")
```

### Returning a value from a function
Functions can also be used to return values, if a value from a function is stored, but nothing is returned from the function, a `null` value is given by default. However to explicitly return a value from a function, the `return` keyword will allow for this. The `return` keyword will only return a value when executed from within a scope, otherwise an error will be thrown. An example of a value being returned, is a follows:
```
return 123.456
```

## Scopes
Scopes are contents that are situated between a `{` and a `}`, all variables that are declared within a scope are automatically removed once the execution of the scope has ended. Scopes can be nested within another scope. An example of a scope is shown in an `if` statement below:
```
if (true) {
   print("This will be outputted")
}
```

---

This syntax guide was written for Laturon 0.3 on May 6th 2022.