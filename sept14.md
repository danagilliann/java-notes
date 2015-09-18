# 9/14
### Expressions vs Statements
Expression - Combination which evaluates to a value, can compound, do not exist by themselves
Statement - Smallest chunk of a program can contain an expression, cannot compound

```java
int z = 1+1
// 1 + 1 --> expression
// int z --> statement

// This will be a block
{ 
	System.out.println("Hello");
	System.out.println("World");
}
```

### Boolean Data Types
Must declare booleans
```java
boolean a = true;
boolean b = false;
boolean c = 10 > 1;

System.out.println("The value of c is " + c); // will print true
```
### If/else
if/else if vs. multiple if statements
- Multiple if statements not mutually exclusive

##### Ternary operator
```java
int test = 1 * 100 == 100 ? 5 : 6;
// Same as
int test = 1 * 100;
if (test == 100) { 
	test = 5;
} else { 
	test = 6;
}
```

### Switch statements
- For too many if/else statements
- Kind of JSON-looking
- Cases restrictions: int, char, str

```java 
int month = 1;
String monthString = "Unknown";
switch (month) { 
	case 1: monthString = "Jan";
					break; // breaks out of a switch
	case 2: monthString = "Feb"; // case value will match a variable, can also group cases
					break; // w/o break, it would print "Feb", fall-through behavior
	default: monthString = "Invalid month"; // if no matching cases, can be anywhere
}
System.out.println(monthString);
```

### Logical operators
- Short circuiting is helpful
- Short circuiting - Not evalutating the right hand
```
false && .. --> Will not evaluate the right
true || .. --> Will not evalutate the right
```
``` 
! - not
&& - and
|| - ord
^ - exclusive or
```
- Exclusive or
	- "One or the other, but not both"
	- Only one can be true
- Semi-colons ends EVERYTHING
- Braces are nice

### Helpful features 
- Command + / --> multi line
- Shift + Command + F --> Formatting
