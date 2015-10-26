# 10/26

## Default values 

```java
public class Rectangle {
	int width;
	int length;
	
	String foo; // Default for reference type is null

	// Contructor
	public Rectangle() {
		/* 
		* Both will print 0 because those are the intialized values
		*/
		System.out.println(width);
		System.out.println(length;
		
		System.out.println(foo) // Prints null because that's a reference type's default value
	}
}
```

```java
private String foo;
// Both are equal to each other
private String bar = null;

System.out.println(s1.equals(s2)); // null pointer exception error
System.out.println(s1 == s2); // prints tru
```

## This()
- `this(foo, bar)` looks for the constructor that takes in the type and number of parameter. In this case, it's `foo` and `bar`

```java
public class Rectangle {
	private int width;
	private int length;

	// Contructor
	public Rectangle() { 
		this(5, 5);
	}

	public Rectangle(int w, int l) {
		width = w;
		// width must equal w and length must equal l otherwise you'll interfere with private int width and private int length
		length = l;
		/*
	}

	// or
	public Rectangle(int width, int length) {
		this.width = width;
		this.length = length;
	}

}
```

## Static
- Variable is not associated with instance of class
- Not associated with an object of a class
- To use a static object or method, you DO NOT have to create an instance of an object
- Static methods can only reference static objects
- BUT instance methods can reference both static objects and instance objects

```java
// instance variable
private int i = 0;
// static variable
private static int j = 0; 

public static void someStaticMethod() {
  System.out.println(j);    // OK
  // System.out.println(i); // Does not compile
  // someInstanceMethod();  // Does not compile
}

// But instance methods can reference static methods and members
public void someInstanceMethod() {
  System.out.println(j); // OK
  System.out.println(i); // OK
  someStaticMethod();    // OK
}
```

## Access Modifiers
- One access modifier at a time
- `public`: Any other class can see this variable/method
	- Constructors should be public, in general (certain exceptions may apply)
- `private`: Only members of the class can see this variable/method
- `protected`
	- Only the subclasses can see this variable/method
	- Only children of parents can see this
- `packageMethod`
	- Only things inside the same directory can see
	- Default for Java
```java
public int foo() { 
	return 1;
}
// vs. package
int foo() { 
	return 1;
}
```

## Getters and Setters
- `public` methods can modify `private` objects
- Protect data by wrapping `public` methods around `private` objects (think of it like clothes on private areas)
