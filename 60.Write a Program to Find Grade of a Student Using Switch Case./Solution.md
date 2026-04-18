## 📌 Program 60: Find Grade of a Student Using Switch-Case

### 💻 Code

```c id="g3m8qx"
#include <stdio.h>

int main() {
    int marks;

    printf("Enter marks: ");
    scanf("%d", &marks);

    switch(marks / 10) {
        case 10:
        case 9:
            printf("Grade: A");
            break;
        case 8:
            printf("Grade: B");
            break;
        case 7:
            printf("Grade: C");
            break;
        case 6:
            printf("Grade: D");
            break;
        case 5:
        case 4:
            printf("Grade: E");
            break;
        default:
            printf("Grade: F");
    }

    return 0;
}
```

### 📖 Explanation

* `marks / 10` → converts marks into range (e.g., 85 → 8)
* `switch` checks range instead of exact value
* Multiple cases grouped (like 9 & 10 → Grade A)
* `default` handles low marks

### ▶️ Output

```id="q9m2zn"
Enter marks: 78
Grade: C
```

---
