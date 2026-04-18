## 📌 Program 31: Check if a Number is a Multiple of 3 and 5

### 💻 Code

```c id="m5q2zx"
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (num % 3 == 0 && num % 5 == 0)
        printf("Number is a multiple of both 3 and 5");
    else
        printf("Number is not a multiple of both 3 and 5");

    return 0;
}
```

### 📖 Explanation

* `int num;` → variable to store number
* `scanf()` → takes input
* `num % 3 == 0` → checks multiple of 3
* `num % 5 == 0` → checks multiple of 5
* `&&` → ensures both conditions are true

### ▶️ Output

```id="q2m9zn"
Enter a number: 30
Number is a multiple of both 3 and 5
```

---
