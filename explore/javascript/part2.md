1. The console logs the value of i, which is '3' because that is the index at which the for loop terminates.
2. The console logs the discountedPrice, which is '150' because the current value of discountedPrice is the value of the last index of prices, multipled by (1 - 0.5). 300 * 0.5 = 150.
3. The console logs the finalPrice, which is '150' because the current value of finalPrice is just the value of discountedPrice multiplied by 100, rounded, and divded by 100. Math.round(150 * 100)/100 is clearly 150.
4. This function will return an array [50, 100, 150]. For every value in the argument 'prices', the function finds their discounted value based on the argument 'discount' and appends them to an array 'discounted,' which is the return value. In this case, every value in prices [100, 200, 300] is discounted by 0.5. 
5. The code returns an error because the function call console.log(i) tries to access 'i', which is a block scope variable declared with 'let' that is only accessible in the for loop.  
6. The code returns an error because the function call console.log(discountedPrice) tries to access 'discountedPrice', which is a block scope variable declared with 'let' that is only accessible in the for loop. 
7. The console logs the finalPrice, which is '150', just like in question 3. There is no error because the scope of finalPrice is the entire function discountPrices(), as finalPrice was declared with 'let' at the beginning of the function.
8. This function will return an array [50, 100, 150], just like in question 4. There is no error because the return value 'discounted' has a scope that is the entire function discountPrices(), as 'discounted' was declared with 'let' at the beginning of the function.
9. The code returns an error because the function call console.log(i) tries to access 'i', which is a block scope variable declared with 'let' that is only accessible in the for loop.
10. The console logs the value of 'length', initally declared as 'prices.length', which is '3' because that is the size of the array 'prices.' There is no scope-related error because length was declared at the beginning of the function.
11. This function will return an array [50, 100, 150], just like in question 4 and 8. Even though the array 'discounted' was declared with 'const', we are still allowed to push new values to it, so long as we do not assign the variable to a new array. 
    
12. 
A. student.name     
B. student['Grad Year']   
C. student.greeting();      
D. student["Favorite Teacher"].name
E. student.courseLoad[0]  

13.  
A. 32
Integers map to their exact string representation so '3' + 2 concatenates two strings instead of adding two integers.
B. 1
The operation being performed is subtraction, so no string conversion can take place. '3' undergoes numeric conversion, leading to an interpretation of just 3 - 2.
C. 3
The first value 3 is a number, so the second value undergoes numeric conversion from null to 0, leading to an interpretation of 3 + 0.
D. 3null
The first value 3 is a string, so the second value is also interpreted as a string. The two strings are concatenated to form '3null'.
E. 4
Because one of the two values is a number and the other is a boolean value, the boolean value undergoes numeric conversion and becomes 1. 3 + 1 = 4.
F. 0
There are no string values in the two terms so both false and null undergo numeric conversion. 0 + 0 = 0.
G. 3undefined
Because the first value is a string, the second value 'undefined' is also treated as a string, and the two terms are concatenated. 
H. NaN
Because the operation being performed is subtraction, no string conversion can take place. Therefore both '3' and undefined undergo numeric conversion, leading to 3 - NaN, which is just NaN because the operation being performed is undefined. 

14. 
A. True
When comparing values of different types, numeric conversion is done. 2 > 1 is true.
B. False
The strings '2' > '12' as the character '2' > the character '1'.
C. True
Using the non-strict equality operator, the string side undergoes numeric conversion and we find that 2 == 2.
D. False
Using the strict equality operator, we find that both sides are of different types and are therefore unequal.
E. False
Numeric conversion turns true into 1, and 1 !== 2. 
F. True
Boolean(2) turns the right side into true as 2 is a value that falls under that criteria. Both sides are therefore the boolean true and are equal under the strict equality operator.

15.  '==' compares the equality of two terms with respect to type conversion, i.e. '0' == false. '===' compares the equality of two terms without respect to type conversion, i.e. '0' !=== false. 

16. See part2-question16.js

17. The result is that newArr will be returned with value [2, 4, 6]. When modifyArray() is called, the program enters a for loop that runs callback() on every value at every index. In this case, callback() is the doSomething() function, which returns double the value of the argument. 
    
18. See part2-question18.js
    
19. 
1
4
3
2