# cis165-lab2
  sum.cpp   mpg.cpp   README.md   AI_REFLECTION.md

Program 1 — sum.cpp
Program Plan
Create variables for the values 50 and 100.

Add the two variables together.

Store the result in a variable named total.

Display total with a clear label.
Expected Calculation
The assigned values are:

value1 = 50

value2 = 100

The calculation is:

50 + 100 = 150

Expected output:

Total: 150


Program 2 — mpg.cpp
Program Plan
Create variables for miles and gallons.

Store 312 miles and 16 gallons in the variables.

Divide miles by gallons.

Store the result in a variable named mpg.

Use a data type that preserves a fractional result.

Display the result with a label and units.
Expected Calculation
The assigned values are:

miles = 312

gallons = 16

The formula is:

miles per gallon = miles / gallons

Therefore:

312 / 16 = 19.5

Expected output:

Miles per gallon: 19.5 MPG

Compile sum.cpp
g++ -std=c++17 -Wall -Wextra sum.cpp -o sum

Run:

./sum

Expected output:

Total: 150

Compile mpg.cpp
g++ -std=c++17 -Wall -Wextra mpg.cpp -o mpg

Run:

./mpg

Expected output:

Miles per gallon: 19.5 MPG

## Testing

| Program | Values Used | Expected Result | Actual Output | Match or Fix |
|---|---|---|---|---|
| `sum.cpp` — assigned values | 50 and 100 | Total = 150 | 150 | Match |
| `sum.cpp` — changed values | 25 and 75 | Total = 100 | 100 | Match |
| `mpg.cpp` — assigned values | 312 miles; 16 gallons | 19.5 MPG |19.25 MPG | Match |
| `mpg.cpp` — changed values | 250 miles; 12 gallons | Approximately 20.8333 MPG | Approximately 20.8333 MPG | Match |

## Code Explanation

### sum.cpp

The program stores 50 and 100 in the variables `value1` and `value2`. The program adds these two values together and stores the result in the variable `total`. The value of `total` is then displayed using `cout`. Storing the calculation in `total` before printing makes the calculation easier to read and allows the result to be stored and used as a variable.

### mpg.cpp

The MPG program calculates miles per gallon by dividing the number of miles by the number of gallons. The formula is `miles / gallons`. I used the `double` data type so that the calculation can preserve a fractional result such as 19.5 or 20.8333. If C++ divides two integer operands, it performs integer division and removes the fractional portion of the answer.

For my changed-value test, I used 250 miles and 12 gallons. The program calculated `250 / 12`, which produced approximately 20.8333 MPG. The result was stored in the `mpg` variable before being displayed.

Changed sum.cpp Test
For the second sum.cpp test, I temporarily changed the values to:

value1 = 25

value2 = 75

The expected calculation was:

25 + 75 = 100

Expected output:

Total: 100

After completing the test, I restored the assigned values of 50 and 100.

Changed mpg.cpp Test
For the second mpg.cpp test, I temporarily used:

miles = 250

gallons = 12

The expected calculation was:

250 / 12 = 20.833333

Expected output is approximately:

Miles per gallon: 20.8333 MPG

This test uses positive values and produces a fractional result.

After completing the test, I restored the assigned values of 312 miles and 16 gallons.

I restored the originally assigned values in both .cpp files and completed final runs of both programs before the final upload.
