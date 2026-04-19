## 📌 Program 100: Demonstrate the Use of `#pragma`

### 💻 Code

```c id="p9m8qx"
#include <stdio.h>

// Disable specific warning (example for some compilers)
#pragma GCC diagnostic ignored "-Wunused-variable"

int main() {
    int unusedVar;  // This won't trigger a warning due to pragma

    printf("Demonstrating #pragma directive\n");

    return 0;
}
```

### 📖 Explanation

* `#pragma` → special instruction to the compiler
* Used for:

  * Controlling warnings
  * Optimizations
  * Compiler-specific features
* `#pragma GCC diagnostic ignored` → disables specific warning (GCC compiler)
* Behavior may vary depending on compiler

### ▶️ Output

```id="m8q2zn"
Demonstrating #pragma directive
```

---
