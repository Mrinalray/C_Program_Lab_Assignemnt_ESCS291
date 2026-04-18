## 📌 Program 23: Check if a Triangle is Equilateral, Isosceles, or Scalene

### 💻 Code

```c id="t7m4qx"
#include <stdio.h>

int main() {
    int a, b, c;

    printf("Enter three sides of triangle: ");
    scanf("%d %d %d", &a, &b, &c);

    if (a == b && b == c)
        printf("Equilateral Triangle");
    else if (a == b || b == c || a == c)
        printf("Isosceles Triangle");
    else
        printf("Scalene Triangle");

    return 0;
}
```

### 📖 Explanation

* `int a, b, c;` → sides of triangle
* `a == b && b == c` → all sides equal → Equilateral
* `a == b || b == c || a == c` → any two equal → Isosceles
* Else → all sides different → Scalene

### ▶️ Output

```id="n5q2zn"
Enter three sides of triangle: 5 5 5
Equilateral Triangle
```

---
