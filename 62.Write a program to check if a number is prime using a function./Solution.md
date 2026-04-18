## 📌 Program 62: Check if a Number is Prime Using a Function

### 💻 Code

```c id="p7m3qx"
#include <stdio.h>

// Function to check prime
int isPrime(int n) {
    int i;

    if (n <= 1)
        return 0;

    for (i = 2; i <= n / 2; i++) {
        if (n % i == 0)
            return 0;
    }

    return 1;
}

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (isPrime(num))
        printf("Prime Number");
    else
        printf("Not a Prime Number");

    return 0;
}
```

### 📖 Explanation

* `isPrime(int n)` → user-defined function
* Returns `1` if prime, `0` otherwise
* Checks divisibility from `2` to `n ÷ 2`
* `main()` calls function and prints result

### ▶️ Output

```id="x4m8zn"
Enter a number: 11
Prime Number
```

---
