## Program 101: Find the Largest Element in an Array

💻 Code

```c
#include <stdio.h>

int main() {

    int arr[5], i, largest;

    // Input array elements
    printf("Enter 5 elements:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &arr[i]);
    }

    // Assume first element is largest
    largest = arr[0];

    // Find largest element
    for(i = 1; i < 5; i++) {
        if(arr[i] > largest) {
            largest = arr[i];
        }
    }

    // Display result
    printf("Largest element = %d\n", largest);

    return 0;
}
```

📖 Explanation

* An array is used to store multiple numbers
* First element is assumed as the largest initially
* Loop compares each element with the current largest value
* If a bigger element is found, it becomes the new largest
* Finally, the largest element is displayed

▶️ Output

```text
Enter 5 elements:
12
45
7
89
23

Largest element = 89
```
