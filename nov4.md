# 11/4
- Strings are immutable like Python

### Primitive Wrappers
```java
Integer i = new Integer(1);
Integer max = Integer.max(i, 100);
max = Integer.parseInt(max.toString)); // converts max to string then parses it to an integer
```
- Done to perform methods on primitive types
- Autoboxing
```java
Character someChar = 'z';
char j = someChar;
System.out.println("Unboxed char " + j); // Will append j to "Unboxed char"
```
- `BigInteger` will never overflow

### Stacks
- Data structure: Hold data and provide operations on that data --> Object or class
- .push() and .pop() --> Popular operations
- LIFO (last-in, first-out)
- Only items on top can be removed
- Use for objects with LIFO behavior
- Ex: Reversing a string
- Set size before creating a stack
- Not recommended to have setters
- View classCode from nov4 for implementation

### Inheritence
- OOP allows classes to share certain behavior or data
- Every class can only have one superclass, many subclasses
- Syntax
```java
public class MountainBike extends Bicycle { 
	// Things!
	// MountainBike class "inherits" some methods and data from Bicycle
}
```
- Code reuse
- Allows "hierarchies" of inheritence
```java
public class CrossCountryMountainBike extends MountainBike {  
}
```
- `Bicycle` is subclass of Object
- `MountainBicycle` is subclass of Object (via Bicycle)
- Overriding
	- A class can override superclass methods and objects

### Processing
- Create graphical programs
