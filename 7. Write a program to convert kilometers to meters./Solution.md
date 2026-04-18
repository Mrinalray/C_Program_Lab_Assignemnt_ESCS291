## 📌 Program 7: Convert Kilometers to Meters

### 💻 Code

```c id="km4z2x"
#include <stdio.h>

int main() {
    float km, meters;

    printf("Enter distance in kilometers: ");
    scanf("%f", &km);

    meters = km * 1000;

    printf("Distance in meters = %.2f", meters);

    return 0;
}
```

### 📖 Explanation

* `float km, meters;` → variables to store distance
* `scanf()` → takes input in kilometers
* `meters = km × 1000` → conversion formula
* `printf()` → displays the result

### ▶️ Output

```id="m9x2qs"
Enter distance in kilometers: 2.5
Distance in meters = 2500.00
```

---
