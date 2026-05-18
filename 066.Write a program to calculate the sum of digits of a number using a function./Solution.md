## 📌 Program 66: Calculate Sum of Digits of a Number Using a Function

### 💻 Code

```c id="s4m9qx"
#include <stdio.h>

// Function to calculate sum of digits
int sumOfDigits(int n) {
    int sum = 0;

    while (n != 0) {
        sum += n % 10;
        n = n / 10;
    }

    return sum;
}

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    printf("Sum of digits = %d", sumOfDigits(num));

    return 0;
}
```

### 📖 Explanation

* `sumOfDigits(int n)` → user-defined function
* Extracts each digit using `% 10`
* Adds digits to `sum`
* Returns result to `main()`
* `main()` prints output

### ▶️ Output

```id="p6m2zn"
Enter a number: 1234
Sum of digits = 10
```

---
