## 📌 Program 40: Print the Fibonacci Series up to a Given Number

### 💻 Code

```c id="f2m9qx"
#include <stdio.h>

int main() {
    int n, a = 0, b = 1, next;

    printf("Enter a number: ");
    scanf("%d", &n);

    printf("Fibonacci series: ");

    while (a <= n) {
        printf("%d ", a);
        next = a + b;
        a = b;
        b = next;
    }

    return 0;
}
```

### 📖 Explanation

* Starts with `0` and `1`
* Each next term = sum of previous two
* Loop continues until value exceeds given number

### ▶️ Output

```id="z4q3zn"
Enter a number: 20
Fibonacci series: 0 1 1 2 3 5 8 13
```

---
