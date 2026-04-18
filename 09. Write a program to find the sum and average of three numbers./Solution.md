## 📌 Program 9: Find Sum and Average of Three Numbers

### 💻 Code

```c id="v6p2qx"
#include <stdio.h>

int main() {
    float a, b, c, sum, average;

    printf("Enter three numbers: ");
    scanf("%f %f %f", &a, &b, &c);

    sum = a + b + c;
    average = sum / 3;

    printf("Sum = %.2f\n", sum);
    printf("Average = %.2f", average);

    return 0;
}
```

### 📖 Explanation

* `float a, b, c` → variables for three numbers
* `sum = a + b + c` → calculates total
* `average = sum ÷ 3` → calculates average
* `printf()` → displays results

### ▶️ Output

```id="x3m8zn"
Enter three numbers: 10 20 30
Sum = 60.00
Average = 20.00
```

---
