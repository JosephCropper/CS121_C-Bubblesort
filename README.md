# CS121_C-Bubblesort
using c to do a basic bubble sort

bubble sort algorithm:
----------------------------------------------------------------
```
int temp;

for (int u = 0; u < ArrSize; u++){

      for (int n = 0; n < size - 1; n++){
      
        	if (array[n] > array[(n+1)]){

           		temp = array[(n+1)];
                        array[(n+1)] = array[n];
                        array[n] = temp;

            }
        }
    }
```
