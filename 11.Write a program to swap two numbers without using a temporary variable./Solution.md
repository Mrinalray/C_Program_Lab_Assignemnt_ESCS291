## 📌 Program 11: Swap Two Numbers Without Using a Temporary Variable

### 💻 Code

```c id="r5m8qk"
#include <stdio.h>

int main() {
    int a, b;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    a = a + b;
    b = a - b;
    a = a - b;

    printf("After swapping: a = %d, b = %d", a, b);

    return 0;
}
```

### 📖 Explanation

* `int a, b;` → variables to store numbers
* `a = a + b;` → sum stored in `a`
* `b = a - b;` → original value of `a` assigned to `b`
* `a = a - b;` → original value of `b` assigned to `a`
* `printf()` → displays swapped values

### ▶️ Output

```id="k9v3mz"
Enter two numbers: 8 3
After swapping: a = 3, b = 8
```

---
