## 📌 Program 80: Find the Factorial of a Number Using Recursion

### 💻 Code

```c id="f5m3qx"
#include <stdio.h>

// Recursive function to calculate factorial
long long factorial(int n) {
    if (n == 0 || n == 1)
        return 1;
    else
        return n * factorial(n - 1);
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

* Base case: `factorial(0) = 1`, `factorial(1) = 1`
* Recursive case: `n × factorial(n-1)`
* Function calls itself until base case is reached

### ▶️ Output

```id="q9m2zn"
Enter a number: 5
Factorial = 120
```

---
