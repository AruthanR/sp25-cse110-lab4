1. At line 12, the code prints 3 because i is declared with var, which is function-scoped. This means i remains accessible outside the for loop, and after the loop ends, its value is 3, so it is printed without error.

2. Line 13 prints 150 because discountedPrice is declared with var, making it function-scoped. This means it's still accessible outside the for loop, and after the loop ends, it holds the last calculated value from the final iteration.

3. At line 14, the code prints 150, which is the last value assigned to finalPrice inside the loop. This works without error because finalPrice is declared with var, making it function-scoped and accessible anywhere within the discountPrices function, including after the loop.

4. This function will return [50, 100, 150]. Each element in the input array [100, 200, 300] is multiplied by 0.5 (i.e., discounted by 50%), and the result is rounded to the nearest whole number. These final prices are pushed to the discounted array. Since there are no scoping issues or errors, the function successfully returns the array of rounded discounted prices.

5. At line 12, the code will throw a ReferenceError because i is declared with let, which is block-scoped. This means i only exists inside the for loop block, and trying to access it outside the loop (like on line 12) causes an error since it's no longer in scope.

6. At line 13, the code will throw a ReferenceError because discountedPrice is declared with let, which is block-scoped. Since it was defined inside the for loop block, it cannot be accessed outside the loop, and trying to log it after the loop ends causes an error.

7. At line 14, the code will print 150. This works because finalPrice is declared with let at the top of the function, giving it function scope. It is updated inside the loop and still accessible after the loop ends, so console.log(finalPrice) prints the last value assigned to it.

8. This function will return [50, 100, 150]. Each price in the array [100, 200, 300] is discounted by 50% (using the formula price * (1 - discount)), then rounded and added to the discounted array. The use of let ensures variables are properly scoped, and no errors occur. The function runs as expected and returns the array of discounted prices.

9. At line 11, the code will throw a ReferenceError because i is declared using let, which is block-scoped within the for loop. This means i is not accessible outside the loop, so attempting to log it on line 11 causes an error.

10. At line 12, the code will print 3. This works because length is declared with const in the function scope and is assigned the value prices.length, which is 3 for the input [100, 200, 300]. Since length is accessible throughout the function, console.log(length) runs without error.

11. The function returns [50, 100, 150] because each price is discounted by 50% and added to the array. Using const is fine here since the array is mutated, not reassigned.

12.
A. student.name  
B. student["Grad Year"]  
C. student.greeting()  
D. student["Favorite Teacher"].name  
E. student.courseLoad[0]

13. Arithmetic

A. '3' + 2 → '32'  
   - String concatenation occurs because one operand is a string.

B. '3' - 2 → 1  
   - The string '3' is coerced to a number, then subtraction happens.

C. 3 + null → 3  
   - null is coerced to 0, so the result is 3.

D. '3' + null → '3null'  
   - null is coerced to 'null' (string), so concatenation happens.

E. true + 3 → 4  
   - true becomes 1, so 1 + 3 = 4.

F. false + null → 0  
   - false is 0, null is 0, so 0 + 0 = 0.

G. '3' + undefined → '3undefined'  
   - undefined becomes 'undefined', so string concatenation occurs.

H. '3' - undefined → NaN  
   - '3' becomes 3, undefined becomes NaN → 3 - NaN = NaN

14. Comparison

A. '2' > 1 → true  
   - '2' is coerced to 2, and 2 > 1 is true.

B. '2' < '12' → false  
   - String comparison: '2' comes after '1' lexicographically.

C. 2 == '2' → true  
   - Type coercion makes both 2 before comparing, so true.

D. 2 === '2' → false  
   - Strict equality checks both type and value. Different types.

E. true == 2 → false  
   - true becomes 1, but 1 != 2.

F. true === Boolean(2) → true  
   - Boolean(2) is true, and both are of the same type and value.

15. The `==` operator compares values with type coercion, converting types if needed. The `===` operator checks both value and type without conversion.

16. in part2-question16.js

17. 









