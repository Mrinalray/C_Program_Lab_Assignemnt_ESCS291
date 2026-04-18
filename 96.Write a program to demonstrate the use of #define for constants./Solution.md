## 📌 Program 96: Demonstrate the Use of `#define` for Constants

### 💻 Code

```c id="d8m3qx"
#include <stdio.h>

// Define constant using #define
#define PI 3.14

int main() {
    float radius, area;

    printf("Enter radius: ");
    scanf("%f", &radius);

    area = PI * radius * radius;

    printf("Area of circle = %.2f\n", area);

    return 0;
}
```

### 📖 Explanation

* `#define PI 3.14` → defines a constant
* No memory allocation (handled by preprocessor)
* Replaces `PI` with `3.14` before compilation
* Used for fixed values

### ▶️ Output

```id="m6q2zn"
Enter radius: 5
Area of circle = 78.50
```

---
