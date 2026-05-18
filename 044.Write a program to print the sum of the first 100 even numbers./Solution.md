## 📌 Program 44: Print the Sum of the First 100 Even Numbers

### 💻 Code

```c id="e2m9qx"
#include <stdio.h>

int main() {
    int i, sum = 0;

    for (i = 2; i <= 200; i += 2) {
        sum = sum + i;
    }

    printf("Sum = %d", sum);

    return 0;
}
```

### 📖 Explanation

* First 100 even numbers → `2, 4, 6, ..., 200`
* Loop runs from `2` to `200` with step `2`
* Adds each even number to `sum`

### ▶️ Output

```id="z3q8xn"
Sum = 10100
```

---
