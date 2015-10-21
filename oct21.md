# 10/21
- Strings are immutable
- Lists contain stuff in memory
- These affect how you can change them with methods

## Purpose a class
- Can create own
- Create own reference and data types
- State represented by data fields (properties)
- Behavior defined by methods (function)
- Constructor: Method used to create an object from a class --> `new` keyword
```java
public class aCoolClass {
	public aCoolClass() { // This thing is constructor. It has no return type and has the same name as the class 
		someDate = 5;
	}
}
```
- Think of constructors as an entrypoint to the class and the way to create instances of class
```java
Scanner s = new Scanner();
//							^^^^^^^^^ Constructor!!
```
- Can create class files to be accessed by other class files
```java
public Box(int l, int w) {
  this(l, w, 1); 
	/* 
	* this() calls the above three-arg constructor. 
	* this(), in this case (lol), create an instance of the cube.
	* Knows that this == Cube method because of the type and number of parameters
	*/
}
```
- If two classes are being used in the same package, you do not need to import the class

## Fun things
- Change multiple words at the same time: Refactor > Rename 
