## 📌 Program 43: Print the Sum of the First 100 Natural Numbers

### 💻 Code

```c id="s9m4qx"
#include <stdio.h>

int main() {
    int i, sum = 0;

    for (i = 1; i <= 100; i++) {
        sum = sum + i;
    }

    printf("Sum = %d", sum);

    return 0;
}
```

### 📖 Explanation

* Loop runs from `1` to `100`
* Each number is added to `sum`
* Final result is printed

### ▶️ Output

```id="x7q2zn"
Sum = 5050
```

---
