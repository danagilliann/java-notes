## 9/9
# Java Variables 

Java assigning variables:

```
type variableName = value;
```

Assigning variables:

``` 
int myInt = 0;		// initilization --> Both an declaration and assignment
int myOtherInt;		// declaration --> Get the default value
myOtherInt = 0;		// assignment
```

Types of Variables:

```
byte, short, int, long, float, double, boolean, char
// Just use doubles
// 32-bit: float --> Bc who uses 32-bit...lol Microsoft.
// 64-bit: double
```

Sting is a reference type, not primative type. It's a class.

Making variables a constant
```
final int MYINT = 100;		// Constants are UPPERCASE
```

Dynamic Typing
Static Typing
Strong Typing
Weak Typing

# User Input

To take input:

``` 
double b;
Scanner in = new Scanner(System.in);		// Must declare Scanner before the program
System.out.println("b = ");
b = in.nextDouble();		// Specifies the type you're reading. Must follow the declared variable.
in.close();		// Good practice. Follow Nike, JUST DO IT.
```

`in` can be anything

```
Scanner foo = new Scanner(System.in);
b = foo.nextDouble();
foo.close();
```

# Operators

Shorthand and operators are the same as Python. Party!!! :tada:

Class Name and File name same in Java


