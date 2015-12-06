# 12/2

## Interface
- Common languages between classes
- `implement` use an interface

```java
public class Dog extends Animal implements Pet
```
  - Concrete classes that implement an interface must implement ALL methods in order to compile
  - Can implement as many as you want
  - Must pass (or not pass) the proper params
- Interface and Inheritance
  - The lowest hierarchy (the concrete class) must implement all interface methods
- Abstract Classes vs. Interfaces
  - Abstract Classes - Hierarchy
    - Extends once
  - Interfaces - Common behaviors
    - `public static` only
    - No Constructors
    - Can implement multiple
    - Removes "Diamond Problem"
  - Choosing between the two
    - Always choose interface (usually)
    - "is-a" vs "can-behave-as"
  - Main difference
    - Interfaces DO NOT have hierarchies
- Advantage of Interfaces: Retrofitting
  - Classes can be retrofitted to implement a new interface
  - Interfaces can add methods to classes
    - Interfaces - Common behaviors
- Mixins
  - Interfaces ideal for defining "Mixin"
- Nonhierarchical Types
  - Interfaces can implement other interfaces using `extends`
- Advantage of Abstract Classes: Easier to evolve functionality
  - Adding a method to an interface will break ALL THE THINGS
  - Not with Java 8! It has a default method!
- Comparable Interface
  - Only has one method `compareTo()`
  - Return 1, 0, or -1
  - Can be used to use `java.util.Arrays.sort(yourArray);`
- `java.util.Arrays.sort(yourArray);`
  - yourArray's type must implement the `.compareTo()` method from Comparable Interface in order for `java.util.Arrays.sort(yourArray);` to work

```java
public class Thing implements Comparable<Thing> { // <Thing> is the type parameter
  /* Code here... */
}
```
  - Without `<Thing>`, you must do things more ~manually~
