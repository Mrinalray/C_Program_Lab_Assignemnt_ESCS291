## 📌 Program 13: Calculate Compound Interest

### 💻 Code

```c id="p9v3mx"
#include <stdio.h>
#include <math.h>

int main() {
    float principal, rate, time, amount, compound_interest;

    printf("Enter principal, rate, and time: ");
    scanf("%f %f %f", &principal, &rate, &time);

    amount = principal * pow((1 + rate / 100), time);
    compound_interest = amount - principal;

    printf("Compound Interest = %.2f", compound_interest);

    return 0;
}
```

### 📖 Explanation

* `float principal, rate, time` → input values
* `pow()` → used for power calculation (from `math.h`)
* `amount = P × (1 + R/100)^T` → compound amount formula
* `compound_interest = amount - principal` → final interest
* `printf()` → displays result

### ▶️ Output

```id="q4z8kx"
Enter principal, rate, and time: 1000 5 2
Compound Interest = 102.50
```

---
