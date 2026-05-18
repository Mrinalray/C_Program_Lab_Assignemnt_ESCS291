## 📌 Program 39: Find the Factorial of a Number

### 💻 Code

```c id="f6m3qx"
#include <stdio.h>

int main() {
    int num, i;
    long long factorial = 1;

    printf("Enter a number: ");
    scanf("%d", &num);

    for (i = 1; i <= num; i++) {
        factorial = factorial * i;
    }

    printf("Factorial = %lld", factorial);

    return 0;
}
```

### 📖 Explanation

* `long long factorial` → stores large result
* Loop multiplies numbers from `1` to `num`
* Factorial = `n × (n-1) × ... × 1`

### ▶️ Output

```id="p3q8zn"
Enter a number: 5
Factorial = 120
```

---
