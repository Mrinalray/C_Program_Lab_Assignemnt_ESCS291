## 📌 Program 57: Print Number of Days in a Month (Using Switch-Case)

### 💻 Code

```c id="m7n3qx"
#include <stdio.h>

int main() {
    int month, year;

    printf("Enter month (1-12): ");
    scanf("%d", &month);

    printf("Enter year: ");
    scanf("%d", &year);

    switch(month) {
        case 1: case 3: case 5: case 7:
        case 8: case 10: case 12:
            printf("31 days");
            break;

        case 4: case 6: case 9: case 11:
            printf("30 days");
            break;

        case 2:
            if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0))
                printf("29 days (Leap Year)");
            else
                printf("28 days");
            break;

        default:
            printf("Invalid month");
    }

    return 0;
}
```

### 📖 Explanation

* `month` → stores month number (1–12)
* `switch(month)` → checks month
* Groups months with 31 and 30 days
* February handled separately
* Leap year condition used for Feb

### ▶️ Output

```id="p8m2zn"
Enter month (1-12): 2
Enter year: 2024
29 days (Leap Year)
```

---
