## Program 111: Add Two Matrices

💻 Code

```c id="k7q2mx"
#include <stdio.h>

int main() {

    int a[2][2], b[2][2], sum[2][2];
    int i, j;

    // Input first matrix
    printf("Enter elements of first matrix:\n");
    for(i = 0; i < 2; i++) {
        for(j = 0; j < 2; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    // Input second matrix
    printf("Enter elements of second matrix:\n");
    for(i = 0; i < 2; i++) {
        for(j = 0; j < 2; j++) {
            scanf("%d", &b[i][j]);
        }
    }

    // Add matrices
    for(i = 0; i < 2; i++) {
        for(j = 0; j < 2; j++) {
            sum[i][j] = a[i][j] + b[i][j];
        }
    }

    // Display result
    printf("Sum of matrices:\n");

    for(i = 0; i < 2; i++) {
        for(j = 0; j < 2; j++) {
            printf("%d ", sum[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```

📖 Explanation

* Two 2×2 matrices are stored in arrays `a` and `b`
* Corresponding elements of both matrices are added
* Result is stored in another matrix `sum`
* Nested loops are used for matrix operations
* Finally, the sum matrix is displayed

▶️ Output

```text id="p5v9rt"
Enter elements of first matrix:
1 2
3 4

Enter elements of second matrix:
5 6
7 8

Sum of matrices:
6 8
10 12
```
