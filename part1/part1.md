## 1a)
1. values added: 20
2. final result: 20
3. values added: 20
4. There is an error because the 'let' keyword was used and therefore the 'result' variable is considered defined only
   in the block it was defined within. Thus the else block considered the variable undefined.

5. There would be an error because on line 7 we are attempting to change the value of a const variable. 
6. Again, there is an error because on line 7 we attempted to change the value of a const variable, and also even if that were not an 
    issue, there would be a scope issue. 


<br>

## 1b)
1. The value '3' will be logged to the console. This is because var has no block scope, meaning it is visible through blocks and thus this means that the variable 'i' can be seen outside the for loop block. 
2. The value '150' will be logged to the console. This is because var has no block scope, meaning it is visible through blocks and thus this means that the variable 'discountedPrice' can be seen outside the for loop block. 
3. The value '150' will be logged to the console. There for sure wont be a scope issue since finalPrice is declared in the same scope that console.log(finalPrice) is called. finalPrice is initialized as 0, but after the for loop, the final iteration sets it to 150. 
4. The function will a return an array of the discounted values, those discount values being: [50, 100, 150]. The discounted array variable is declared in the same scope that the return statement is made in so there for sure can be no scope issues. The for loop goes through three iterations, calculating the 50% off prices of each of the three prices being passed as parameter (100, 200 and 300).
5. There will be an error because the variable 'i' is not considered defined outside the for loop block scope since it was initialized with the let keyword.
6. Again, there will be an error because the variable 'discountedPrice' is not considered defined outside the for loop block scope because it was initialized with the let keyword.
7. The value '150' will be logged to the console. There is no scope issue because the variable final price was initialized in the same scope as the console.log(finalPrice) line. 
8. The function will a return an array of the discounted values, those discount values being: [50, 100, 150]. There is no scope issue because the discounted array is declared in the same scope as the return statement. 
9. There will be an error because the variable 'i' is not considered defined outside the for loop block scope since it was initialized with the let keyword.
10. The value '3' will be logged to the console, because there are three values in the array passed as parameter. Variables declared with const have the same scope rules as variables declared with let, so there's no scope issue. 
11. The function will a return an array of the discounted values, those discount values being: [50, 100, 150]. Variables declared with const have the same scope rules as variables declared with let, so there's no scope issue.
12.    
       - A) student.name
       - B) student['Grad Year'] 
       - C) student.greeting()
       - D) (student['Favorite Teacher']).name
       - E) student.courseLoad[0]

13. 
       - A) Output: '32'.  This is because the integer 2 maps to its string representation, and it is concatenated with the string '3'
       - B) Output: 1  .   This is because the string '3' is numerically converted to the number 3
       - C) Output: 3  .   This is becuase the numeric conversion of null is that it becomes 0
       - D) Output: '3null' . This is because null is considered a string to be concatenated with the string '3'
       - E) Output: 4 .This is because the numeric conversion for true is 1
       - F) Output: 0 .This is because the numeric conversion for both false and null is 0
       - G) Output: '3undefined' .Similarly to D, undefined is considered a string to be concatenated with the string '3'
       - H) Output: NaN .This is because the numeric conversion of undefined is NaN

14. 
       - A) Output: true.  Values of different types in a comparison are converted to numbers
       - B) Output: false. This is because two strings are being compared, and so the strings are compared letter by letter based on their Unicode values. The unicode value of 2 is greater than 1, so it returns false. 
       - C) Output: true. For regular equality checks of values with different types, Javascript converts them to numbers. 
       - D) Output: false. The strict equality operator does not perform type conversion. 
       - E) Output: false. Values of different typse are converted to numbers for comparisons, and the numeric value of true is 1. 
       - F) Output: true. For boolean conversions, "empty" values like 0, an empty string, null, undefined and NaN become false, and other values become true. So, since 2 doesn't fall into the former category, it converts to true. 

15. The regular equality operator == performs numeric type conversions when there are values of two different types being compared. The === operator is a strict equality check that does not perform type conversion. If two values are compared with === and they are of different types then false is returned. 

16. (Answer in part1b-question16.js file)
17. The modifyArray([1,2,3], doSomething) command will return an array with the values [2,4,6]. The modifyArray function is called, and as parameter the array [1,2,3] is passed, and the doSomething function is passed as parameter as well. In the modifyArray function, a new array is initialized and for each element in the array passed as parameter, doSomething (which is the callback function that was stored as parameter) is called on the element. So, the elements of the array [1,2,3] are iterated through and doSomething() is called on them, which multiplies these numbers by two. The product of each iteration is stored in the new array which is returned by the function at the end. 
18. (Aswer in part1b-question18.js)

19. 
    1 <br>
    4 <br>
    3 <br>
    2 <br>
    



