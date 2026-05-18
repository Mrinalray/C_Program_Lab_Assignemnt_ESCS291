## Program 103: Find the Sum of Elements in an Array

💻 Code

```c id="n4v8kp"
#include <stdio.h>

int main() {

    int arr[5], i, sum = 0;

    // Input array elements
    printf("Enter 5 elements:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &arr[i]);
    }

    // Calculate sum of elements
    for(i = 0; i < 5; i++) {
        sum = sum + arr[i];
    }

    // Display result
    printf("Sum of array elements = %d\n", sum);

    return 0;
}
```

📖 Explanation

* Array elements are stored using a loop
* Variable `sum` is initialized to `0`
* Each array element is added to `sum` using a loop
* After all additions, the total sum is displayed
* Useful for basic array operations and calculations

▶️ Output

```text id="t6x2mz"
Enter 5 elements:
10
20
30
40
50

Sum of array elements = 150
```
