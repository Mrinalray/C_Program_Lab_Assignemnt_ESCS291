## 📌 Program 91: Demonstrate the Use of `volatile` Keyword

### 💻 Code

```c id="v3m8qx"
#include <stdio.h>

int main() {
    volatile int x = 10;

    printf("Initial value of x = %d\n", x);

    x = 20;  // Value changed

    printf("Updated value of x = %d\n", x);

    return 0;
}
```

### 📖 Explanation

* `volatile` tells the compiler that the variable’s value **may change at any time**
* Prevents compiler optimizations that assume value remains constant
* Useful in:

  * Hardware registers
  * Interrupt service routines
  * Multithreading

### ▶️ Output

```id="p5m2zn"
Initial value of x = 10
Updated value of x = 20
```

---
