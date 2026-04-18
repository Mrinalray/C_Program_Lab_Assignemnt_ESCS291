## 📌 Program 61: Calculate Factorial of a Number Using a Function

### 💻 Code

```c id="f3m7qx"
#include <stdio.h>

// Function to calculate factorial
long long factorial(int n) {
    long long fact = 1;
    int i;

    for (i = 1; i <= n; i++) {
        fact = fact * i;
    }

    return fact;
}

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    printf("Factorial = %lld", factorial(num));

    return 0;
}
```

### 📖 Explanation

* `factorial(int n)` → user-defined function
* Loop multiplies numbers from `1` to `n`
* Returns result to `main()`
* `main()` calls function and prints output

### ▶️ Output

```id="q8m2zn"
Enter a number: 5
Factorial = 120
```

---
