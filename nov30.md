# 11/30

## Final and immutability
- `Final`
  - Prevents classes from being subclassed
  - Prevents methods from being overriden
  - `final static` --> constant
    - UPPERCASE names
  - Reference is final, but data is not (except for primitives and possibly Strings(?))
```java
final Counter c = new Counter();
c = new Counter(4); // not allowed
c.increment(); // allowed
```
  - Blank finals must be assigned in Constructor
  - Building block for immutable class
- Immutability
  - Considered good technique
  - Making classes immutable (view slides)
  - Good for threading

## Abstract class
- `Animal` abstraction but `three-toed sloth` is concrete example of `Animal`
- Represents general concepts of objects
- `public abstract class Thing`
- Cannot be instantiated using `new`
- Can contain mix of concrete and abstract methods
- Abstract methods must be abstract classes
- To extend, must provide an implementation on abstract classes
- At the lowest hierarchy, must implement all abstract classes
- Abstract classes DO NOT need to implement all classes
- Can have a constructor in abstract class. Can call it using `super()`
- Abstract classes are used like normal class

## Interfaces
- Abstract class-like
- Abstract methods and data fields
- No constraint because no subclasses
- Great for modelling behaviors
- Any declaration in the interface is `abstract` by definition
