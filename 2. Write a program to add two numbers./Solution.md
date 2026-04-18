## 📌 Program 2: Add Two Numbers

### 💻 Code

```c
#include <stdio.h>

int main() {
    int a, b, sum;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    sum = a + b;

    printf("Sum = %d", sum);

    return 0;
}
```

### 📖 Explanation

* `int a, b, sum;` → variables to store numbers and result
* `scanf()` → takes input from user
* `sum = a + b;` → performs addition
* `printf()` → displays the result

### ▶️ Output

```
Enter two numbers: 5 7
Sum = 12
```

---
