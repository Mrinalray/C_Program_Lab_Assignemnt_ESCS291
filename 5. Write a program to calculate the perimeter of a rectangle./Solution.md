## 📌 Program 5: Calculate Perimeter of a Rectangle

### 💻 Code

```c id="x7m2qp"
#include <stdio.h>

int main() {
    float length, width, perimeter;

    printf("Enter length and width: ");
    scanf("%f %f", &length, &width);

    perimeter = 2 * (length + width);

    printf("Perimeter of rectangle = %.2f", perimeter);

    return 0;
}
```

### 📖 Explanation

* `float length, width, perimeter;` → variables for dimensions and result
* `scanf()` → takes input values
* `perimeter = 2 × (length + width)` → formula for perimeter
* `printf()` → displays the result

### ▶️ Output

```id="q2v8sn"
Enter length and width: 10 5
Perimeter of rectangle = 30.00
```

---
