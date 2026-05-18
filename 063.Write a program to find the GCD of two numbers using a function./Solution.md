## 📌 Program 63: Find GCD of Two Numbers Using a Function

### 💻 Code

```c id="g4m9qx"
#include <stdio.h>

// Function to find GCD using Euclidean algorithm
int gcd(int a, int b) {
    while (b != 0) {
        int temp = b;
        b = a % b;
        a = temp;
    }
    return a;
}

int main() {
    int num1, num2;

    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);

    printf("GCD = %d", gcd(num1, num2));

    return 0;
}
```

### 📖 Explanation

* `gcd(a, b)` → user-defined function
* Uses **Euclidean algorithm**
* Replaces `(a, b)` → `(b, a % b)` repeatedly
* Stops when `b = 0` → `a` is GCD

### ▶️ Output

```id="z7m2qn"
Enter two numbers: 48 18
GCD = 6
```

---
