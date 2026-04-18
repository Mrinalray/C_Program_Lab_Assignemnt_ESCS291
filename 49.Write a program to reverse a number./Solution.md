## 📌 Program 49: Reverse a Number

### 💻 Code

```c id="r8m3qx"
#include <stdio.h>

int main() {
    int num, reversed = 0, remainder;

    printf("Enter a number: ");
    scanf("%d", &num);

    while (num != 0) {
        remainder = num % 10;
        reversed = reversed * 10 + remainder;
        num = num / 10;
    }

    printf("Reversed number = %d", reversed);

    return 0;
}
```

### 📖 Explanation

* Extract last digit using `num % 10`
* Build reversed number → `reversed × 10 + digit`
* Remove last digit using `num ÷ 10`
* Repeat until number becomes 0

### ▶️ Output

```id="q6m2zn"
Enter a number: 1234
Reversed number = 4321
```

---
