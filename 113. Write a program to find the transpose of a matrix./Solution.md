# Program 113: Find the Transpose of a Matrix

💻 Code

```c id="y7k2qp"
#include <stdio.h>

int main() {

    int a[3][3], transpose[3][3];
    int i, j;

    // Input matrix
    printf("Enter elements of matrix:\n");

    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    // Find transpose
    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            transpose[j][i] = a[i][j];
        }
    }

    // Display transpose matrix
    printf("Transpose of matrix:\n");

    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            printf("%d ", transpose[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```

📖 Explanation

* A 3×3 matrix is stored in array `a`
* The transpose of a matrix is obtained by interchanging rows and columns
* Elements are copied using:
  `transpose[j][i] = a[i][j]`
* Nested loops are used for matrix operations
* Finally, the transpose matrix is displayed

▶️ Output

```text id="z3k8vf"
Enter elements of matrix:
1 2 3
4 5 6
7 8 9

Transpose of matrix:
1 4 7
2 5 8
3 6 9
```
