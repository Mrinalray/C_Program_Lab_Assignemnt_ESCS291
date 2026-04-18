## 📌 Program 48: Find the Sum of Digits of a Number

### 💻 Code

```c id="d4m8qx"
#include <stdio.h>

int main() {
    int num, sum = 0, remainder;

    printf("Enter a number: ");
    scanf("%d", &num);

    while (num != 0) {
        remainder = num % 10;
        sum = sum + remainder;
        num = num / 10;
    }

    printf("Sum of digits = %d", sum);

    return 0;
}
```

### 📖 Explanation

* Extract each digit using `num % 10`
* Add digit to `sum`
* Remove last digit using `num ÷ 10`
* Repeat until number becomes 0

### ▶️ Output

```id="z8q3xn"
Enter a number: 1234
Sum of digits = 10
```

---
