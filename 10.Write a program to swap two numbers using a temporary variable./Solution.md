## 📌 Program 10: Swap Two Numbers Using a Temporary Variable

### 💻 Code

```c id="t8m4qz"
#include <stdio.h>

int main() {
    int a, b, temp;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    temp = a;
    a = b;
    b = temp;

    printf("After swapping: a = %d, b = %d", a, b);

    return 0;
}
```

### 📖 Explanation

* `int a, b, temp;` → variables for numbers and temporary storage
* `temp = a;` → store value of `a`
* `a = b;` → assign `b` to `a`
* `b = temp;` → assign stored value to `b`
* `printf()` → displays swapped values

### ▶️ Output

```id="p7x2kd"
Enter two numbers: 5 10
After swapping: a = 10, b = 5
```

---
