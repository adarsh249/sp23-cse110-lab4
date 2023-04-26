1. var is intially declared in the for loop as 0. Once the for loop is done running, it will be equal to 3. Since i is declared with a var keyword, you have access to it in the function scope which means it will print `3` to the console.
2. Since `discountedPrice` is declared as a var in the same function scope, we will print its last value. This means after the for loop finishes running. `discountedPrice` will be equal to `prices[2]` * (1 - 0.5) which is 150. Then, `150` will be printed to the console.
3. `finalPrice` was declared with a var keyword and the value was changed in the for loop so we will get the last for loop which is after the loop finishes. Therefore, `finalPrice` will be equal to `Math.round(150 * 100)/100`. The 150 is from #2. Therefore, `150` will be printed to the console.
4. `discounted` was delcared in the same function block with the var keyword. Therefore, we will return its last value, which is after the for loop ends. This means this function will return `[50, 100, 150]`.
5. This will cause an error since `i` was declared using the let keyword and this was declared in a different scope from where line 12 is.
6. This will cause an error since `discountedPrice` was declared using the let keyword in a different scope from where line 13 is.
7. `finalPrice` was declared with the let keyword in the same scope which means it will just print `150` to the console as that is the last value it was assigned once the for loop ended.what 
8. The function will return `[50, 100, 150]`. `discounted` was declared with the let keyword in the same scope and it's value will change in the for loop, so it would just return the last known value.
9. This will cause an error because `i` was declared with the let keyword in a different scope.
10. `3` will be printed to the console since we assign `length` to be `prices.length` which is 3. This `length` cannot chnage because it has the `const` keyword in front of it.
11. This function returns `[50, 100, 150]` because we can still push to an array that is const, so we just take whatever is last from the for loop. We just cannot reassign the const variable to a new array.
12A. student.name
12B. student['Grad Year']
12C. student.greeting()
12D. student['Favorite Teacher'].name
12E. student.courseLoad[0]
13A. `'32'` For string + integer, JS converts integer to string and concatenates.
13B. `1` For string - integer, JS converts the string to an interger and returns an integer.
13C. `3` For integer + null, JS converts null to the integer 0, performs addition, and returns an integer.
13D. `'3null'` For string + null, JS converts null to a string and concatenates.
13E. `4` For true + 3, JS converts true to 1, since true = 1, performs addition, and returns an integer.
13F. `0` For false + null, JS converts false to 0, since false = 0, and null to 0, performs addition, then returns an integer.
13G. `'3undefined'` For string + undefined, JS converts undefined to a string and concatenates.
13H. `Nan`. This is a special value because JS tries to convert 3 to an integer, however, an integer subtracting from undefined is not valid arithmetic, so it produces NaN. 
14A. `True`. This is because JS converts 2 to an integer and compares it with integer 1.
14B. `False`. Comparison of two strings is done as in any other language using ASCII values. Since 2 > 1, this returns false.
14C. `True`. JS converts the string 2 to an integer and then compares if integer 2 and integer 2 are equal.
14D. `False`. JS does not try to convert in this case since we are using 3 equal signs and because both values are of different types, false is returned.
14E. `False`. JS converts true to 1, since true = 1, however, this comparison is obviously false since 1 does not equal 2.
14F. `True`. Since any value not equal to 0 is considered true, then `Boolean(2)` returns true as a boolean, so comparing the types and values in this case is true since both are booleans and both are true.
15. For ==, Javascript compares the values and also tries to convert the types on each side to compare them. For ===, Javascript does not do type conversion, so it will only return true if two values have the same type and value.
17. First we create a new empty array labeled `newArr`. Then we run a for loop from 0 to 3, since `array.length` is 3. In this for loop, we will push to the `newArr` whatever value `callback` returns. We call `callback` on each value of the `array`. `callback` simply doubles the value and returns in, meaning after pushing new values to `newArr`, we will return it and it will return `[2, 4, 6]`.
19. `1`
    `4`
    `3`
    `2`

