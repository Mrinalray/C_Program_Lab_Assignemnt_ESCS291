## Program 110: Merge Two Arrays

💻 Code

```c id="y6p3vk"
#include <stdio.h>

int main() {

    int arr1[5], arr2[5], merged[10];
    int i;

    // Input first array
    printf("Enter 5 elements for first array:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &arr1[i]);
    }

    // Input second array
    printf("Enter 5 elements for second array:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &arr2[i]);
    }

    // Copy first array into merged array
    for(i = 0; i < 5; i++) {
        merged[i] = arr1[i];
    }

    // Copy second array into merged array
    for(i = 0; i < 5; i++) {
        merged[i + 5] = arr2[i];
    }

    // Display merged array
    printf("Merged array:\n");

    for(i = 0; i < 10; i++) {
        printf("%d ", merged[i]);
    }

    return 0;
}
```

📖 Explanation

* Two arrays `arr1` and `arr2` are used to store elements
* A third array `merged` stores elements of both arrays
* First array elements are copied into the merged array
* Then second array elements are added after the first array elements
* Finally, the merged array is displayed

▶️ Output

```text id="c4m8zr"
Enter 5 elements for first array:
1
2
3
4
5

Enter 5 elements for second array:
6
7
8
9
10

Merged array:
1 2 3 4 5 6 7 8 9 10
```
