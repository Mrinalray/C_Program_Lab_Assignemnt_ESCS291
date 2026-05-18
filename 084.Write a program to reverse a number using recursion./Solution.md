## 📌 Program 84: Reverse a Number Using Recursion

### 💻 Code

```c id="r5m3qx"
#include <stdio.h>

// Recursive function to reverse number
int reverse(int n, int rev) {
    if (n == 0)
        return rev;
    else
        return reverse(n / 10, rev * 10 + (n % 10));
}

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    printf("Reversed number = %d", reverse(num, 0));

    return 0;
}
```

### 📖 Explanation

* Base case: when `n = 0`, return reversed number
* Recursive step: build reversed number using `rev × 10 + last digit`
* Function keeps calling itself until all digits are processed

### ▶️ Output

```id="p3m8zn"
Enter a number: 1234
Reversed number = 4321
```

---
