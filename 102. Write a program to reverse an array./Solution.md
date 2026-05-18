## Program 102: Reverse an Array

💻 Code

```c id="p8n4xt"
#include <stdio.h>

int main() {

    int arr[5], i, temp;

    // Input array elements
    printf("Enter 5 elements:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &arr[i]);
    }

    // Reverse the array
    for(i = 0; i < 5 / 2; i++) {
        temp = arr[i];
        arr[i] = arr[5 - i - 1];
        arr[5 - i - 1] = temp;
    }

    // Display reversed array
    printf("Reversed array:\n");
    for(i = 0; i < 5; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}
```

📖 Explanation

* Array elements are stored using a loop
* First element is swapped with the last element
* Second element is swapped with the second last element
* Swapping continues until the middle of the array
* Finally, the reversed array is displayed

▶️ Output

```text id="1u8q7m"
Enter 5 elements:
1
2
3
4
5

Reversed array:
5 4 3 2 1
```
