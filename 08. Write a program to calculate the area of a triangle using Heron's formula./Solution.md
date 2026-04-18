## 📌 Program 8: Area of a Triangle using Heron's Formula

### 💻 Code

```c id="h4k9zp"
#include <stdio.h>
#include <math.h>

int main() {
    float a, b, c, s, area;

    printf("Enter three sides of triangle: ");
    scanf("%f %f %f", &a, &b, &c);

    s = (a + b + c) / 2;

    area = sqrt(s * (s - a) * (s - b) * (s - c));

    printf("Area of triangle = %.2f", area);

    return 0;
}
```

### 📖 Explanation

* `float a, b, c` → sides of triangle
* `s = (a + b + c) ÷ 2` → semi-perimeter
* `area = √[s × (s-a) × (s-b) × (s-c)]` → Heron’s formula
* `sqrt()` → used for square root (from `math.h`)
* `printf()` → displays result

### ▶️ Output

```id="k7d3mn"
Enter three sides of triangle: 3 4 5
Area of triangle = 6.00
```

---
