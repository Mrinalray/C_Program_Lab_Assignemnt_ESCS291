## Program 104: Sort an Array Using Bubble Sort

💻 Code

```c id="m7q2vx"
#include <stdio.h>

int main() {

    int arr[5], i, j, temp;

    // Input array elements
    printf("Enter 5 elements:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &arr[i]);
    }

    // Bubble sort
    for(i = 0; i < 5 - 1; i++) {
        for(j = 0; j < 5 - i - 1; j++) {

            if(arr[j] > arr[j + 1]) {

                // Swap elements
                temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }

    // Display sorted array
    printf("Sorted array:\n");
    for(i = 0; i < 5; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}
```

📖 Explanation

* Bubble sort repeatedly compares adjacent elements
* If the current element is greater than the next element, they are swapped
* After each pass, the largest element moves to its correct position
* The process continues until the array becomes sorted
* This program sorts the array in ascending order

▶️ Output

```text id="g5r1kn"
Enter 5 elements:
64
34
25
12
22

Sorted array:
12 22 25 34 64
```
