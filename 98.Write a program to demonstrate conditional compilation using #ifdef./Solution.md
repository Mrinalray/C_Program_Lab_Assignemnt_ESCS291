## 📌 Program 98: Demonstrate Conditional Compilation Using `#ifdef`

### 💻 Code

```c id="c9m3qx"
#include <stdio.h>

// Define a macro
#define DEBUG

int main() {

#ifdef DEBUG
    printf("Debug mode is ON\n");
#endif

#ifndef DEBUG
    printf("Debug mode is OFF\n");
#endif

    return 0;
}
```

### 📖 Explanation

* `#define DEBUG` → defines a macro
* `#ifdef DEBUG` → code runs only if `DEBUG` is defined
* `#ifndef DEBUG` → runs if `DEBUG` is NOT defined
* Used for debugging, testing, or platform-specific code

### ▶️ Output

```id="m2q8zn"
Debug mode is ON
```

---
