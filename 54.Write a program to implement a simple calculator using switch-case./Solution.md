## 📌 Program 54: Simple Calculator Using Switch-Case

### 💻 Code

```c id="c8m3qx"
#include <stdio.h>

int main() {
    float a, b;
    char op;

    printf("Enter operator (+, -, *, /): ");
    scanf(" %c", &op);

    printf("Enter two numbers: ");
    scanf("%f %f", &a, &b);

    switch(op) {
        case '+':
            printf("Result = %.2f", a + b);
            break;
        case '-':
            printf("Result = %.2f", a - b);
            break;
        case '*':
            printf("Result = %.2f", a * b);
            break;
        case '/':
            if (b != 0)
                printf("Result = %.2f", a / b);
            else
                printf("Error! Division by zero");
            break;
        default:
            printf("Invalid operator");
    }

    return 0;
}
```

### 📖 Explanation

* `char op;` → stores operator
* `switch(op)` → selects operation
* Each `case` performs different calculation
* Division checks for zero to avoid error
* `default` handles invalid input

### ▶️ Output

```id="x2q9zn"
Enter operator (+, -, *, /): *
Enter two numbers: 5 4
Result = 20.00
```

---
