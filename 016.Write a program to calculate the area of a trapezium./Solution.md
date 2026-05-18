## 📌 Program 16: Calculate Area of a Trapezium

### 💻 Code

```c id="t4m9qx"
#include <stdio.h>

int main() {
    float a, b, height, area;

    printf("Enter lengths of two parallel sides and height: ");
    scanf("%f %f %f", &a, &b, &height);

    area = 0.5 * (a + b) * height;

    printf("Area of trapezium = %.2f", area);

    return 0;
}
```

### 📖 Explanation

* `float a, b, height, area;` → variables for sides and height
* `scanf()` → takes input values
* `area = ½ × (a + b) × height` → trapezium area formula
* `printf()` → displays result

### ▶️ Output

```id="y8q3zn"
Enter lengths of two parallel sides and height: 6 8 5
Area of trapezium = 35.00
```

---
