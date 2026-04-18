## 📌 Program 50: Print the First 20 Prime Numbers

### 💻 Code

```c id="p6m3qx"
#include <stdio.h>

int main() {
    int count = 0, num = 2, i, isPrime;

    printf("First 20 prime numbers:\n");

    while (count < 20) {
        isPrime = 1;

        for (i = 2; i <= num / 2; i++) {
            if (num % i == 0) {
                isPrime = 0;
                break;
            }
        }

        if (isPrime) {
            printf("%d ", num);
            count++;
        }

        num++;
    }

    return 0;
}
```

### 📖 Explanation

* Start checking from `2` (first prime)
* Check divisibility using loop
* If not divisible → prime number
* Continue until 20 primes are printed

### ▶️ Output

```id="m9q4zn"
First 20 prime numbers:
2 3 5 7 11 13 17 19 23 29 31 37 41 43 47 53 59 61 67 71
```

---
