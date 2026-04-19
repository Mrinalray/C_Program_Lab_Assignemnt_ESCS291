## 📌 Program 99: Demonstrate the Use of `#if`, `#elif`, and `#else`

### 💻 Code

```c id="p1m8qx"
#include <stdio.h>

// Define a macro value
#define VALUE 10

int main() {

#if VALUE > 10
    printf("VALUE is greater than 10\n");

#elif VALUE == 10
    printf("VALUE is equal to 10\n");

#else
    printf("VALUE is less than 10\n");

#endif

    return 0;
}
```

### 📖 Explanation

* `#if`, `#elif`, `#else` → conditional compilation directives
* Conditions are checked at compile time
* Only one block of code is compiled
* Useful for configuration, debugging, and platform-specific code

### ▶️ Output

```id="m4q2zn"
VALUE is equal to 10
```

---
