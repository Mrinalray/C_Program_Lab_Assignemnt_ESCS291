## 📌 Program 21: Check if a Number is Positive, Negative, or Zero

### 💻 Code

```c id="n6m2qx"
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (num > 0)
        printf("Positive Number");
    else if (num < 0)
        printf("Negative Number");
    else
        printf("Zero");

    return 0;
}
```

### 📖 Explanation

* `int num;` → variable to store number
* `scanf()` → takes input
* `num > 0` → checks positive
* `num < 0` → checks negative
* Else → number is zero

### ▶️ Output

```id="k3q9zn"
Enter a number: -5
Negative Number
```

---
