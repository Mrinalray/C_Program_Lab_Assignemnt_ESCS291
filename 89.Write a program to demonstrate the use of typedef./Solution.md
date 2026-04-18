## 📌 Program 89: Demonstrate the Use of typedef

### 💻 Code

```c id="t5m3qx"
#include <stdio.h>

// Using typedef to create alias
typedef int Integer;

int main() {
    Integer a = 10, b = 20;
    Integer sum;

    sum = a + b;

    printf("Sum = %d", sum);

    return 0;
}
```

### 📖 Explanation

* `typedef int Integer;` → creates a new name for `int`
* `Integer` can now be used instead of `int`
* Improves readability and simplifies complex data types

### ▶️ Output

```id="p8m2zn"
Sum = 30
```

---
