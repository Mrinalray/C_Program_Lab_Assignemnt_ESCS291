## 📌 Program 78: Find the Sum of Two Matrices Using Pointers

### 💻 Code

```c id="m3n8qx"
#include <stdio.h>

// Function to add two matrices using pointers
void addMatrix(int *a, int *b, int *result, int rows, int cols) {
    int i, j;

    for (i = 0; i < rows; i++) {
        for (j = 0; j < cols; j++) {
            *(result + i * cols + j) =
            *(a + i * cols + j) + *(b + i * cols + j);
        }
    }
}

int main() {
    int a[10][10], b[10][10], result[10][10];
    int i, j, rows, cols;

    printf("Enter number of rows and columns: ");
    scanf("%d %d", &rows, &cols);

    printf("Enter elements of first matrix:\n");
    for (i = 0; i < rows; i++) {
        for (j = 0; j < cols; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    printf("Enter elements of second matrix:\n");
    for (i = 0; i < rows; i++) {
        for (j = 0; j < cols; j++) {
            scanf("%d", &b[i][j]);
        }
    }

    addMatrix((int *)a, (int *)b, (int *)result, rows, cols);

    printf("Sum of matrices:\n");
    for (i = 0; i < rows; i++) {
        for (j = 0; j < cols; j++) {
            printf("%d ", result[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```

### 📖 Explanation

* Uses pointers to access matrix elements
* Formula: `*(arr + i × cols + j)` → 2D to 1D mapping
* Adds corresponding elements of both matrices
* Stores result in third matrix

### ▶️ Output

```id="x8m2zn"
Enter number of rows and columns: 2 2
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

---
