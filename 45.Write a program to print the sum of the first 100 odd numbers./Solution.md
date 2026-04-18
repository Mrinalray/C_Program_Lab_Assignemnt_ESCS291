## 📌 Program 45: Print the Sum of the First 100 Odd Numbers

### 💻 Code

```c id="o8m3qx"
#include <stdio.h>

int main() {
    int i, sum = 0;

    for (i = 1; i <= 199; i += 2) {
        sum = sum + i;
    }

    printf("Sum = %d", sum);

    return 0;
}
```

### 📖 Explanation

* First 100 odd numbers → `1, 3, 5, ..., 199`
* Loop runs from `1` to `199` with step `2`
* Adds each odd number to `sum`

### ▶️ Output

```id="m5q2zn"
Sum = 10000
```

---
