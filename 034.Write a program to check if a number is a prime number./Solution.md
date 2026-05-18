## 📌 Program 34: Check if a Number is a Prime Number

### 💻 Code

```c id="p8m4qx"
#include <stdio.h>

int main() {
    int num, i, flag = 0;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (num <= 1) {
        printf("Not a Prime Number");
        return 0;
    }

    for (i = 2; i <= num / 2; i++) {
        if (num % i == 0) {
            flag = 1;
            break;
        }
    }

    if (flag == 0)
        printf("Prime Number");
    else
        printf("Not a Prime Number");

    return 0;
}
```

### 📖 Explanation

* Prime number → divisible only by 1 and itself
* Loop checks divisibility from `2` to `num ÷ 2`
* If divisible → not prime
* `flag` is used to track condition

### ▶️ Output

```id="v3q9zn"
Enter a number: 7
Prime Number
```

---
