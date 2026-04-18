## 📌 Program 59: Print Name of the Month (1–12)

### 💻 Code

```c id="m8p3qx"
#include <stdio.h>

int main() {
    int month;

    printf("Enter a number (1-12): ");
    scanf("%d", &month);

    switch(month) {
        case 1:
            printf("January");
            break;
        case 2:
            printf("February");
            break;
        case 3:
            printf("March");
            break;
        case 4:
            printf("April");
            break;
        case 5:
            printf("May");
            break;
        case 6:
            printf("June");
            break;
        case 7:
            printf("July");
            break;
        case 8:
            printf("August");
            break;
        case 9:
            printf("September");
            break;
        case 10:
            printf("October");
            break;
        case 11:
            printf("November");
            break;
        case 12:
            printf("December");
            break;
        default:
            printf("Invalid input! Please enter a number between 1 and 12.");
    }

    return 0;
}
```

### 📖 Explanation

* `int month;` → stores input number
* `switch(month)` → matches number to month
* Each case prints corresponding month name
* `default` handles invalid input

### ▶️ Output

```id="x3q8zn"
Enter a number (1-12): 10
October
```

---
