## 📌 Program 53: Print the First 10 Palindrome Numbers

### 💻 Code

```c id="p5m3qx"
#include <stdio.h>

int main() {
    int num = 1, count = 0;

    printf("First 10 palindrome numbers:\n");

    while (count < 10) {
        int original = num, reversed = 0, remainder;

        // Reverse number
        while (original != 0) {
            remainder = original % 10;
            reversed = reversed * 10 + remainder;
            original = original / 10;
        }

        if (reversed == num) {
            printf("%d ", num);
            count++;
        }

        num++;
    }

    return 0;
}
```

### 📖 Explanation

* Starts checking from `1`
* Reverses each number
* If original == reversed → palindrome
* Stops after printing 10 palindrome numbers

### ▶️ Output

```id="m8q2zn"
First 10 palindrome numbers:
1 2 3 4 5 6 7 8 9 11
```

---
