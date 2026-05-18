## 📌 Program 76: Find the Sum of Elements in an Array Using Pointers

### 💻 Code

```c id="s7m3qx"
#include <stdio.h>

// Function to calculate sum using pointers
int sumArray(int *arr, int n) {
    int i, sum = 0;

    for (i = 0; i < n; i++) {
        sum += *(arr + i);
    }

    return sum;
}

int main() {
    int arr[100], n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter elements:\n");
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Sum of elements = %d", sumArray(arr, n));

    return 0;
}
```

### 📖 Explanation

* `int *arr` → pointer to array
* Loop accesses elements using `*(arr + i)`
* Adds each element to `sum`
* Returns final result

### ▶️ Output

```id="p2m9zn"
Enter number of elements: 5
Enter elements:
1 2 3 4 5
Sum of elements = 15
```

---
