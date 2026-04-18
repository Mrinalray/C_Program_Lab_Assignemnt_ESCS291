## 📌 Program 69: Check if a Number is an Armstrong Number Using a Function

### 💻 Code

```c id="a3m8qx"
#include <stdio.h>
#include <math.h>

// Function to count digits
int countDigits(int n) {
    int count = 0;
    while (n != 0) {
        n = n / 10;
        count++;
    }
    return count;
}

// Function to check Armstrong
int isArmstrong(int n) {
    int original = n, remainder, digits;
    float sum = 0;

    digits = countDigits(n);

    while (n != 0) {
        remainder = n % 10;
        sum += pow(remainder, digits);
        n = n / 10;
    }

    return (int)sum == original;
}

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (isArmstrong(num))
        printf("Armstrong Number");
    else
        printf("Not an Armstrong Number");

    return 0;
}
```

### 📖 Explanation

* `countDigits()` → counts number of digits
* `isArmstrong()` → calculates sum of digits raised to power of digit count
* Compares sum with original number
* Returns `1` if Armstrong, else `0`

### ▶️ Output

```id="m6q2zn"
Enter a number: 153
Armstrong Number
```

---
