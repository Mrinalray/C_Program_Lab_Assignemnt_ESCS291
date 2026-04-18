## 📌 Program 93: Demonstrate the Use of `extern` Keyword

### 💻 Code

```c id="e5m3qx"
#include <stdio.h>

int x = 10;  // Global variable

void display();

int main() {
    printf("Value of x in main = %d\n", x);
    display();
    return 0;
}

// Using extern to access global variable
void display() {
    extern int x;
    printf("Value of x in display = %d\n", x);
}
```

### 📖 Explanation

* `int x = 10;` → global variable
* `extern int x;` → declares that `x` is defined elsewhere
* Allows access to global variables across functions/files
* No new memory is allocated using `extern`

### ▶️ Output

```id="q7m2zn"
Value of x in main = 10
Value of x in display = 10
```

---
