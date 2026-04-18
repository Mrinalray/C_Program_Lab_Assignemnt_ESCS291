## 📌 Program 12: Calculate Simple Interest

### 💻 Code

```c id="m3q9vx"
#include <stdio.h>

int main() {
    float principal, rate, time, interest;

    printf("Enter principal, rate, and time: ");
    scanf("%f %f %f", &principal, &rate, &time);

    interest = (principal * rate * time) / 100;

    printf("Simple Interest = %.2f", interest);

    return 0;
}
```

### 📖 Explanation

* `float principal, rate, time, interest;` → variables for calculation
* `scanf()` → takes input values
* `interest = (P × R × T) ÷ 100` → simple interest formula
* `printf()` → displays result

### ▶️ Output

```id="z8m4qt"
Enter principal, rate, and time: 1000 5 2
Simple Interest = 100.00
```

---
