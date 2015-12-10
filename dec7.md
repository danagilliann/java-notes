# 12/7

## ArrayList
- No primitives, can store wrapper types
- Access with memory calls

## HashMap
- Dictionary
- Built over an array
- Built over an array
- Built over an array
- Built over an array
- Built over an array
- Built over an array
- Order does not matter
- Refer by key as opposed to index --> Key can be anything
```java
HashMap <String, Pokemon> myMap;
// initialize the map
myMap = new HashMap<>();
```
- Checking if a key exists
```java
if ( myMap.get(“Charmander”) == null ) {
  // create a new object
  Pokemon temp = new Pokemon();
  // put it into the map
  myMap.put(“Charmander”, temp);
}
```
- Keys must be unique
- If you add a value to an existing key, override value
- Enhanced for loop
```java
for (String key : myMap.keySet() ) {
  // grab a reference
  Pokemon temp = myMap.get(key);
  // do something
  System.out.println( temp.name );
}
```
  - Can loop over values and key and values
  - `.keySet()` is a set (bc you can't have repeating values)
  - Can do it for almost any data structure
- Key --> Hash function --> Integer --> Gets value associated with Integer

## Recursion
- Method that calls itself
- Problem --> Subproblem --> Recursive call
- Base case && recursive call
- Base case
  - Stop recursing
  - End recursive call
- Stack frame on call stack
```
|-----------------|
|                 |
|   Stack Frame   |
|-----------------|
|                 |
|   Stack Frame   |   <---- Call Stack
|-----------------|
|                 |
|   Stack Frame   |
|-----------------|

```
- Divide and conquer approach
- Important
  1. HAVE A BASE CASE!!
  2. Make progress
- If no base case, StackOverflow!
- Some problems are easier to solve recursively

## Memoization
- Caching
- Done with a HashMap
- Space/Time trade-off
