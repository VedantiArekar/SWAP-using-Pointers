# SWAP-using-Pointers

Swapping values using pointer

Swapping of values of variables by using pointers is a great example of calling functions by call by reference.
Functions can be called in two ways:


1. Call by Value

2. Call by reference

In call by value, a copy of actual arguments is passed to formal arguments of the called function. Any change made to the formal arguments in the called function has no effect on the values of actual arguments in the calling function.

In call by reference method, the address of the actual parameter is passed into the formal parameter. Inside the function, the address is used to access the actual argument. Any changes made to the formal parameters are also made to the actual parameters, since the changes are being made to the same location in memory.

We ask the user to enter values for variable a and b. We pass the address of variable a and b to function swap().

Inside function swap() we take a local variable temp. Since address of variable a and b are passed to swap() method, we take 2 pointer variables *x and *y. Pointer variable x holds the address of a and pointer variable y holds the address of b. Using below logic we swap the values present at address a( or x ) and b( or y ).


temp = *x;

*x = *y;

*y = temp;

Since we are directly changing the value present at particular address, the value gets reflected throughout the program and not just inside particular function. That’s why we are able to print the result inside main function and the values of variable a and b are swapped, without getting any returned value from function swap().
