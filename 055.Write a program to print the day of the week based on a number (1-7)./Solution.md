## 📌 Program 55: Print Day of the Week (1–7)

### 💻 Code

```c id="d9m3qx"
#include <stdio.h>

int main() {
    int day;

    printf("Enter a number (1-7): ");
    scanf("%d", &day);

    switch(day) {
        case 1:
            printf("Monday");
            break;
        case 2:
            printf("Tuesday");
            break;
        case 3:
            printf("Wednesday");
            break;
        case 4:
            printf("Thursday");
            break;
        case 5:
            printf("Friday");
            break;
        case 6:
            printf("Saturday");
            break;
        case 7:
            printf("Sunday");
            break;
        default:
            printf("Invalid input! Please enter a number between 1 and 7.");
    }

    return 0;
}
```

### 📖 Explanation

* `int day;` → stores input number
* `switch(day)` → selects corresponding day
* Each case prints a specific weekday
* `default` handles invalid input

### ▶️ Output

```id="m6q2zn"
Enter a number (1-7): 3
Wednesday
```

---
