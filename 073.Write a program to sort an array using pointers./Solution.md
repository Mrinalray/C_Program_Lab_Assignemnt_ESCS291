## 📌 Program 73: Sort an Array Using Pointers

### 💻 Code

```c id="s3m8qx"
#include <stdio.h>

// Function to sort array using pointers (Bubble Sort)
void sortArray(int *arr, int n) {
    int i, j, temp;

    for (i = 0; i < n - 1; i++) {
        for (j = 0; j < n - i - 1; j++) {
            if (*(arr + j) > *(arr + j + 1)) {
                temp = *(arr + j);
                *(arr + j) = *(arr + j + 1);
                *(arr + j + 1) = temp;
            }
        }
    }
}

int main() {
    int arr[100], n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter elements:\n");
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    sortArray(arr, n);

    printf("Sorted array:\n");
    for (i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}
```

### 📖 Explanation

* `int *arr` → pointer to array
* Uses **pointer arithmetic** (`*(arr + j)`)
* Implements Bubble Sort
* Swaps elements using pointers

### ▶️ Output

```id="x4m2zn"
Enter number of elements: 5
Enter elements:
5 2 4 1 3
Sorted array:
1 2 3 4 5
```

---
