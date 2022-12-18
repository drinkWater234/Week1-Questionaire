## What is the difference between var and let?

var is keyword used to declare a variable.  
let is keyword used to declare a constant.

## What is an optional?

An optinal is a property of a variable/constant. Variables/constants must have a data type associated with it; additionally, it can further be declared as an optinal. The optional property of a variable/constant means that the value of the variable/constant can be either a nil or a value of the specified data type.

## What is optional chaining vs optional binding?

Optional chaining is a way to query properties, method on an optional that may be nil. If the optional is non-nil, the property or method query return thevalue, if the optional is nil, the property or method return a nil. By chaining multiple queries together, we can handle any fails if any of the link in the chain results in a nil. Optional chaining can be done by placing the question mark after the optional value on a property or method. The type of the return value from optional chaining is always an optional value. 

## What are the different ways to unwrap an optional? How do they work? Are they safe?

### Force unwrapping
For example:  
```
var x: Int? = 5
print("\(x!)")
```
In the code above, the exlamation point at the end of the optional's name is used to force unwrap the optional. Generally using forced unwrapping is unsafe if you do not know whether the optional contains a value or a nil. It is important to note that if you force unwrap optional that contains nil, the code will trigger a runtime error.

### Optinal binding
For example:  
```
var x: Int? = 5
if let y = x
{
	print("The value of x is: \(y)")	
}
```
In the code above optional binding is used to unwrap the optional variable x. Optional binding is a safe way to unwrap an optional because it checks whether the optional contains a value or nil.

### Optional chaining
Optionals may be unwrapped with optional chaining. See the section *What is optional chaining vs optional binding?* section for the explanation on how it works. Optional chaining is a safe way to unwrap an optional because it checks whether or not the optional is nil.


### nil-coalescing operator
For example:  
```
var x: String? = "Hello World"
print("\(x ?? "Water")")
```
The nil-coalescing operator is a binary operator in the form of: A ?? B. Where A is an optional type, and B is a the same type of A (which does not need to be an optional). The nil-coalescing operator unwraps the optional A it if contians a value, else, it returns the value B. It is important to note that, if A is non-nill, the B is not evaluated. Essentially, the expression A ?? B is equivalent to: a != nil ? a! : b. With that said, using nil-coalescing operator to unwrap an optional is safe because it checks wether or not the optional is a nil.


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
