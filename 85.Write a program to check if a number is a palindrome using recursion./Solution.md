## 📌 Program 85: Check if a Number is a Palindrome Using Recursion

### 💻 Code

```c id="p9m3qx"
#include <stdio.h>

// Recursive function to reverse number
int reverse(int n, int rev) {
    if (n == 0)
        return rev;
    else
        return reverse(n / 10, rev * 10 + (n % 10));
}

// Function to check palindrome
int isPalindrome(int n) {
    if (n == reverse(n, 0))
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

* `reverse(n, rev)` → recursively reverses number
* Base case: when `n = 0`, return reversed value
* `isPalindrome()` compares original and reversed
* Returns `1` if palindrome, else `0`

### ▶️ Output

```id="q2m8zn"
Enter a number: 121
Palindrome Number
```

---
