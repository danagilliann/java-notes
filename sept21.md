# 9/21
## Short-Circuiting
- If not parenthesized, a thing could possibly change the whole outcome
## Type Coercion and Casting
- Java variables must only have one type throughout the program
```java 
long l = Interger.MAX_VALUE + 1l;
int i = (int) l; // giving compiler approval and type coercion
```
- Type casting just cuts things to adjust the type
- Widening conversions are safe but shortening them can be tricky
## Random numbers
- Pseudo random vs. Random numbers
- Use `Math.random` and do not use `Random.nextInt()`
- `Math.random`
	- Floating number greater than 0 and less than 1
	- To get numbers greater than 1, multiply it by 10
```java
int r = (int) (Math.random() * 10);
```
- Formula for range
```
a + (Math.random() * b) where
a - the min of range
b - size of the range
```
## Formatting Output
```java 
boolean x = true;
System.out.printf("if x is %b and y is %b, then x && y is %b", x, true, x && true);
```
- Replace output
- Format specifiers to get fancy
``` 
%W.PC where
W - width
P - precision
C - type 
```
