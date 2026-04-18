## 📌 Program 74: Find the Largest Element in an Array Using Pointers

### 💻 Code

```c id="l5m3qx"
#include <stdio.h>

// Function to find largest element using pointers
int findLargest(int *arr, int n) {
    int i, max = *arr;

    for (i = 1; i < n; i++) {
        if (*(arr + i) > max) {
            max = *(arr + i);
        }
    }

    return max;
}

int main() {
    int arr[100], n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter elements:\n");
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Largest element = %d", findLargest(arr, n));

    return 0;
}
```

### 📖 Explanation

* `int *arr` → pointer to array
* `max = *arr` → initialize with first element
* Loop compares each element using pointer arithmetic
* Updates `max` when larger value found

### ▶️ Output

```id="p3m8zn"
Enter number of elements: 5
Enter elements:
10 25 8 15 30
Largest element = 30
```

---
