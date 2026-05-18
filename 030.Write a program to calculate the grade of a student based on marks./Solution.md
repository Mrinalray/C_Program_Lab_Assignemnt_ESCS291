## 📌 Program 30: Calculate Grade of a Student

### 💻 Code

```c id="g9m3qx"
#include <stdio.h>

int main() {
    int marks;

    printf("Enter marks: ");
    scanf("%d", &marks);

    if (marks >= 90)
        printf("Grade: A");
    else if (marks >= 75)
        printf("Grade: B");
    else if (marks >= 60)
        printf("Grade: C");
    else if (marks >= 40)
        printf("Grade: D");
    else
        printf("Grade: F");

    return 0;
}
```

### 📖 Explanation

* `int marks;` → stores student marks
* `scanf()` → takes input
* Conditions check range of marks
* Assigns grade based on performance

### ▶️ Output

```id="r3q8zn"
Enter marks: 82
Grade: B
```

---
