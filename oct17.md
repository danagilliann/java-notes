# 2-D Arrays
- Aka creating a database using Java

## Declaration
```java
elementType [][] arrayName;
double [][] myDopeArray;
```

## Creating an Arrauy
- "Standard" version
```java
arrayName = new elementType [noOfRows][noOfColumns];
// Example
myDopeArray = new double [8][4];
```
- Ragged Array
```java
arrayName = new elementType [noOfRows][];
for (int i=0; i < arrayName.length; ++i) { 
	arrayName[i] = new elementType[noOfColsInRow];
}
// Example
myDopeArray = new double [8][];
for (int i=0; i < arrayName.length; ++i) { 
	myDopeArray = new double[4];
}
```

## Accessing individual elements
```java
arrayName[rowIndex][columnIndex]
zeroTwo = myDopeArray[0][2]
threeFour = myDopeArray[3][4]
```

## Processing two-dimensional arrays
- Nested for loops often used
```java
double [][] nums = new double[50][150];
for (int row=0; row < nums.length; ++row) { 
	for (int col=0; col < nums[row].length; ++col) { 
		numbers[row][col] = value;
	}
}
```
- Printing values on a diagonal of a square two-dimensional array
```java
double [][] numbers = new double [50][50];
for (int row=0; row < numbers.length; ++row) { 
	if (numbers.length != numbers[row].length) { 
		System.err.println("Error: array not square");
	}
	System.out.println(numbers[row][row]);
}
```
