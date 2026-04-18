## 📌 Program 19: Find the Largest of Three Numbers

### 💻 Code

```c id="l9m3qx"
#include <stdio.h>

int main() {
    int a, b, c;

    printf("Enter three numbers: ");
    scanf("%d %d %d", &a, &b, &c);

    if (a >= b && a >= c)
        printf("Largest number = %d", a);
    else if (b >= a && b >= c)
        printf("Largest number = %d", b);
    else
        printf("Largest number = %d", c);

    return 0;
}
```

### 📖 Explanation

* `int a, b, c;` → variables for three numbers
* `scanf()` → takes input values
* Conditions compare all three numbers
* Prints the largest value using `printf()`

### ▶️ Output

```id="v4q8zn"
Enter three numbers: 10 25 15
Largest number = 25
```

---
