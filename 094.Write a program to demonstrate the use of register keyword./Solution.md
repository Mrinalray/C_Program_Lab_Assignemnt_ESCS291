## 📌 Program 94: Demonstrate the Use of `register` Keyword

### 💻 Code

```c id="r6m3qx"
#include <stdio.h>

int main() {
    register int i;

    for (i = 1; i <= 5; i++) {
        printf("Value of i = %d\n", i);
    }

    return 0;
}
```

### 📖 Explanation

* `register int i;` → suggests storing variable in CPU register
* Faster access compared to normal variables
* Cannot use `&i` (address operator) with register variables
* Mostly used for loop counters

### ▶️ Output

```id="p2m8zn"
Value of i = 1
Value of i = 2
Value of i = 3
Value of i = 4
Value of i = 5
```

---
