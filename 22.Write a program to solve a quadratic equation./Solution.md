## 📌 Program 22: Solve a Quadratic Equation

### 💻 Code

```c id="q8m3zx"
#include <stdio.h>
#include <math.h>

int main() {
    float a, b, c, discriminant, root1, root2, real, imag;

    printf("Enter coefficients a, b and c: ");
    scanf("%f %f %f", &a, &b, &c);

    discriminant = b * b - 4 * a * c;

    if (discriminant > 0) {
        root1 = (-b + sqrt(discriminant)) / (2 * a);
        root2 = (-b - sqrt(discriminant)) / (2 * a);
        printf("Roots are real and different:\n");
        printf("Root1 = %.2f, Root2 = %.2f", root1, root2);
    }
    else if (discriminant == 0) {
        root1 = -b / (2 * a);
        printf("Roots are real and equal:\n");
        printf("Root = %.2f", root1);
    }
    else {
        real = -b / (2 * a);
        imag = sqrt(-discriminant) / (2 * a);
        printf("Roots are complex:\n");
        printf("Root1 = %.2f + %.2fi\n", real, imag);
        printf("Root2 = %.2f - %.2fi", real, imag);
    }

    return 0;
}
```

### 📖 Explanation

* `a, b, c` → coefficients of equation
* `discriminant = b² - 4ac` → determines nature of roots
* If > 0 → real & different roots
* If = 0 → real & equal roots
* If < 0 → complex roots
* `sqrt()` → used from `math.h`

### ▶️ Output

```
Enter coefficients a, b and c: 1 -3 2
Roots are real and different:
Root1 = 2.00, Root2 = 1.00
```

---
