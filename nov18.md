# 11/18

## Packages
-	Like folders on file system
- declaration `package edu.nyu.cs101`
- End up with default, unnamed package
- Cannot import class from default package. Avoid using default unless for small programs
- `import edu.nyu.cs101.SomeClass;` --> Importing one class from package
- `import edu.nyu.cs101.*;` --> Importing all classes
- Can use "fully qualified names" ex: `edu.nyu.SomeClass s = new edu.nyu.SomeClass();`

## Polymorphism
- Allows variables to be treated as a supertype

```java
// Here, we're assuming Bird is the superclass of Duck 
Bird a = new Bird();
Bird b = new Duck();
// ^^^ static type
//       ^^^^^^^^^^^ dynamic type
// THIS IS LEGAL!!!
```

- Only call methods on static type (view `Bird.java`, `Duck.java`, `TestBird01.java` on `line 27`)

## Dynamic Binding (Dynamic Dispatch)
- If dynamic type is different from static, and overriden method on dynamic type, that's the method that gets called
- Cannot call methods of a static type of a dynamic type

## Casting
```java
Animal a = new Cat();
( (Cat) a ).meow(); 
```
- If `Animal` does not have `.meow()`, but `Cat` does, then you can cast
- To safetly do this, use `instanceof()` operator to check
-	NOT RECOMMENDED because not thinking of Polymorphism and also it's hard to maintain

## Alternative to Casting
```java
public static void withPolymorphism() {
  Animal a = randomAnimal();
  a.talk();
}

public static Animal randomAnimal() {
  int r = (int) (Math.random() * 2);
  if (r % 2 == 0) {
    return new Cat(); // return the subclass of Animal
  } else {
    return new Dog();
  }
}
```

## ArrayList
- Don't have to give a size, but inefficient

```java
import java.util.ArrayList;
ArrayList<SomeType> = new ArrayList<SomeType>(); // SomeType can be String, int, etc
```
