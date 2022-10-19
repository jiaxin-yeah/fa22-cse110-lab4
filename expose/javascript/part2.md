1. It prints `3`. The reason is in the `for loop`, the `i` would start from 0, checked that 0 < `prices.length`. Then  increase to 1, checked that `1 < prices.length`. Then  increase to 2, checked that `2 < prices.length`. Then  increase to 3, checked that `3 = prices.length`. So, the `for` loop stops at `i = 3`.
2. It prints `150`. Since the last `i` that qualifies for the `i < prices.length` is `i = 2`. So, line 13 will print the final value of `discountedPrice` when `i = 2`. In this case, `discountedPrice = prices[2] * (1 - discount) = 300 * (1 - 0.5) = 150`.
3. It prints `150`. As reasoned above, line 14 will print the final value of `finalPrice` when `i = 2`. In this case, `finalPrice = Math.round(discountedPrice * 100) / 100 = Math.round(150 * 100) / 100 = 150`.
4. The function will return the `discounted` list whose value is a list of final prices, i.e. `[100 * 0.5, 200 * 0.5, 300 * 0.5] = [50, 100, 150]`.
5. It prints the ReferenceError. It's when we use `let` to declare `i`, we can only access `i` inside the `for loop`. When we try to print `i` outside the `for loop`, we would get the ReferenceError.
   
/Users/apple/fa22-cse110-lab4/expose/javascript/discountPrices.js:12
    console.log(i);
                ^

ReferenceError: i is not defined
    at discountPrices (/Users/apple/fa22-cse110-lab4/expose/javascript/discountPrices.js:12:17)
    at Object.<anonymous> (/Users/apple/fa22-cse110-lab4/expose/javascript/discountPrices.js:19:1)
    at Module._compile (node:internal/modules/cjs/loader:1155:14)
    at Object.Module._extensions..js (node:internal/modules/cjs/loader:1209:10)
    at Module.load (node:internal/modules/cjs/loader:1033:32)
    at Function.Module._load (node:internal/modules/cjs/loader:868:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:81:12)
    at node:internal/main/run_main_module:22:47

6. It prints the ReferenceError. It's when we use `let` to declare `discountedPrice`, we can only access `discountedPrice` inside the `for loop`. When we try to print `discountedPrice` outside the `for loop`, we would get the ReferenceError.

/Users/apple/fa22-cse110-lab4/expose/javascript/discountPrices.js:13
    console.log(discountedPrice);
                ^

ReferenceError: discountedPrice is not defined
    at discountPrices (/Users/apple/fa22-cse110-lab4/expose/javascript/discountPrices.js:13:17)
    at Object.<anonymous> (/Users/apple/fa22-cse110-lab4/expose/javascript/discountPrices.js:19:1)
    at Module._compile (node:internal/modules/cjs/loader:1155:14)
    at Object.Module._extensions..js (node:internal/modules/cjs/loader:1209:10)
    at Module.load (node:internal/modules/cjs/loader:1033:32)
    at Function.Module._load (node:internal/modules/cjs/loader:868:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:81:12)
    at node:internal/main/run_main_module:22:47

7. It prints `150`. As reasoned in Question 3, the final value of `finalPrice` becomes `150`. And since `finalPrice` is defined with `let` in line 4, not in the `for loop`. So, we can access this `finalPrice` at line 14.
8. The function will return the `discounted` list whose value is a list of final prices, i.e. `[100 * 0.5, 200 * 0.5, 300 * 0.5] = [50, 100, 150]`. `????????????????`
9. It prints the ReferenceError. It's when we use `let` to declare `i`, we can only access `i` inside the `for loop`. When we try to print `i` outside the `for loop`, we would get the ReferenceError.

/Users/apple/fa22-cse110-lab4/expose/javascript/discountPrices.js:11
    console.log(i);
                ^

ReferenceError: i is not defined
    at discountPrices (/Users/apple/fa22-cse110-lab4/expose/javascript/discountPrices.js:11:17)
    at Object.<anonymous> (/Users/apple/fa22-cse110-lab4/expose/javascript/discountPrices.js:17:1)
    at Module._compile (node:internal/modules/cjs/loader:1155:14)
    at Object.Module._extensions..js (node:internal/modules/cjs/loader:1209:10)
    at Module.load (node:internal/modules/cjs/loader:1033:32)
    at Function.Module._load (node:internal/modules/cjs/loader:868:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:81:12)
    at node:internal/main/run_main_module:22:47

10. It prints `3`. It will just print the length of `prices`, which is `3`.
11. The function will return the `discounted` list whose value is a list of final prices, i.e. `[100 * 0.5, 200 * 0.5, 300 * 0.5] = [50, 100, 150]`. `????????????????`
12. 
    - A. `student.name`
    - B. `student["Grad Year"]`
    - C. `student.greeting()`
    - D. `student["Favorite Teacher"].name`
    - E. `student.courseLoad[0]`
13. 
    - A. `'32'`: The string `'3'` is concatenated with the int `2` while converting `2` from int to string to form the string `'32'`.
    - B. `1`: The string `'3'` is converted to int `3` since JavaScript can't perform substraction on strings, and `3 - 2 = 1`.
    - C. `3`: JavaScript treats `null` as `0` while adding it to an int, so `3 + 0 = 3`.
    - D. `'3null'`: JavaScript treats `null` as a string while adding it to a string, so these two strings concatenated together to form `'3null'`.
    - E. `4`: JavaScript treats `true` as an int equal to `1` while adding it to an int, so `1 + 3 = 4`.
    - F. hi
    - G. hi
    - H. hi