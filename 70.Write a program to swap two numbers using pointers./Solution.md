## 📌 Program 70: Swap Two Numbers Using Pointers

### 💻 Code

```c id="p6m3qx"
#include <stdio.h>

// Function to swap using pointers
void swap(int *a, int *b) {
    int temp;

    temp = *a;
    *a = *b;
    *b = temp;
}

int main() {
    int x, y;

    printf("Enter two numbers: ");
    scanf("%d %d", &x, &y);

    swap(&x, &y);

    printf("After swapping: x = %d, y = %d", x, y);

    return 0;
}
```

### 📖 Explanation

* `swap(int *a, int *b)` → pointer parameters
* `*a`, `*b` → access actual values (dereferencing)
* Swaps values using temporary variable
* `swap(&x, &y)` → passes addresses
* Changes reflect in original variables

### ▶️ Output

```id="m4q8zn"
Enter two numbers: 5 10
After swapping: x = 10, y = 5
```

---
