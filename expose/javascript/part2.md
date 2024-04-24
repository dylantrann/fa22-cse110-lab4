# Part 2

1. `3` is printed. This is because the variable `i` was declared as a `var`, which makes it a global variable accessible outside of it's normal scope. 

2. `150` is printed. This is because `150` was the last price discounted using the temp variable `discountedPrice`. Since `discountedPrice` was declared as a `var`, it is accessible outside the scope of the for loop and maintained it's latest assignment, which was `150`. 

3. `150` is printed. This is for the same reasons as #2, such that the variable `finalPrice` was last updated with the number `150`, meaning that printing it would display its most recent assignment. It was declared before the for loop, so the print message is still within it's natural scope. 

4. The function will return an array consisting of all the discounted prices of their original input: `[ 50, 100, 150 ]`. This is because the function `discountPrices` takes in an array (100, 200, 300) and reduces each of it's elements by a discount multiplier (0.5). Each input is muliplied by the discount factor and appended to a new array, which is returned at the end of the function call.

5. It causes an error. This is because the variable `i` wasn't declared in the scope of the print statement. The variable `i` was declared using `let`, which means it is limited by the scope in which it was called in. Thus, `i` cannot be access outside of the for loop it was declared within.

6. It causes an error. This is for the same reasons as #6 such that the variable `discountedPrice` was declared with `let`, meaning it is restricted in accessibility by the scope of the for loop it was declared within. 

7. `150` is printed. This is because the variable `finalPrice` is within the same scope as the print statement. The variable `finalPrice` was declared using `let`, meaning that it's only accessible within the scope it was declared in. The scope of `finalPrice` is the entirety of the function `discountPrices`, which means it is printable by line 14. 

8. It returns the array of discounted prices: `[ 50, 100, 150 ]`. This is just the functionality of the function `discountPrices`, as it returns an array representing the discounted version of the inputed array. 

9. It causes an error. This is because the print statement tries to access a variable out of scope. The variable `i` was declared usign `let`, meaning that it is only accessible within the scope of the for loop it was declared within. 

10. `3` is printed. This is because the print statement at line 12 is within the scope of the variable it is trying to print, `length`. 

11. It surprisingly returns the correct array: `[ 50, 100, 150 ]`. The reason line 7 doesn't cause an error is because it redeclares the variable `discountedPrice` each time it updates, meaning that it doesn't break the conventions created by the `const` declaration. Line 8 also doesn't cause an error because the variable `discounted` isn't being reassigned, only the object that is assigned to it is being manipulated. 

12. Object Notation
    - a. student.name
    - b. student["Grad Year"]
    - c. student.greeting()
    - d. student["Favorite Teacher"].name
    - e. student.courseLoad[0]

13. Arithmetic
    - a. `'32'`. This is because integers map to their exact string representations. It was like appedning `'2'` to the string `'3'`.
    - b. `1`. There is no string protocol using the minus sign so the equation is treated as an integer one. 
    - c. `3`. Null becomes 0.
    - d. `'3null'`. `null` is treated as a string literal and is appended to the string `'3'`. 
    - e. `4`. `true` gets converted to `1` so its just `3 + 1 = 4`.
    - f. `0`. `false` and `null` are both converted into `0`, so `0 + 0 = 0`
    - g. `'3undefined'`. `undefined` is converted to a string literal and is appended to the string `3`. 
    - h. `NaN`. Since there is no string protocol using minus, it is treated as integer arithmetic. Any integer arithmetic using undefined results in `NaN`. 

14. Comparison
    - a. `true`. `'2'` becomes an integer and `2 > 1`.
    - b. `false`. They are treated as strings in which `'2' > '1'` so it returns `false`. 
    - c. `true`. They are converted to match types.
    - d. `false`. Checks equality without type conversion, thus false by default since they're different types. 
    - e. `false`. `true` is represented by `1` as an integer conversion, not `2`. 
    - f. `true`. The function `Boolean(n)` returns `true` for any non-zero integer as n. 

15. The double equals comparator checks equality while allowing type conversions. The triple equals comparator doesn't allow for type conversions and does a strict check of equality. 

17. `[ 2, 4, 6 ]`. The function call starts by creating a new array at line 2. Then, for each element in  the old array, it is sent into the function `doSomething` and its new value is pushed into the new array. Basically, each element in the argumented array gets changed based on `doSomething`, which in this case multiplies the original by 2. Thus, the returned array is just the original with each element multiplied by 2. 

19. `1`, `4`, `3`, `2`. Each are followed by a newline. `1` is printed first since its without a delay and the first function. `4` is next because it has no delay. `3` is third because it has a slight delay compared to the instantaeous functions. `2` is last because it has a delay of 1 second. 