## 📌 Program 20: Check if a Year is a Leap Year

### 💻 Code

```c id="y6m3qx"
#include <stdio.h>

int main() {
    int year;

    printf("Enter a year: ");
    scanf("%d", &year);

    if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0))
        printf("Leap Year");
    else
        printf("Not a Leap Year");

    return 0;
}
```

### 📖 Explanation

* `int year;` → variable to store year
* `year % 4 == 0` → divisible by 4
* `year % 100 != 0` → not divisible by 100
* `year % 400 == 0` → special case for century years
* Combines conditions to correctly identify leap years

### ▶️ Output

```id="x9q2zn"
Enter a year: 2024
Leap Year
```

---
