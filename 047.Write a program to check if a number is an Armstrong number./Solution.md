## 📌 Program 47: Check if a Number is an Armstrong Number

### 💻 Code

```c id="a7m3qx"
#include <stdio.h>
#include <math.h>

int main() {
    int num, original, remainder, n = 0;
    float result = 0;

    printf("Enter a number: ");
    scanf("%d", &num);

    original = num;

    // Count digits
    while (original != 0) {
        original = original / 10;
        n++;
    }

    original = num;

    // Calculate Armstrong sum
    while (original != 0) {
        remainder = original % 10;
        result += pow(remainder, n);
        original = original / 10;
    }

    if ((int)result == num)
        printf("Armstrong Number");
    else
        printf("Not an Armstrong Number");

    return 0;
}
```

### 📖 Explanation

* Counts number of digits (`n`)
* Each digit raised to power `n`
* Sum of powers compared with original number
* If equal → Armstrong number

### ▶️ Output

```id="m2q8zn"
Enter a number: 153
Armstrong Number
```

---
