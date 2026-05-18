## 📌 Program 35: Check if a Number is a Palindrome

### 💻 Code

```c id="n4m8qx"
#include <stdio.h>

int main() {
    int num, original, reversed = 0, remainder;

    printf("Enter a number: ");
    scanf("%d", &num);

    original = num;

    while (num != 0) {
        remainder = num % 10;
        reversed = reversed * 10 + remainder;
        num = num / 10;
    }

    if (original == reversed)
        printf("Palindrome Number");
    else
        printf("Not a Palindrome Number");

    return 0;
}
```

### 📖 Explanation

* Reverse the number using loop
* Compare original and reversed
* If equal → palindrome

### ▶️ Output

```id="q7m2zn"
Enter a number: 121
Palindrome Number
```

---
