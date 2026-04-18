## 📌 Program 3: Calculate Area of a Circle

### 💻 Code

```c
#include <stdio.h>

int main() {
    float radius, area;

    printf("Enter radius: ");
    scanf("%f", &radius);

    area = 3.14 * radius * radius;

    printf("Area of circle = %.2f", area);

    return 0;
}
```

### 📖 Explanation

* `float radius, area;` → variables to store radius and area
* `scanf()` → takes radius input from user
* `area = 3.14 × radius × radius` → formula for area of circle
* `printf()` → displays the result

### ▶️ Output

```
Enter radius: 5
Area of circle = 78.50
```

---
