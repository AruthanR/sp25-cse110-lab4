1. values added:  20

2. final result:  20

3. Using var can cause bugs because it doesn’t follow block scope and gets moved to the top of its function, making it easy to access or change it by mistake.

4. values added:  20

5. Error: result is not defined. Because let is block-scoped, result is not accessible outside the if block, so referencing it on line 13 causes a ReferenceError.

6. Error: Assignment to constant variable. Because const creates an immutable binding, line 7 attempts to reassign result (which was initialized to 0), causing an error.

7. Since the code already throws an error at line 7, line 13 is never reached.
