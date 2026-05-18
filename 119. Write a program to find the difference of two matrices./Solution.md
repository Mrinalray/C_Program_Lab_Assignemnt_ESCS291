# Program 119: Find the Difference of Two Matrices

💻 Code

```c id="n6q2vk"
#include <stdio.h>

int main() {

    int a[3][3], b[3][3], difference[3][3];
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

    // Find difference of matrices
    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            difference[i][j] = a[i][j] - b[i][j];
        }
    }

    // Display result
    printf("\nDifference of matrices:\n");

    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            printf("%d ", difference[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```

📖 Explanation

* Two 3×3 matrices are stored in arrays `a` and `b`
* Corresponding elements of both matrices are subtracted
* The result is stored in matrix `difference`
* Nested loops are used for matrix operations
* Finally, the difference matrix is displayed

▶️ Output

```text id="m9x4rp"
Enter elements of first matrix:
9 8 7
6 5 4
3 2 1

Enter elements of second matrix:
1 2 3
4 5 6
7 8 9

Difference of matrices:
8 6 4
2 0 -2
-4 -6 -8
```
