## 📌 Program 92: Demonstrate the Use of `static` Keyword

### 💻 Code

```c id="s8m3qx"
#include <stdio.h>

// Function to demonstrate static variable
void counter() {
    static int count = 0;  // retains value between calls
    count++;
    printf("Count = %d\n", count);
}

int main() {
    counter();
    counter();
    counter();

    return 0;
}
```

### 📖 Explanation

* `static int count = 0;` → initialized only once
* Value is **retained between function calls**
* Each call increases the same variable
* Unlike normal variables, it does not reset

### ▶️ Output

```id="p3m9zn"
Count = 1
Count = 2
Count = 3
```

---
