## 📌 Program 58: Print Season Based on Month (Using Switch-Case)

### 💻 Code

```c id="s5m3qx"
#include <stdio.h>

int main() {
    int month;

    printf("Enter month (1-12): ");
    scanf("%d", &month);

    switch(month) {
        case 12: case 1: case 2:
            printf("Winter Season");
            break;

        case 3: case 4: case 5:
            printf("Spring Season");
            break;

        case 6: case 7: case 8:
            printf("Summer Season");
            break;

        case 9: case 10: case 11:
            printf("Autumn Season");
            break;

        default:
            printf("Invalid month");
    }

    return 0;
}
```

### 📖 Explanation

* `int month;` → stores month number
* `switch(month)` → selects season
* Months grouped into seasons
* `default` handles invalid input

### ▶️ Output

```id="q7m2zn"
Enter month (1-12): 4
Spring Season
```

---
