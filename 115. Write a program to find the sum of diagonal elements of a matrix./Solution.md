# Program 115: Find the Sum of Diagonal Elements of a Matrix

💻 Code

```c id="d7m4qp"
#include <stdio.h>

int main() {

    int a[3][3];
    int i, j, sum = 0;

    // Input matrix
    printf("Enter elements of matrix:\n");

    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    // Find sum of diagonal elements
    for(i = 0; i < 3; i++) {
        sum = sum + a[i][i];
    }

    // Display result
    printf("Sum of diagonal elements = %d", sum);

    return 0;
}
```

📖 Explanation

* A 3×3 matrix is stored in array `a`
* Diagonal elements are those where row index and column index are equal
* The condition used is:
  `a[i][i]`
* A loop is used to add all diagonal elements
* The result is stored in variable `sum`
* Finally, the sum is displayed

▶️ Output

```text id="n5v8rk"
Enter elements of matrix:
1 2 3
4 5 6
7 8 9

Sum of diagonal elements = 15
```
