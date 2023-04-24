# SWAP-using-Pointers

We ask the user to enter values for variable a and b. We pass the address of variable a and b to function swap().

Inside function swap() we take a local variable temp. Since address of variable a and b are passed to swap() method, we take 2 pointer variables *x and *y. Pointer variable x holds the address of a and pointer variable y holds the address of b. Using below logic we swap the values present at address a( or x ) and b( or y ).


temp = *x;

*x = *y;

*y = temp;

Since we are directly changing the value present at particular address, the value gets reflected throughout the program and not just inside particular function. That’s why we are able to print the result inside main function and the values of variable a and b are swapped, without getting any returned value from function swap().
