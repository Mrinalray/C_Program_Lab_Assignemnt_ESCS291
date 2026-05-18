## 📌 Program 33: Check if a Number is a Perfect Cube

### 💻 Code

```c id="c3m8qx"
#include <stdio.h>
#include <math.h>

int main() {
    int num;
    float root;

    printf("Enter a number: ");
    scanf("%d", &num);

    root = cbrt(num);

    if (root == (int)root)
        printf("It is a perfect cube");
    else
        printf("It is not a perfect cube");

    return 0;
}
```

### 📖 Explanation

* `cbrt()` → finds cube root (from `math.h`)
* If cube root is an integer → perfect cube
* `(int)root` → converts to integer for comparison

### ▶️ Output

```id="m7q2zn"
Enter a number: 27
It is a perfect cube
```

---
