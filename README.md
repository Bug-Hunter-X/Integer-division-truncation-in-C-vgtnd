# Integer Division Truncation in C
This example demonstrates a common issue in C: integer division truncation. Integer division in C always truncates the fractional part, resulting in an integer result. This behavior can be unexpected if you're working with values that you expect to have a fractional part.

**bug.c** contains a simple program demonstrating this truncation. The program divides 10 by 5 and prints the result. Although we might expect the result to be 2.0 (since 10/5 = 2.0), the actual output is 2 due to integer division's truncation behavior.  The bug lies in the implicit assumption that the division will yield a floating-point value. 

**bugSolution.c** demonstrates a corrected version by using floating-point data types to handle potential fractional results more accurately.
