## 📌 Program 4: Convert Fahrenheit to Celsius

### 💻 Code

```c
#include <stdio.h>

int main() {
    float fahrenheit, celsius;

    printf("Enter temperature in Fahrenheit: ");
    scanf("%f", &fahrenheit);

    celsius = (fahrenheit - 32) * 5 / 9;

    printf("Temperature in Celsius = %.2f", celsius);

    return 0;
}
```

### 📖 Explanation

* `float fahrenheit, celsius;` → variables to store temperatures
* `scanf()` → takes input in Fahrenheit
* `(fahrenheit - 32) × 5 ÷ 9` → formula to convert to Celsius
* `printf()` → displays the result

### ▶️ Output

```
Enter temperature in Fahrenheit: 98.6
Temperature in Celsius = 37.00
```

---
