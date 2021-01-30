### Part 3: Debugging using the DevTools
 - The bug lies in the fact that the parameters ```num1``` and ```num2``` passed in the function 
 ```calculateSum``` are of data type string. We know this from the fact that in the Watch expressions tab, 
 the value of ```num1``` is not ```3``` but rather it is ```"3"```. If we compare it with the sample number 
 ```98``` and the sample string ```"string"``` provided, we can see that the datatype of ```num1``` is string 
 because of the ```" "``` around the number. The same can be said about ```num2``` as well because of the 
 ```" "``` around the ```4```. Thus when we define ```result = num1 + num2```, our code doesn't add the 
 numbers. Rather it treats them as string and concatenates them. That is why in our case, when 
 ```num1 = "3"``` and ```num2 = "4"``` instead of getting ```7```, we get ```"34"```.
 - We can fix this bug by explicitly converting ```num1``` and ```num2``` in ```calculateSum``` to integers before adding them.
