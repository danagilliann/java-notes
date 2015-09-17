# 9/16
## Strings (Strangz)
- Strings can be taken as input
```java 
Scanner in = new Scanner(System.in);
String name = in.next(); // Note the .next() method
```

- String concatenations
```java 
String greeting = "Hello" + name + "!";
```

## Increments and Decrements
```java
int x = 0;
x++; // adds 1 to x, postfix
++x; // also adds 1 to x, prefix
```
```java 
int y = 100;
y-- // minus 1 from y, postfix
--y // also minus 1 from y, prefix
```
- `++x` and `x++` is important because of precedence. `x++` takes less precedence.
- Basically just do postfix for asap results

## While loops
```java 
int count = 0:
while (count < 10) { 
	System.out.println(count);
	++count;
}
```
- Do while loop, will happen at least once. Unlike while loops which require a thing to be true before another thing executes
```java 
int count = 0;
do { 
	System.out.println(count);
	++count;
} while (count < 0);
```
- Sentinel --> a value which is the "break" for the while loop

## For loops
```java 
// Prints 0-9
// While k is less than 10, print k, add +1 to k after every iteration
for (int k=0; k<10; k++) { 
	System.out.println(k)
}
```
- Nested for-loops
```java
int i;
for (i=0; i<2; i++) { 
	for (int j=0; j<2; j++) { 
		System.out.println(j);
	}
}
```
- Second for loop highly dependent on the first loop
- Protip: Multiply the two constraints of i and j to see how many times the `System.out.println` prints
- Infinite loop:

```java 
for (;;) { 
	System.out.println("Forever and ever!);
}
```
-`continue` --> Skips to next iteration of loop for short circuiting
-`break` --> Get tf out of the loop

```java
for (int k=0; k<10; k++) {  
	if (k == 3) { 
		System.out.println(k);
		continue; // Ignore past this point
	}
	
	if (k % 2 == 0) { 
		System.out.println("Bye!");
		break;
	}

}
```

