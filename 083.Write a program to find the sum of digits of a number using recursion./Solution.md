## 📌 Program 83: Find the Sum of Digits of a Number Using Recursion

### 💻 Code

```c id="s9m3qx"
#include <stdio.h>

// Recursive function to find sum of digits
int sumDigits(int n) {
    if (n == 0)
        return 0;
    else
        return (n % 10) + sumDigits(n / 10);
}

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    printf("Sum of digits = %d", sumDigits(num));

    return 0;
}
```

### 📖 Explanation

* Base case: if `n = 0`, return `0`
* Recursive case: last digit + sum of remaining digits
* Uses `% 10` and `/ 10` for digit extraction
* Function keeps calling itself until number becomes 0

### ▶️ Output

```id="m4q8zn"
Enter a number: 1234
Sum of digits = 10
```

---
