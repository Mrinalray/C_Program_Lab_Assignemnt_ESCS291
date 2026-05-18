## 📌 Program 28: Check if a Triangle is Valid (Given its Sides)

### 💻 Code

```c id="k8m3qx"
#include <stdio.h>

int main() {
    int a, b, c;

    printf("Enter three sides of triangle: ");
    scanf("%d %d %d", &a, &b, &c);

    if ((a + b > c) && (a + c > b) && (b + c > a))
        printf("Triangle is valid");
    else
        printf("Triangle is not valid");

    return 0;
}
```

### 📖 Explanation

* `int a, b, c;` → sides of triangle
* Triangle validity condition:

  * `a + b > c`
  * `a + c > b`
  * `b + c > a`
* All conditions must be true (`&&`)

### ▶️ Output

```id="z5q2xn"
Enter three sides of triangle: 3 4 5
Triangle is valid
```

---
