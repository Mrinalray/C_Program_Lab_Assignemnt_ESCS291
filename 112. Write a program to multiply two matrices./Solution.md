# Program 112: Multiply Two Matrices

💻 Code

```c id="m8q2vn"
#include <stdio.h>

int main() {

    int a[2][2], b[2][2], product[2][2];
    int i, j, k;

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

    // Initialize product matrix
    for(i = 0; i < 2; i++) {
        for(j = 0; j < 2; j++) {
            product[i][j] = 0;
        }
    }

    // Multiply matrices
    for(i = 0; i < 2; i++) {
        for(j = 0; j < 2; j++) {
            for(k = 0; k < 2; k++) {
                product[i][j] += a[i][k] * b[k][j];
            }
        }
    }

    // Display result
    printf("Product of matrices:\n");

    for(i = 0; i < 2; i++) {
        for(j = 0; j < 2; j++) {
            printf("%d ", product[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```

📖 Explanation

* Two 2×2 matrices are stored in arrays `a` and `b`
* Matrix multiplication is performed using nested loops
* Each element is calculated using:
  `product[i][j] += a[i][k] * b[k][j]`
* The result is stored in matrix `product`
* Finally, the product matrix is displayed

▶️ Output

```text id="x5n8rw"
Enter elements of first matrix:
1 2
3 4

Enter elements of second matrix:
5 6
7 8

Product of matrices:
19 22
43 50
```
