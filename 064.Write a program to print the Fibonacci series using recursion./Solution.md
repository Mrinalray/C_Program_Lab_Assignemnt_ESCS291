## 📌 Program 64: Print Fibonacci Series Using Recursion

### 💻 Code

```c id="f9m3qx"
#include <stdio.h>

// Recursive function for Fibonacci
int fibonacci(int n) {
    if (n == 0)
        return 0;
    else if (n == 1)
        return 1;
    else
        return fibonacci(n - 1) + fibonacci(n - 2);
}

int main() {
    int i, n;

    printf("Enter number of terms: ");
    scanf("%d", &n);

    printf("Fibonacci series: ");

    for (i = 0; i < n; i++) {
        printf("%d ", fibonacci(i));
    }

    return 0;
}
```

### 📖 Explanation

* `fibonacci(n)` → recursive function
* Base cases: `f(0)=0`, `f(1)=1`
* Recursive case: `f(n)=f(n-1)+f(n-2)`
* Loop calls function for each term

### ▶️ Output

```id="q3m8zn"
Enter number of terms: 7
Fibonacci series: 0 1 1 2 3 5 8
```

---

