## 📌 Program 14: Calculate Area of a Rectangle

### 💻 Code

```c id="w3m8qx"
#include <stdio.h>

int main() {
    float length, width, area;

    printf("Enter length and width: ");
    scanf("%f %f", &length, &width);

    area = length * width;

    printf("Area of rectangle = %.2f", area);

    return 0;
}
```

### 📖 Explanation

* `float length, width, area;` → variables for dimensions and result
* `scanf()` → takes input values
* `area = length × width` → formula for area
* `printf()` → displays result

### ▶️ Output

```id="x7q2zn"
Enter length and width: 10 5
Area of rectangle = 50.00
```

---
