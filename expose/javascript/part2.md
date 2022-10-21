1. What will happen at line 12 and why?  
   **Line 12 will return result of `3` because `i` was declared with `var` in line 6 that does not prevent it from accessing outside the `for` block scope. Hence, after `for` loop completes, `i` equals `3` as a result returned.**
2. What will happen at line 13 and why?  
   **Line 13 will return result of `150` because `discountedPrice` was also declared with `var` in line 7 that does not prevent it from accessing outside the `for` block scope. Hence, after `for` loop completes, `discountedPrice` equals `150` as a result returned.**
3. What will happen at line 14 and why?  
   **Line 14 will return result of `150` because `finalPrice` is inside the block scope of this function and is also declared with `var` in line 4 that does not prevent it from accessing either inside or outside the `for` block scope. Hence, after `for` loop completes, `finalPrice` equals `150` as a result returned.**
4. What will this function return? Give a brief explanation why. If the code causes an error, explain why.  
   **This function runs correctly but will return nothing to the web console since `console.log` is not used here to print out the result.**
5. What will happen at line 12 and why?  If the code causes an error, explain why. ^^^ (assume this function is being called like the others: discountPrices([100, 200, 300], 0.5))  
   **The code causes a ReferenceError because `i` was declared with `let` in line 6 that prevents it from accessing outside the `for` block scope. Therefore, when `console.log` is called to print the result of `i`, `i` is not defined yet after finishing the `for` block scope.**
6. What will happen at line 13 and why? If the code causes an error, explain why.  
   **Similar to question 5 above, the code also causes a ReferenceError because `discountedPrice` was declared with `let` in line 7 that prevents it from accessing outside the `for` block scope. Therefore, when `console.log` is called to print the result of `discountedPrice`, `discountedPrice` is still not defined yet after finishing the `for` block scope.**
7. What will happen at line 14 and why? If the code causes an error, explain why.  
   **Line 14 will return result of `150` because `finalPrice` was declared with `let` in line 4 inside the block scope of this function that does not prevent it from accessing either inside or outside the `for` block scope. Hence, after `for` loop completes, `finalPrice` equals `150` as a result returned.**
8. What will this function return? Give a brief explanation. If the code causes an error, explain why.  
   **`discounted` and `finalPrice` are declared with `let` inside the block scope of this function that do not prevent them being used either inside or outside the block scope of `for` loop and leading no errors. Also, `discountedPrice` and `i` are also declared with `let` and used inside the `for` block scope that will not cause any errors. Therefore, this function can be compiled correctly but will return nothing to the web console since `console.log` is not used here to print out the result.**
9. What will happen at line 11 and why? If the code causes an error, explain why.  
    **The line 11 will cause an error since `i` was declared with `let` in line 6 that prevents it from accessing outside the `for` block scope. Therefore, when `console.log` is called to print the result of `i`, `i` is not defined yet after finishing the `for` block scope.**
10. What will happen at line 12 and why? If the code causes an error, explain why.  
    **Line 12 will return result of `3` because `length` was declared with `const` in line 4 inside the block scope of this function that does not prevent it from accessing either inside or outside the `for` block scope. Also, `length` is not reassigned after it is assigned the first time in line 4. Hence, after `for` loop completes, `length` still equals `3` as a result returned.**
11. What will this function return? Give a brief explanation. If the code causes an error, explain why.  
    **`discounted` and `length` are declared with `const` inside the block scope of this function that do not prevent them being used either inside or outside the block scope of `for` loop and they are not reassign later after they are assigned in line 3 and 4. Also, `discountedPrice` is declared with `const` for every `i` that does not cause any errors. `i` is also declared with `let` and used inside the `for` block scope only that will not cause any errors either. Therefore, this function can be compiled correctly but will return nothing to the web console since `console.log` is not used here to print out the result.**
12. Given the above Object, write the notation for:  (These should be in your part2.md)
    - Accessing the value of the name property in the student object  
    **student.name**
    - Accessing the value of the Grad Year property in the student object  
    **student['Grad Year']**
    - Calling the function for the greeting property in the student object  
    **student.greeting()**
    - Accessing the name property of the object in the Favorite Teacher property in student  
    **student['Favorite Teacher'].name**
    - Access index zero in the array of the courseLoad property of the student object  
    **student.courseLoad[0]**
13. Arithmetic
    - ‘3’ + 2
    **`= '32'` since the first operand is a string, the compile will treat the second one as string as well and the result is the concatenation of 2 strings.**
    - ‘3’ - 2
    **`= 1` since the compile will automatically convert string to number `3` and implement the subtraction between two numbers.**
    - 3 + null
    **`= 3` since the compile will make numeric conversion on `null` to become number `0` and implement the math operation.**
    - ‘3’ + null
    **`= '3null'` since the first operand is a string, the compile will also treat `null` as a string and the result is the concatenation of 2 strings.**
    - true + 3
    **`= 4` since the first operand is a boolean, the compile will make numeric conversion on `true` to become `1` and results in `4`.**
    - false + null
    **`= 0` since the compile will make numeric conversion on `false` to become `0` and `null` to become `0`.**
    - '3' + undefined
    **`= '3undefined'` since the first operand is a string, the compile will treat the second one as string as well and the result is the concatenation of 2 strings.**
    - '3' - undefined
    **`= NaN` since the compile will convert the first operand to number `3` and the second operand `undefined` to `NaN`, so this subtraction between a number and `Not a Number` will get Not A Number.**
14. Comparison
    - ‘2’ > 1  
    **This is `true` since `2` will become a number `2` and implement comparison of two same types.**
    - ‘2’ < ‘12’  
    **This is `false` since this is string comparison and strings are compared letter-by-letter. Hence, `2 < 1` is false**
    - 2 == ‘2’  
    **This is `true` since the string `2` becomes number 2 and 2 equals 2.**
    - 2 === ‘2’  
    **This is `false` since strict euality operator `===` checks the equality without type conversion. Hence, 2 and '2' are different types that results in `false`**
    - true == 2  
    **This is `false` since `true` becomes a number `1` and 1 does not equal 2**
    - true === Boolean(2)  
    **This is `true` because a strict euality operator `===` checks the equality without type conversion and `Boolean(2)` results in `true`**
15. Explain the difference between the == and === operators.
    **`===` is a strict equality operator that checks the equality without type conversion. This also means the result will return false immediately while comparing two different types without type conversion. Meanwhile `==` will check the comparison after type conversion happens, so it cannot differentiate the different types.**
16. [part2-question16.js](expose\javascript\part2-question16.js)
17. If the function above is called with the following parameters modifyArray([1,2,3], doSomething), what will be the result? Briefly walk through how you arrived at that result. (This should be in your part2.md). Here we are passing in a function as a parameter, however we can also return a function from another function just as easily, you're encouraged to play around with callbacks as they are used heavily in frontend JS development.  
    **The result of newArr is an array of `[2,4,6]`.**  
    Firstly, the function `modifyArray([1,2,3], doSomething)` is called, newArr starts with an empty array before `for` loop runs. In the second step, while running `for` loop, for every `i`, the `callback` will call `doSomething(num)` function and pass `array[i]` as its parameter `num`. The `doSomething(sum)` function returns the value of `2 * num` where `num` is passed by the value of `array[i]` and this result will be pushed back to `newArr` array. This step will repeat and continue until `for` loop is done. Hence, `newArr` finally return an array of `[2, 4, 6]`.
18. [part2-question18.js](expose\javascript\part2-question18.js)
19. What is the output of the above code? (This should be in your part2.md)
    **The output of the code is `1 4 3 2`**
