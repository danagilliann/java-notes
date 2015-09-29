# 9/28
## Scopes
- `{ }` and params `()` define one scope
- Scope can define a location in memory
- Variables can be reassigned in different scopes
```java
public static void methodA() { // one scope 
	int a = 1;
	public static void methodA1() { // nested scope 
		a = 2; // gets reassigned in methodA1
	}
}
```

## Functions
- `public static void thing1` expected to NOT return anything, calls a side-effect
- `public static short thing2` expected to return an short
- Can call a method before defining it 
- Storing functions within a variable
- Functions are objects so you can treat them like variables
```java
int y = calculateGrade(50, 50);
public static int calculateGrade(int x, int y) {  
	return x + (int) (Math.random() * y);
}
System.out.println(y) // prints an int
```
- Can simplify nesting returned functions
```java
x = max2(1,3,5);
System.out.println(x);
public static int max2(int a, int a, int c) { 
	return max(max(a,b),c); // max gets nested
}
```
- Boilerplate code should be converted into functions
