# Overview
The BasicMath program is a simple C++ console application that allows users to perform basic arithmetic operations: addition, subtraction, multiplication, division, and modulus. The program prompts the user to input two numbers and then select the desired operation.

## Class: BasicMath
* Public Methods:
int addnum(int x, int y): Returns the sum of x and y.
int subnum(int x, int y): Returns the difference when y is subtracted from x.
int multnum(int x, int y): Returns the product of x and y.
int divnum(int x, int y): Returns the quotient of x divided by y.
int modnum(int x, int y): Returns the remainder when x is divided by y.

## Main Function
### 1. Input:

Prompts the user to enter two integers, x and y.
Asks the user to choose a mathematical operation by selecting a corresponding character:
- 'A' for addition
- 'S' for subtraction
- 'M' for multiplication
- 'D' for division
- 'G' for modulus

### 2. Processing:

Depending on the user's choice, the program calls the appropriate method from the BasicMath class to perform the operation.
For division, the program includes a basic check to handle cases where division by zero might occur, though the condition x < 0 || y < 0 does not effectively prevent this error.

### 3. Output:
Displays the result of the chosen operation or an error message for invalid inputs.

## Error Handling
The program does not handle division by zero and may crash if this operation is attempted with a zero divisor. The error handling for negative numbers in division seems misdirected as it should focus on zero division checks.
## Notes
The divnum method assumes valid non-zero divisor inputs, and the modulus operation similarly assumes valid inputs.
For accurate division results, consider using floating-point numbers instead of integers.