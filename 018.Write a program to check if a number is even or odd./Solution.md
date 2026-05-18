## 📌 Program 18: Check if a Number is Even or Odd

### 💻 Code

```c id="e4m9qx"
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (num % 2 == 0)
        printf("The number is Even");
    else
        printf("The number is Odd");

    return 0;
}
```

### 📖 Explanation

* `int num;` → variable to store number
* `scanf()` → takes input
* `num % 2 == 0` → checks divisibility by 2
* If true → Even, else → Odd

### ▶️ Output

```id="p3q7zn"
Enter a number: 7
The number is Odd
```

---
