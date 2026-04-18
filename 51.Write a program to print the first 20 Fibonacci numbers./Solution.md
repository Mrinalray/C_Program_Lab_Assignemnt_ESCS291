## 📌 Program 51: Print the First 20 Fibonacci Numbers

### 💻 Code

```c id="f7m3qx"
#include <stdio.h>

int main() {
    int a = 0, b = 1, next, i;

    printf("First 20 Fibonacci numbers:\n");

    for (i = 1; i <= 20; i++) {
        printf("%d ", a);
        next = a + b;
        a = b;
        b = next;
    }

    return 0;
}
```

### 📖 Explanation

* Starts with `0` and `1`
* Each next term = sum of previous two
* Loop runs 20 times to print first 20 numbers

### ▶️ Output

```id="x2m8zn"
First 20 Fibonacci numbers:
0 1 1 2 3 5 8 13 21 34 55 89 144 233 377 610 987 1597 2584 4181
```

---
