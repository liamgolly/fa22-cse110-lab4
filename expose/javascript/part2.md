Part 2
   1. The output is '3'. This is because after the last execution of the for loop, i will be equal to prices.length and break out of the loop without executing.
   2. The output is '150', as this is the last thing that the for loop will set it to by setting it to prices[2] * (1-0.5)
   3. The output to this line is also 150, as it is just a rounded version of discounted price, which was alraedy a whole number.
   4. The function returns an array, where each elment is the input array discoutned by the discount that is passed in. For the example given, it will be [50, 100, 150].
   5. The code returns an error, as in line 12 it is attempting to access the variable 'i', however it is a let that is defined within the scope of the for loop and therefore does not exist outside of it.
   6. The code returns an error, as discountedPrice was defined within the for loop as a let, and therefore the console.log is not within the scope of the variable.
   7. The code returns 150, as final price is defined within the same scope as the console.log statement and is set within the for loop in the same way  as it was in (3).
   8. The function returns the same thing as is returned in (4), for the same reason.
   9. The function errors, as i is a let that is defined within the scope of the for loop, and does note exist in the scope of the print statement.
   10. The code returns 3, as it is a constant value that is set to the length of the input prices, which is 3.
   11. The function returns the discounted prices of each of the input prices. This does not run into the problem of const assigning to discounted because pushing to a constant array is legal, as it doesn't reassign the constant variable.
   12. Notation
       1.  `student['name']`
       2.  `student['Grad Year']`
       3.  `student['greeting']()`
       4.  `student['Favorite Teacher']['name']`
       5.  `student['courseLoad'][0]`
   13. Arithmetic
       1.  `'3' + 2` outputs '32', as it is using the + operator as string concat, and appending '2' as a string to the string '3'.
       2.  `'3' - 2` outputs 1, as subtraction is a math operation as you cannot perform subtraction on a string, so the 3 is cast to a number.
       3.  `3 + null` outputs 3, as the null is cast to 0.
       4.  `'3' + null` outputs '3null', as it is attempting to do string concat with null, so it is reading null as a string.
       5.  `true + 3` outputs 4, as true is equal to '1' like in C.
       6.  `false + null` outputs 0, as false is 0 with addition, and null is also 0.
       7.  `'3' + undefined` outputs '3undefined', as undefined is being read as a string and therefore string concat is happening here.
       8.  `'3' - undefined` outputs NaN, as it is attempting to perform math on undefined.
   14. Comparison
       1.  `'2' > 1` outputs true, as it is casting the string to an number.
       2.  `'2' < '12'` outputs false, as it is comparing to the first character of the string first, and ending after that.
       3.  `2 == '2'` outputs true, as once cast these two are equal.
       4.  `2 === '2'` returns false, as these are not of the same type.
       5.  `true == 2` returns false, as true casts to 1.
       6.  `true === Boolean(2)` returns true, as Boolean(2) is true, as 2 is not 0.
   15. The `==` operator compares equality between two elements, and will attempt to cast to see if the elements are equal after casting. The `===` operator will check if the elements are the same value AND type.
   16. Check part2-question16.js
   17. The function will return a new array containing the values [2, 4, 6]. The function iterates through the input array, and gets the value of the array element passed into the callback function, and returns an array that contains the new values. In this case, the callback multiplied the input by 2, so when we pass in [1, 2, 3], the modifyArray function calls doSomething on each element, effectively doubling every value in the passed in array.
   18. Check part2-question18.js
   19. The output of the code is 1 4 3 2.