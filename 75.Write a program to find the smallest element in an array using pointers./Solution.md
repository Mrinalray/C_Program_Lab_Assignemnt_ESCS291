## 📌 Program 75: Find the Smallest Element in an Array Using Pointers

### 💻 Code

```c id="s2m8qx"
#include <stdio.h>

// Function to find smallest element using pointers
int findSmallest(int *arr, int n) {
    int i, min = *arr;

    for (i = 1; i < n; i++) {
        if (*(arr + i) < min) {
            min = *(arr + i);
        }
    }

    return min;
}

int main() {
    int arr[100], n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter elements:\n");
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Smallest element = %d", findSmallest(arr, n));

    return 0;
}
```

### 📖 Explanation

* `int *arr` → pointer to array
* `min = *arr` → initialize with first element
* Loop compares each element using pointer arithmetic
* Updates `min` when smaller value found

### ▶️ Output

```id="m4q9zn"
Enter number of elements: 5
Enter elements:
10 25 8 15 30
Smallest element = 8
```

---
