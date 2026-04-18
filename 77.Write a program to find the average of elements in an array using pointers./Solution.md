## 📌 Program 77: Find the Average of Elements in an Array Using Pointers

### 💻 Code

```c id="a2m8qx"
#include <stdio.h>

// Function to calculate average using pointers
float averageArray(int *arr, int n) {
    int i, sum = 0;

    for (i = 0; i < n; i++) {
        sum += *(arr + i);
    }

    return (float)sum / n;
}

int main() {
    int arr[100], n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter elements:\n");
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Average = %.2f", averageArray(arr, n));

    return 0;
}
```

### 📖 Explanation

* `int *arr` → pointer to array
* Loop sums elements using pointer arithmetic
* Cast to `(float)` for correct division
* Returns average value

### ▶️ Output

```id="q6m3zn"
Enter number of elements: 5
Enter elements:
1 2 3 4 5
Average = 3.00
```

---
