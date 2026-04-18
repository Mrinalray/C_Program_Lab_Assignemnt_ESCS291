## 📌 Program 81: Find GCD of Two Numbers Using Recursion

### 💻 Code

```c id="g6m3qx"
#include <stdio.h>

// Recursive function to find GCD
int gcd(int a, int b) {
    if (b == 0)
        return a;
    else
        return gcd(b, a % b);
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

* Uses **Euclidean algorithm (recursion)**
* Base case: if `b = 0`, GCD = `a`
* Recursive step: `gcd(b, a % b)`
* Continues until base case is reached

### ▶️ Output

```id="m2q8zn"
Enter two numbers: 48 18
GCD = 6
```

---
