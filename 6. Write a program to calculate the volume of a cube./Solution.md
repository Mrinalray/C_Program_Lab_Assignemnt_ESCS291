## 📌 Program 6: Calculate Volume of a Cube

### 💻 Code

```c id="q8m4zs"
#include <stdio.h>

int main() {
    float side, volume;

    printf("Enter side of cube: ");
    scanf("%f", &side);

    volume = side * side * side;

    printf("Volume of cube = %.2f", volume);

    return 0;
}
```

### 📖 Explanation

* `float side, volume;` → variables for side and result
* `scanf()` → takes input (side of cube)
* `volume = side × side × side` → formula (side³)
* `printf()` → displays the result

### ▶️ Output

```id="n2k9dp"
Enter side of cube: 4
Volume of cube = 64.00
```

---
