# Program 118: Find the Sum of Two Matrices

💻 Code

```c id="k4m8qp"
#include <stdio.h>

int main() {

    int a[3][3], b[3][3], sum[3][3];
    int i, j;

    // Input first matrix
    printf("Enter elements of first matrix:\n");

    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    // Input second matrix
    printf("Enter elements of second matrix:\n");

    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            scanf("%d", &b[i][j]);
        }
    }

    // Add matrices
    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            sum[i][j] = a[i][j] + b[i][j];
        }
    }

    // Display result
    printf("\nSum of matrices:\n");

    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            printf("%d ", sum[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```

📖 Explanation

* Two 3×3 matrices are stored in arrays `a` and `b`
* Corresponding elements of both matrices are added
* The result is stored in matrix `sum`
* Nested loops are used for matrix operations
* Finally, the sum matrix is displayed

▶️ Output

```text id="p7v2xn"
Enter elements of first matrix:
1 2 3
4 5 6
7 8 9

Enter elements of second matrix:
9 8 7
6 5 4
3 2 1

Sum of matrices:
10 10 10
10 10 10
10 10 10
```
