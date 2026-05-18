## Program 109: Find the Frequency of Each Element in an Array

💻 Code

```c id="v5n2qx"
#include <stdio.h>

int main() {

    int arr[5], freq[5];
    int i, j, count;

    // Input array elements
    printf("Enter 5 elements:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &arr[i]);
        freq[i] = -1;
    }

    // Find frequency of elements
    for(i = 0; i < 5; i++) {

        count = 1;

        for(j = i + 1; j < 5; j++) {

            if(arr[i] == arr[j]) {
                count++;
                freq[j] = 0;
            }
        }

        if(freq[i] != 0) {
            freq[i] = count;
        }
    }

    // Display frequencies
    printf("Frequency of elements:\n");

    for(i = 0; i < 5; i++) {

        if(freq[i] != 0) {
            printf("%d occurs %d times\n", arr[i], freq[i]);
        }
    }

    return 0;
}
```

📖 Explanation

* The program stores array elements using a loop
* Another array `freq[]` is used to store frequencies
* Each element is compared with remaining elements in the array
* If duplicate elements are found, the count increases
* Frequency of every unique element is displayed
* Duplicate occurrences are ignored during printing

▶️ Output

```text id="r8k4mp"
Enter 5 elements:
2
3
2
5
3

Frequency of elements:
2 occurs 2 times
3 occurs 2 times
5 occurs 1 times
```
