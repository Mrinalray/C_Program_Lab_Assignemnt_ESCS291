## 📌 Program 88: Demonstrate the Use of Enum

### 💻 Code

```c id="e3m8qx"
#include <stdio.h>

// Define enum
enum Day {Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday};

int main() {
    enum Day today;

    today = Wednesday;

    printf("Day value = %d\n", today);

    if (today == Wednesday)
        printf("Today is Wednesday");

    return 0;
}
```

### 📖 Explanation

* `enum Day` → defines named constants
* Values start from `0` by default

  * Sunday = 0, Monday = 1, ...
* `today` → variable of enum type
* Improves readability compared to integers

### ▶️ Output

```id="m5q2zn"
Day value = 3
Today is Wednesday
```

---
