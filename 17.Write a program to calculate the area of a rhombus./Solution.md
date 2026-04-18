## 📌 Program 17: Calculate Area of a Rhombus

### 💻 Code

```c id="r3m8qx"
#include <stdio.h>

int main() {
    float d1, d2, area;

    printf("Enter diagonals of rhombus: ");
    scanf("%f %f", &d1, &d2);

    area = 0.5 * d1 * d2;

    printf("Area of rhombus = %.2f", area);

    return 0;
}
```

### 📖 Explanation

* `float d1, d2, area;` → diagonals and result
* `scanf()` → takes input values
* `area = ½ × d1 × d2` → rhombus area formula
* `printf()` → displays result

### ▶️ Output

```id="u8q2zn"
Enter diagonals of rhombus: 6 8
Area of rhombus = 24.00
```

---
