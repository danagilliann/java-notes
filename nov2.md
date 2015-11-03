# 11/2
- this()
```java
class Car {
	private String color;
	private int year;
	private String make;

	public Car ( String color, int year, String make ) { // Constructor A
		this.color = color;
		this.year = year;
		this.make = make;
	}

	public Car ( ) {
		this( ”red”, 2014, ”Mazda” ); // This calls Constructor A with "red", 2014, and "Mazda" as parameters
	}
}
```
