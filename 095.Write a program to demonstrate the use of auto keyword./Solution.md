## 📌 Program 95: Demonstrate the Use of `auto` Keyword

### 💻 Code

```c id="a4m8qx"
#include <stdio.h>

int main() {
    auto int x = 10;  // default storage class

    printf("Value of x = %d\n", x);

    {
        auto int x = 20;  // new local variable (block scope)
        printf("Value of x inside block = %d\n", x);
    }

    printf("Value of x outside block = %d\n", x);

    return 0;
}
```

### 📖 Explanation

* `auto` → default storage class for local variables
* Scope is limited to the block where declared
* Inner block creates a new variable with same name
* Outer variable remains unchanged

### ▶️ Output

```id="m3q9zn"
Value of x = 10
Value of x inside block = 20
Value of x outside block = 10
```

---
