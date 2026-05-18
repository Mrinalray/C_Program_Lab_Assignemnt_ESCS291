# Program 117: Find the Sum of Each Row and Column of a Matrix

💻 Code

```c id="f8m3qp"
#include <stdio.h>

int main() {

    int a[3][3];
    int i, j, rowSum, colSum;

    // Input matrix
    printf("Enter elements of matrix:\n");

    for(i = 0; i < 3; i++) {
        for(j = 0; j < 3; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    // Sum of each row
    printf("\nSum of each row:\n");

    for(i = 0; i < 3; i++) {

        rowSum = 0;

        for(j = 0; j < 3; j++) {
            rowSum = rowSum + a[i][j];
        }

        printf("Row %d Sum = %d\n", i + 1, rowSum);
    }

    // Sum of each column
    printf("\nSum of each column:\n");

    for(j = 0; j < 3; j++) {

        colSum = 0;

        for(i = 0; i < 3; i++) {
            colSum = colSum + a[i][j];
        }

        printf("Column %d Sum = %d\n", j + 1, colSum);
    }

    return 0;
}
```

📖 Explanation

* A 3×3 matrix is stored in array `a`
* Nested loops are used to access matrix elements
* For row sum:

  * Elements of each row are added together
* For column sum:

  * Elements of each column are added together
* The sums are stored in `rowSum` and `colSum`
* Finally, all row sums and column sums are displayed

▶️ Output

```text id="r5n9vk"
Enter elements of matrix:
1 2 3
4 5 6
7 8 9

Sum of each row:
Row 1 Sum = 6
Row 2 Sum = 15
Row 3 Sum = 24

Sum of each column:
Column 1 Sum = 12
Column 2 Sum = 15
Column 3 Sum = 18
```
