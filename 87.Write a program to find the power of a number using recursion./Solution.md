## 📌 Program 87: Find the Power of a Number Using Recursion

### 💻 Code

```c id="p7m3qx"
#include <stdio.h>

// Recursive function to calculate power
long long power(int base, int exponent) {
    if (exponent == 0)
        return 1;
    else
        return base * power(base, exponent - 1);
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

* Base case: `exponent = 0` → return `1`
* Recursive case: `base × power(base, exponent-1)`
* Function calls itself until exponent becomes 0

### ▶️ Output

```id="q6m2zn"
Enter base and exponent: 2 4
Result = 16
```

---
