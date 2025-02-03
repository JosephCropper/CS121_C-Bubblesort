# CS121_C-Bubblesort
using c to do a basic bubble sort

Algorithm:
----------------------------------------------------------------
```
Main:
The main function is the main function that runs the main part of the code when the code is run.
This particular main function utilizes the creation of three arrays within the c programming language and provides adequate feedback when compiled to show that the program has run properly and done what it has been told to do as computer code is supposed to.
The first array holds the data for the most optimal run (testArrayControl) in which the array is already sorted and sorting the array through the sorting function should not cause issue as there should be no confusion sorting the already sorted array.
The second array holds the dara for a standard set (testArrayStandard) in which the array has been preloaded with arguably random numbers to simulate the program running through any random array, where a partially randomized array makes up 362,878 of the 362,880 possible inputs for the program to sort.
The third array holds the data for the supposed least optimal run (testArrayLor) in which the already sorted array is inputted in the reverse order such that the last number is first and the first number is last, etc, for the entire array.

The main function will used the previously described arrays and one at a time show the entire array, run the stated array through the (later described) sorting function that takes the array and sorts the data in it until sorted, and then prints the final result of the array showing that the sorted array plugged into the sorting system has indeed been sorted.

sortBubble:
Aforementioned as the "sorting function", sortBubble is the sorting function that takes an inputted int array and the size of the array. this sorting function uses the quality of arrays in the C language in which calling an array's individual cell will result in the editing of the data within the array's cell, bypassing the need of direct use for pointers and making the program easier to use and understand with an overall simpler design.
The sorting function starts by creating a temporary integer variable appropriately named "temp".
It then shifts a line down on the console to better organize the output for the user's viewing experience.
A for loop is initialized, creating an integer variable and setting it to zero, the continuation clause being that the loop variable is less than the size of the array, and increments the loop variable once at the end of the loop every loop, making this loop loop the exact amount of times as the size of the array.
The sorting function then calls a "printing function" which will take the array being sorted and print it. This will be further clarified in the printArray section of the algorithm.
Another for loop is initialized, creating an integer variable and setting it equal to zero, the continuation clause being that the loop variable is less than the size of the array subtracted by one, and increments the loop variable once at the end of the loop every loop, making this loop loop one less times than the size of the array.
A simple swapping system is then utilized, checking to see if the value within the cell designated by the nested for loop is greater than the value within the cell designated by the nested for loop incremented by one, or checking to see if the value in the cell of the array designated by the nested for loop is greater than the value following it within the array. If this is false, the swapping system does not activate.
If it is true, then the temporary integer value "temp" is set equal to the value of the cell of the array designated by the nested for loop plus one.
The value of the cell of the array designated by the nested for loop plus one is then set to the value of the cell of the array designated by the for loop. The swap is then completed by setting the value in the cell of the array designated by the nested for loop equal to the value of the temporary integer value "temp", succesfully swapping the two compared values within the array such that the larger value comes second.
the use of another function in this instance would be detrimental to the overall runtime of the program, seeing that pointers are unnecessary due to the property of arrays, and that the data of the two integers locations would have to be transferred to the function, which takes unnecesary time. this also oversimplifies the function of sortBubble, where the most internal logic sequence is tied to a seperate segment of code, taking the program from one primary logical sequence to a hollow looping system.
The sortBubble sorting function is set to end when the for loops have both completed.

printArray:
Aforementioned as the "printing function", printArray is the printing function that takes an integer array and its size as arguements, and will print the values of each individual cell within the array.
A for loop is initialized, creating an integer value set to zero, the continuation clause being that the loop variable is less than the size of the array, and increments the loop variable once at the end of the loop every loop, making this loop loop the exact amount of times as the size of the array.
the C print function is called, printing the value of the cell of the array deterimed by the for loop.
After the for loop is finished, another line is printed, and then the function ends.
```
