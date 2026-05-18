## Program 108: Find the Second Smallest Element in an Array

💻 Code

```c id="h3v9qp"
#include <stdio.h>

int main() {

    int arr[5], i;
    int smallest, secondSmallest;

    // Input array elements
    printf("Enter 5 elements:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &arr[i]);
    }

    // Assume first two elements
    if(arr[0] < arr[1]) {
        smallest = arr[0];
        secondSmallest = arr[1];
    }
    else {
        smallest = arr[1];
        secondSmallest = arr[0];
    }

    // Find smallest and second smallest
    for(i = 2; i < 5; i++) {

        if(arr[i] < smallest) {
            secondSmallest = smallest;
            smallest = arr[i];
        }
        else if(arr[i] < secondSmallest && arr[i] != smallest) {
            secondSmallest = arr[i];
        }
    }

    // Display result
    printf("Second smallest element = %d\n", secondSmallest);

    return 0;
}
```

📖 Explanation

* The program stores array elements using a loop
* Two variables `smallest` and `secondSmallest` are used
* Initially, first two elements are compared and assigned
* Remaining elements are checked one by one
* If a smaller element is found, values are updated accordingly
* Finally, the second smallest element is displayed

▶️ Output

```text id="d8k4mz"
Enter 5 elements:
12
45
7
34
20

Second smallest element = 12
```
