## 📌 Program 25: Check if a Number is a Two-Digit Number

### 💻 Code

```c id="f3m9qx"
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if ((num >= 10 && num <= 99) || (num <= -10 && num >= -99))
        printf("It is a two-digit number");
    else
        printf("It is not a two-digit number");

    return 0;
}
```

### 📖 Explanation

* `int num;` → variable to store number
* `scanf()` → takes input
* `10 to 99` → positive two-digit numbers
* `-10 to -99` → negative two-digit numbers
* `||` → checks both positive and negative cases

### ▶️ Output

```id="x8q2zn"
Enter a number: 45
It is a two-digit number
```

---
