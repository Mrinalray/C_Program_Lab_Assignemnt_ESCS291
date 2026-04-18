## 📌 Program 52: Print the First 10 Armstrong Numbers

### 💻 Code

```c id="a5m3qx"
#include <stdio.h>
#include <math.h>

int main() {
    int num = 1, count = 0;

    printf("First 10 Armstrong numbers:\n");

    while (count < 10) {
        int temp = num, digits = 0;
        float sum = 0;

        // Count digits
        while (temp != 0) {
            temp = temp / 10;
            digits++;
        }

        temp = num;

        // Calculate Armstrong sum
        while (temp != 0) {
            int remainder = temp % 10;
            sum += pow(remainder, digits);
            temp = temp / 10;
        }

        if ((int)sum == num) {
            printf("%d ", num);
            count++;
        }

        num++;
    }

    return 0;
}
```

### 📖 Explanation

* Checks each number starting from `1`
* Counts digits of number
* Calculates sum of digits raised to power of digit count
* If equal to original → Armstrong number
* Stops after printing 10 such numbers

### ▶️ Output

```id="m4q9zn"
First 10 Armstrong numbers:
1 2 3 4 5 6 7 8 9 153
```

---
