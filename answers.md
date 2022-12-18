## What is the difference between var and let?

var is keyword used to declare a variable.
let is keyword used to declare a constant.

## What is an optional?

An optinal is a property of a variable/constant. Variables/constants must have a data type associated with it; additionally, it can further be declared as an optinal. The optional property of a variable/constant means that the value of the variable/constant can be either a nil or a value of the specified data type.

## What is optional chaining vs optional binding?


## What are the different ways to unwrap an optional? How do they work? Are they safe?

* Using if else block
* Forced unwrapping
* Optinal binding within if block
* Optional chaining
* Using nil-coalescing operator


## What is a closure?

A closure can be of one of three forms:
* Global function
* Nest function
* Nameless function

Typically, when we talk about closures, we are talking about the nameless function.

## What is the difference between a class and a struct?

The main difference between a class and a struct is that: a class is of reference type and a struct is of reference type.

## What is the syntax '??' do?

?? is the nil-coalescing operator. It is a binary operator. The syntax is given as:

a ?? b

where a is an optional type, and b is the same type as a, however is not required to be an optional. The ?? operator will unwrap the operand a if it is not nil, or return the operand b, if a is nil. 

Essentially, a ?? b is equivalent to, a != null ? a! : b

## What is a tuple?

A tuple is a type, and the syntax for it is a list of type(s) separated by commas, and the whole list surrounded by a pair of parentheses.

e.g: (Int, String, Float)

## What is Any vs AnyObject?

Any is a keyword that represents any type.
AnyObject is a keyword that represents an instance of any class type.

## What is a protocol?
