## 📌 Program 86: Check if a Number is an Armstrong Number Using Recursion

### 💻 Code

```c id="a6m3qx"
#include <stdio.h>
#include <math.h>

// Recursive function to count digits
int countDigits(int n) {
    if (n == 0)
        return 0;
    return 1 + countDigits(n / 10);
}

// Recursive function to calculate Armstrong sum
int armstrongSum(int n, int digits) {
    if (n == 0)
        return 0;
    return pow(n % 10, digits) + armstrongSum(n / 10, digits);
}

int main() {
    int num, digits;

    printf("Enter a number: ");
    scanf("%d", &num);

    digits = countDigits(num);

    if (armstrongSum(num, digits) == num)
        printf("Armstrong Number");
    else
        printf("Not an Armstrong Number");

    return 0;
}
```

### 📖 Explanation

* `countDigits()` → recursively counts digits
* `armstrongSum()` → recursively calculates sum of digits^power
* Base case: when number becomes 0
* Compare sum with original number

### ▶️ Output

```id="m3q8zn"
Enter a number: 153
Armstrong Number
```

---
