### Part 1: Intro to JavaScript
1. We will get an error. That is because the variable ```i``` only exists inside the for loop's curly braces. Since line 11 is outside the for loop's curly braces, it cannot access ```i``` from there. 
2. The value inside the ```discountedPrice``` variable i.e. the price of the final item after discount, will be printed without any errors. That is because though the ```discountedPrice``` variable was declared inside the for-loop similar to ```i```, it was declared with the ```var``` keyword, thus it acts like a global veriable and can be accessed from any scope. 
3. The value inside the ```finalPrice``` variable i.e. the rounded price of the final item after discount, will be printed without any errors.  That is because the ```finalPrice``` variable was declared in the same scope as line 13 i.e. scope of the function ```discountPrices```.    
4. 
