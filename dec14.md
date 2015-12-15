# 12/14

- Make getters and mutators static
- Static
  - If getting/setting a static var, method must be static
  - Method on the class
  - Prefix it with name of class
  - Alternative: have var in params a different name
- Arrays
  - Check to see if array is null
- Constructor
  - Top-down approach
  - Subclasses automatically call the Constructor of its superclass
- Exceptions
  - `public static void statement(int i) throws Exception1, Exception2` --> example of checked exceptions
  - Checked exceptions must be thrown and must be caught
  - Typically, unchecked Exceptions are used
  
```java
if (i == 2) { // example of unchecked Exception
  throw new Exception(); 
```

  - `RuntimeException` is root of unchecked Exceptions, `IOException` root of checked Exception, `Exception` root of all Exceptions
  - Once an exception is caught, everything stops in try scope

```java
public static void main(String[] args) {
  try {
    statement(1);
    statement(2);
    statement(3); // will not execute
  } catch (IllegalArgumentException e) {
    System.out.println("IllegalArgumentException caught");
  } catch (RuntimeException e) {
    System.out.println("RuntimeException caught");
  }
  statement(4);
}

private static void statement(int i) {
  if(i == 2) {
    throw new IllegalArgumentException();
    // throw new RuntimeException();
  } else {
    System.out.println(i + "");
  }
}

```
- Abstract classes
  - ABSOLUTELY CANNOT CALL A METHOD ON THE STATIC TYPE IF IT DOES NOT EXIST ON A DYNAMIC TYPE
