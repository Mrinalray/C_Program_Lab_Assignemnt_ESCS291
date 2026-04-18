## 📌 Program 41: Print All Even Numbers Between 1 and 100

### 💻 Code

```c id="e8m3qx"
#include <stdio.h>

int main() {
    int i;

    for (i = 2; i <= 100; i += 2) {
        printf("%d ", i);
    }

    return 0;
}
```

### 📖 Explanation

* Loop starts from `2` (first even number)
* Increments by `2` each time
* Prints all even numbers up to `100`

### ▶️ Output

```id="q5m2zn"
2 4 6 8 10 12 14 16 18 20 22 24 26 28 30 32 34 36 38 40 42 44 46 48 50 52 54 56 58 60 62 64 66 68 70 72 74 76 78 80 82 84 86 88 90 92 94 96 98 100
```

---
