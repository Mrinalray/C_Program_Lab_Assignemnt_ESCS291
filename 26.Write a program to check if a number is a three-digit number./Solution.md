## 📌 Program 26: Check if a Number is a Three-Digit Number

### 💻 Code

```c id="g7m2qx"
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if ((num >= 100 && num <= 999) || (num <= -100 && num >= -999))
        printf("It is a three-digit number");
    else
        printf("It is not a three-digit number");

    return 0;
}
```

### 📖 Explanation

* `int num;` → variable to store number
* `scanf()` → takes input
* `100 to 999` → positive three-digit numbers
* `-100 to -999` → negative three-digit numbers
* `||` → checks both positive and negative cases

### ▶️ Output

```id="q3m8zn"
Enter a number: 256
It is a three-digit number
```

---
