## 📌 Program 15: Calculate Area of a Square

### 💻 Code

```c id="s8m3qx"
#include <stdio.h>

int main() {
    float side, area;

    printf("Enter side of square: ");
    scanf("%f", &side);

    area = side * side;

    printf("Area of square = %.2f", area);

    return 0;
}
```

### 📖 Explanation

* `float side, area;` → variables for side and result
* `scanf()` → takes input value
* `area = side × side` → formula for area (side²)
* `printf()` → displays result

### ▶️ Output

```id="v2q9zn"
Enter side of square: 6
Area of square = 36.00
```

---
