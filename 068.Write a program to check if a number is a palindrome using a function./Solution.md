## 📌 Program 68: Check if a Number is a Palindrome Using a Function

### 💻 Code

```c id="p8m3qx"
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

// Function to check palindrome
int isPalindrome(int n) {
    if (n == reverseNumber(n))
        return 1;
    else
        return 0;
}

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (isPalindrome(num))
        printf("Palindrome Number");
    else
        printf("Not a Palindrome Number");

    return 0;
}
```

### 📖 Explanation

* `reverseNumber()` → reverses the number
* `isPalindrome()` → compares original and reversed
* Returns `1` if palindrome, else `0`
* `main()` prints result based on function

### ▶️ Output

```id="q3m9zn"
Enter a number: 121
Palindrome Number
```

---
