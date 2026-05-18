## Program 107: Find the Second Largest Element in an Array

💻 Code

```c id="q7m2vx"
#include <stdio.h>

int main() {

    int arr[5], i;
    int largest, secondLargest;

    // Input array elements
    printf("Enter 5 elements:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &arr[i]);
    }

    // Assume first two elements
    if(arr[0] > arr[1]) {
        largest = arr[0];
        secondLargest = arr[1];
    }
    else {
        largest = arr[1];
        secondLargest = arr[0];
    }

    // Find largest and second largest
    for(i = 2; i < 5; i++) {

        if(arr[i] > largest) {
            secondLargest = largest;
            largest = arr[i];
        }
        else if(arr[i] > secondLargest && arr[i] != largest) {
            secondLargest = arr[i];
        }
    }

    // Display result
    printf("Second largest element = %d\n", secondLargest);

    return 0;
}
```

📖 Explanation

* The program stores array elements using a loop
* Two variables `largest` and `secondLargest` are used
* Initially, first two elements are compared and assigned
* Remaining elements are checked one by one
* If a bigger element is found, values are updated accordingly
* Finally, the second largest element is displayed

▶️ Output

```text id="w5n8kp"
Enter 5 elements:
12
45
78
34
67

Second largest element = 67
```
