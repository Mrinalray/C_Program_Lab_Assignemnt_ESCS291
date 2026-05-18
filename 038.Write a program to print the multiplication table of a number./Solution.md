## 📌 Program 38: Print the Multiplication Table of a Number

### 💻 Code

```c id="m2n8qx"
#include <stdio.h>

int main() {
    int num, i;

    printf("Enter a number: ");
    scanf("%d", &num);

    for (i = 1; i <= 10; i++) {
        printf("%d x %d = %d\n", num, i, num * i);
    }

    return 0;
}
```

### 📖 Explanation

* `int num, i;` → variables for number and loop
* `scanf()` → takes input
* Loop runs from 1 to 10
* Prints multiplication table using `printf()`

### ▶️ Output

```id="x6q3zn"
Enter a number: 5
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50
```

---
