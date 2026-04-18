## 📌 Program 67: Reverse a Number Using a Function

### 💻 Code

```c id="r9m3qx"
#include <stdio.h>

// Function to reverse a number
int reverseNumber(int n) {
    int reversed = 0;

    while (n != 0) {
        reversed = reversed * 10 + (n % 10);
        n = n / 10;
    }

    return reversed;
}

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    printf("Reversed number = %d", reverseNumber(num));

    return 0;
}
```

### 📖 Explanation

* `reverseNumber(int n)` → user-defined function
* Extracts digits using `% 10`
* Builds reversed number step-by-step
* Returns result to `main()`
* `main()` prints output

### ▶️ Output

```id="v4m8zn"
Enter a number: 1234
Reversed number = 4321
```

---
