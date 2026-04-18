## 📌 Program 65: Calculate Power of a Number Using a Function

### 💻 Code

```c id="p3m8qx"
#include <stdio.h>

// Function to calculate power
long long power(int base, int exponent) {
    long long result = 1;
    int i;

    for (i = 1; i <= exponent; i++) {
        result = result * base;
    }

    return result;
}

int main() {
    int base, exponent;

    printf("Enter base and exponent: ");
    scanf("%d %d", &base, &exponent);

    printf("Result = %lld", power(base, exponent));

    return 0;
}
```

### 📖 Explanation

* `power(base, exponent)` → user-defined function
* Multiplies `base` repeatedly `exponent` times
* Returns final result
* `main()` calls function and prints output

### ▶️ Output

```id="q7m2zn"
Enter base and exponent: 2 5
Result = 32
```

---
