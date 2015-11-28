# 11/23e 

## Exception Handling/File I/O
- Use try/catch block

```java
try {
  System.out.println(divide(78, 3));
  System.out.println(divide(78, 0));
} catch ( ArithmeticException e ) { // e can be anything. It's the variable of the exception
  System.out.println("you should know better than trying to divide by zero");
}
```

- RuntimeExceptions are things that do not need to be try/catched for
- General rule of thumb: If you can use if/else, use it to prevent example
- For using Scanner, make sure you clear the buffer otherwise it caches
- You can get information from the `e` or Exception variable
- When you print the `e`, it gets printed as a String
- Catch the mother of all Exceptions to catch all Exceptions
- When the exception is seen, the `catch` block gets executed immediately and rest of program is ignored

## File Class
- Represents abstract file in computer
- Unix epoch - 0 for time for the computer
- `Scanner` to be used for reading files
- For reading files, an Exception must be thrown
- Detect error first, but even if you handle the exception, chance that you could still run into that same exception
- Do a file check using `file.exists()`
