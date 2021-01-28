1. `prices.length` will be printed, since `var` has function scope.
2. The value `discountedPrice` is assigned on line 6 is printed, since `var` has function scope.
3. The value `finalPrice` is assigned on line 7 during the last foor loop iteration is printed, since `var` has function scope.
4. `[50,100,150]` is returned, since the for loop will multiply each price by `(1-0.5 = 0.5)` to get a new price half of the original, which is then appended to `discounted`, and every variable is function-scoped.
5. A `ReferenceError` is thrown since `i` is not defined at the function scope, only in the for loop scope
6. A `ReferenceError` is thrown since `discountedPrice` is not defined at the function scope, only in the for loop scope
7. The value `finalPrice` is assigned on line 7 during the last foor loop iteration is printed, since the assignment is used a variable that has function scope, and not just for loop scope.
8. `[50,100,150]` is returned, since the for loop will multiply each price by `(1-0.5 = 0.5)` to get a new price half of the original, which is then appended to `discounted`, and discounted is function-scoped and therefore mutated.
9.  A `ReferenceError` is thrown since `i` is not defined at the function scope, only in the for loop scope
10. A `ReferenceError` is thrown since `discountedPrice` is not defined at the function scope, only in the for loop scope
11. 0 is printed. A `TypeError` would be thrown before line 13 (on line 7) since `finalPrice` can not be re-assigned, so assuming this doesn't throw an error, `finalPrice` will store 0.
12.  `[0,0,0]`. `finalPrice` will never change value after its assignation on line 3, so `0` will be appended each time `finalPrice` is pushed onto `discounted`.
13. a) `student.name`
    b) `student['Grad Year']`
    c) `student.greeting()`
    d) `student['Favorite Teacher'].name`
    e) `student.courseLoad[0]`
14. a) 32
    b) 1
    c) 3
    d) 3null
    e) 4
    f) 0
    g) 3undefined
    h) 3undefined
15. a) true
    b) false
    c) true
    d) false
    e) false
    f) true
16. `==` does not check against typing while `===` does. So `2 == '2'` is true but `2 === '2'` is false.
17. How are you?, since `2 == true` evaluates to false, so the if-block is skipped, but the expression 2 will evaluate to true so the else-if-block is entered.
18. See part1-question18.js
19. `[6,8,10]`. For each element in `array`, we are calling the `callback` function, which in `modifyArray` is the function `doSomething`, and we are passing an anonymous function that multiplies `x` by 2. In `doSomething`, we call that anonymous function, but passing in the number + 2. So, if `array[i] === 1`, then `doSomething` receives 1, then passes 3 into the anonymous function, which returns 6. The same process is followed for the other elements of `array`. 
20. See part1-question20.js
21. 1
    
    4
    
    3
    
    2