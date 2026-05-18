## 📌 Program 24: Check if a Number is Divisible by 5 and 11

### 💻 Code

```c id="d5m8qx"
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (num % 5 == 0 && num % 11 == 0)
        printf("Number is divisible by both 5 and 11");
    else
        printf("Number is not divisible by both 5 and 11");

    return 0;
}
```

### 📖 Explanation

* `int num;` → variable to store number
* `scanf()` → takes input
* `num % 5 == 0` → checks divisibility by 5
* `num % 11 == 0` → checks divisibility by 11
* `&&` → ensures both conditions are true

### ▶️ Output

```id="z2q7zn"
Enter a number: 55
Number is divisible by both 5 and 11
```

---
