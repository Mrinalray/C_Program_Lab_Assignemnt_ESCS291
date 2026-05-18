# Program 120: Find the Product of Two Matrices

💻 Code

```c id="v8m3qp"
#include <stdio.h>

int main() {

    int a[3][3], b[3][3], product[3][3];
    int i, j, k;

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

    // Initialize product matrix
    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            product[i][j] = 0;
        }
    }

    // Multiply matrices
    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            for(k = 0; k < 3; k++) {
                product[i][j] += a[i][k] * b[k][j];
            }
        }
    }

    // Display result
    printf("\nProduct of matrices:\n");

    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            printf("%d ", product[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```

📖 Explanation

* Two 3×3 matrices are stored in arrays `a` and `b`
* Matrix multiplication is performed using nested loops
* Each element is calculated using:
  `product[i][j] += a[i][k] * b[k][j]`
* The result is stored in matrix `product`
* Finally, the product matrix is displayed

▶️ Output

```text id="q4x7rn"
Enter elements of first matrix:
1 2 3
4 5 6
7 8 9

Enter elements of second matrix:
9 8 7
6 5 4
3 2 1

Product of matrices:
30 24 18
84 69 54
138 114 90
```
