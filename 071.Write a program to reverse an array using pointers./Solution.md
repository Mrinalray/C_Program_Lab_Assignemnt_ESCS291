## 📌 Program 71: Reverse an Array Using Pointers

### 💻 Code

```c id="a9m3qx"
#include <stdio.h>

// Function to reverse array using pointers
void reverseArray(int *arr, int size) {
    int *start = arr;
    int *end = arr + size - 1;
    int temp;

    while (start < end) {
        temp = *start;
        *start = *end;
        *end = temp;

        start++;
        end--;
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

    reverseArray(arr, n);

    printf("Reversed array:\n");
    for (i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}
```

### 📖 Explanation

* `int *arr` → pointer to array
* `start` → points to first element
* `end` → points to last element
* Swap elements using pointers
* Move pointers inward until they meet

### ▶️ Output

```id="p2m8zn"
Enter number of elements: 5
Enter elements:
1 2 3 4 5
Reversed array:
5 4 3 2 1
```

---
