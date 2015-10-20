# 10/19

### Object Oriented Principles

### What tf is Java????
- Language
- Libraries
- Compiler and Runtime (JVM)

### JVM
- Java Virtual Machine
- Runtime: Runs program once it is compiled
- Between program and OS --> Abstracts away complexity
- Memory mangement
```
.java --> compiler --> .class --> JVM --> Windows, Linux, or Mac
```

### JVM Memory Management
- Asks OS for memory
- If exceeds memory, then JVM gets more

### Types of Memory in JVM
- Static, stack, and heap
- Declaring variables: Java allocates space from memory regions
- Stack: Call to method
- Heap: `new` keyword

### Stack
- Kind of a data structure
- LIFO
- `Push` and `pop` --> `pop` remove, `push` add

### "Call Stack"
- Stack frame
	- Generated from calling a method
	- 1 stack frame allocated per method
	- Within stack frame, variables in stack frame 
	- When a method is finished, stack frame gets popped
	- When main gets popped, JVM knows program is D O N E
	- Wehn method exits, variables go away

### Heap
- Reference types
	- Two types of variables: Primitives and references
	- Reference types are classes
	- Cannot call primitives on heap
- `new` keyword indicates a thing is on the heap
```java
String referenceToObjOnHeap = new String("On the heap");
// reference on the stack			^^^ creates variable on heap
```

### Key Idea
- Variables don't contain object of type
- It's a reference to object on the Heap
- Similar to the idea of copying arrays

### Intro to OOP
- Large programs break up into become objects
- Programming method to help organize code
- Entities: Nouns
- Actions: Verbs
- Classes - "Nouns"
	- State - Variables
	- Methods - Verbs, does things
	- General idea
		- Has features and properties
		- Conceptual understanding
		- Does one thing to do it well
	- `new` new instance of a class
