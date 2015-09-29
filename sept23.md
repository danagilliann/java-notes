# 9/23
## Characters
```java
char c = 'c';
```
- 16-bit Unicode character
- Unicode --> Character to numbers
- Can cast as an integer and becomes Unicode value, can also cast ints to chars
```java
int i = (int) 'A'; // i becomes 65
```
- Some chars require casting to fit into a variable, narrowing conversions 
- Short and chars both 16-bit

## Binary
- Computers only understand things with Base 2 because range is only 0-1
- When a computer approaches a max-value, it will approach a min-value (and vice-versa)
- Module, divide by 2

## Strings (Strangs)
- Offset, distance from the first character
```java
String s = 'Hello';
char c = s.charAt(1); // prints 'e'
```
- Lowercase and uppercase
```java
String a = s.toUpperCase();
String b = s.toLowerCase();
```
- Cannot compare two strings with `==`
```java
String x = "Hello";
String y = "Hello";
System.out.println(x == y); // may return false cause oop
System.out.println(x.equals(y); // returns true 24/7 all day errrday. Just use the built-in methods girl
```
- Getting a character from user input
```java
char cInput = in.next().charAt(0) // Bc turns out there's no nextChar()
```
- Getting the index
```java
String x = "Hello";
System.out.println(x.indexOf("H");
```

