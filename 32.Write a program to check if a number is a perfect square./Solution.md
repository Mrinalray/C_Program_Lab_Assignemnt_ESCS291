## 📌 Program 32: Check if a Number is a Perfect Square

### 💻 Code

```c id="p4m8qx"
#include <stdio.h>
#include <math.h>

int main() {
    int num;
    float root;

    printf("Enter a number: ");
    scanf("%d", &num);

    root = sqrt(num);

    if (root == (int)root)
        printf("It is a perfect square");
    else
        printf("It is not a perfect square");

    return 0;
}
```

### 📖 Explanation

* `sqrt()` → finds square root (from `math.h`)
* If square root is an integer → perfect square
* `(int)root` → converts to integer for comparison

### ▶️ Output

```id="x5q3zn"
Enter a number: 25
It is a perfect square
```

---
