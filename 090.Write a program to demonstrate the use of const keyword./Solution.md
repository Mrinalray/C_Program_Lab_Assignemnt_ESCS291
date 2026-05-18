## 📌 Program 90: Demonstrate the Use of `const` Keyword

### 💻 Code

```c id="c4m8qx"
#include <stdio.h>

int main() {
    const float PI = 3.14;
    float radius, area;

    printf("Enter radius: ");
    scanf("%f", &radius);

    area = PI * radius * radius;

    printf("Area of circle = %.2f", area);

    return 0;
}
```

### 📖 Explanation

* `const float PI = 3.14;` → constant variable
* Value of `PI` cannot be changed during program execution
* Used to prevent accidental modification
* Improves code safety and readability

### ▶️ Output

```id="m2q9zn"
Enter radius: 5
Area of circle = 78.50
```

---
